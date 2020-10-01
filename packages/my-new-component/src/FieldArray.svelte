<script>
  console.log('my-new-component FieldArray')
  let names = ['a']

  const handleClick = () => {
    console.log('changing names to [a, b] from event callback')
    names = ['a', 'b']
  }
</script>

<button on:click={handleClick}>Blow up</button>
<slot names={names} />
