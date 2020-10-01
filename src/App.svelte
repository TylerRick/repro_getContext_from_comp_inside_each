<script>
import { FieldArray } from "my-new-component";

// Using this results in error:
//   Uncaught (in promise) Error: Function called outside component initialization
import { UsesContext } from "my-new-component";

// But changing it to use a copy of the exact some component located in local app works without any error:
// import UsesContext from "./UsesContext.svelte";
</script>

<FieldArray let:names>
  <div>{names}</div>
  <UsesContext />
</FieldArray>
