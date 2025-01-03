<script>

  const meow = $state(['m', 'e', 'o', 'w', '!'])

  const meowLouder = () => {
    meow.splice(2, 0, 'o');
    // console.log($state.snapshot(booty));
  }

  $inspect(meow).with(() => console.log('Here!'));


</script>

<h1>{meow.join('')}</h1>
<button onclick={meowLouder}>Meow louder</button>


<style>
  button {
    cursor: pointer;
  }
</style>
