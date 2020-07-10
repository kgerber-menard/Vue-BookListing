<template>
  <form class="" action="#" method="post">
    <input v-model="bookTitle" type="text" name="title" value="" placeholder="Book Title">
    <input v-model="bookAuthor" type="text" name="author" value="" placeholder="Book Author">
    <button type="submit" name="button">Add Book</button>
    @submit=bookSubmit(bookTitle, bookAuthor);
  </form>
</template>
<script>
  export default {
    name: 'BookForm',
    props: ['books'],
    data() {
      return{
        bookTitle: '',
        bookAuthor: ''
      }
    },
    methods: {
      bookSubmit(bootTitle, bookAuthor){
        this.$emit('addBook', bootTitle, bookAuthor);
      }
    }
  }
</script>
<style>

</style>
