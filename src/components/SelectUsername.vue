<template lang='pug'>
h1 Hello, World!
   div.select-username
      form
      input(placeholder="Your username: ")
      button=Send
</template>

<script>
export default {
  name: 'SelectUsername',
  props: {},
};
</script>
