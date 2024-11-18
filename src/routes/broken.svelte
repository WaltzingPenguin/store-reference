<script lang="ts">
import { readable } from 'svelte/store'

const store = readable(null)

interface Props {
    children?: import('svelte').Snippet
}
let { children }: Props = $props()
</script>

{ $store }
{@render children?.()}
