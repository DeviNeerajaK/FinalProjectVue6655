<template>

    <div :class="book.available ? 'green': 'red' ">
        <h2>Motel Name : {{book.motelname}}</h2>
        <address> Address : {{book.address}}</address>
        <address> Contact Us : {{book.number}}</address>
        <h4> Total Rooms : {{book.totalrooms}}</h4>
        <h4> Rooms Available : {{book.roomavailability}}</h4>
        <h4> Cost : {{book.cost}}</h4>
        <h4> Ratings : {{book.rating}}</h4>
        
        
    </div>

</template>

<script>


export default{
    name: 'BookItem',
    props:{
        book: Array
    }
}


</script>

<style scoped>


h4{
    margin: 2px;
}

div{
    background-color: #ffb89e;
    color: black;
    padding: 1em;
    text-align: center;
}

.red{
background-color: orangered !important;

}
.green{
    color: white;
    background-color: green;
}


</style>