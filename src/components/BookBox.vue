<template>
    <div v-for="book in books" :key="book.id" >
    <BookItem :book= "book" />
    </div>
</template>

<script>


import BookItem from './BookItem.vue'

export default{
    name: 'BookBox',
    props:{
        books: Array
    },
    components:{
        BookItem    
    }
}

</script>

<style scoped>

.bookbox{
    background-color: bisque;
    padding: 1em;
    color: gray;
    margin: 5px;
    
}
</style>
