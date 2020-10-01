<script>
  console.log('my-new-component FieldArray')
  let names = ['a']

  const callback = () => {
    names = ['a', 'b']
    console.log('changing names variable from async callback')
  }

  setTimeout(callback, 1000);
</script>

<slot names={names} />
