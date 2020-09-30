<script>
import { FieldArray } from "my-new-component";
import { UsesContext } from "my-new-component";
</script>

<FieldArray let:names>
  {#each names as name, i}
    <div>
      {name}:
      <UsesContext />
    </div>
  {/each}
</FieldArray>
