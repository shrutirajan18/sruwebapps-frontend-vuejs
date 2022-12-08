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
    background-color: rgb(196, 255, 248);
    padding: 1em;
    color: rgb(128, 128, 128);
    margin: 5px;
    
}
</style>
