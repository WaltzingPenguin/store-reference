<script lang="ts">
import { readable } from 'svelte/store'

interface Props {
    children?: import('svelte').Snippet
}
let { children }: Props = $props()

const store = readable(null)
</script>

{ $store }
{@render children?.()}
