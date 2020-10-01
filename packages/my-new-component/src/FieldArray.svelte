<script>
  console.log('my-new-component FieldArray')
  let names = ['a']

  console.log('synchronously changing names to [a, b]')
  names = ['a', 'b']
</script>

<slot names={names} />
