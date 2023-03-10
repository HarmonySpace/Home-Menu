<script>

</script>



<template>
    <div class="container">
        <div class="row header">
            <h1>HOME.MENU</h1>
            <p>Hello, this is your home page</p>
            <input class="row" type="text" v-model="filterlist">
        </div>
    </div>
</template>
    


<style>
@import url(./assets/css/normalize.css);
@import url(./assets/css/skeleton.css);

.header {
    text-align: center;
    margin: 100px 0;
    padding: 10px;
}

.header h1 {
    font-size: 150px;
    font-weight: bold;
    text-align: center;
}

.header p {
    font-size: 25px;
    font-weight: 100;
    text-align: center;
}
</style>
