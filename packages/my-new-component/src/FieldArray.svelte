<script>
  console.log('my-new-component FieldArray')
  let names = ['a']

  setTimeout(() => {
    console.log('changing names to [a, b] from async callback')
    names = ['a', 'b']
  }, 1000);
</script>

<slot names={names} />
