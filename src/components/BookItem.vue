<template>
        <div>

            <h2>{{book.Brand}}</h2>
            <h4>{{book.Company}}</h4>
            <h4>{{book.Stock_Exchange}}</h4>
            <h4>{{book.Ticker_Symbol}}</h4>
            <h4>{{book.Price}}</h4>
            <h4>{{book.Founded_Year}}</h4>
            <h4>{{book.Average_Volume}}</h4>
            


        </div>

</template>

<script>

    export default{
        name: 'BookItem',
        props: {
            book: Array
        }
    }
    

</script>


<style scoped>


h4{
    margin: 2px;
    color:#fb00ff;
}
h2{
    color:red;
}
div{
     background-color: #f39c7c;
     color:#226cb6;
     color: black;
     padding: 1em;
     margin: 5px;   
     border-radius: 30px;
    }




</style>