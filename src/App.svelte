<script>
  import { UsesContext } from "my-new-component";

  let names = ['a']

  const callback = () => {
    names = ['a', 'b']
    console.log('changing names variable from async callback')
    // console.log(`FieldArray fieldState for ${name}:`, fields.names())
  }

  setTimeout(callback, 1000);
</script>

{#each names as name, i}
  <div>
    {name}:
    <UsesContext />
  </div>
{/each}
