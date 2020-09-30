<script>
// import { FieldArray } from "my-new-component";
import { FieldArray } from "svelte-final-form";

// import { UsesContext } from "my-new-component";
import { UsesContext } from "svelte-final-form";

</script>

<FieldArray let:names>
  {#each names as name, i}
    <div>
      {name}:
      <UsesContext />
    </div>
  {/each}
</FieldArray>
