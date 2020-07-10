<template>
  <div>
    <h1>{{title}}</h1>
    <ul>
      <li>Star Trek TNG</li>
      <li>Star Trek DS9</li>
      <li>Star Trek Voyager</li>
    </ul>
  </div>

</template>
<script>
export default {
  name: 'BookList',
  data() {
    return {
      title: 'All Books'
    }
  }
}
</script>
<style>
  h1, h2 {
    font-weight: normal;
  }
  ul {
    list-style-type: none;
    padding: 0;
  }
  li {
    display: block;
    margin: 0 10px;
  }

</style>
