<script>
  console.log('my-new-component UsesContext')
  import {setContext, getContext} from 'svelte'

  // Using onMount also causes the same error:
  // import { onDestroy, onMount } from "svelte";
  // onMount(() => {
  //   console.log('UsesContext: onMount')
  // });

  const key = {}
  setContext(key, 'context')
  let context = getContext(key)
</script>
UsesContext: {context}
