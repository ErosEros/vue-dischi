<template>
    <main>
        <div class="container row">
            <div class="d-flex flex-column justify-content-between card" v-for="cd in cdList" :key="cd.title" >
            <div class="box-card">
                <img :src="cd.poster" alt="">
            </div>
            <h5>{{ cd.title }}</h5>
            <h6>{{cd.author}} <h6>{{cd.year}}</h6></h6>
            


        </div>



        </div>
        

    </main>
  
</template>

<script>
export default {
name : 'MainComponent',
props : {
    cdList : Array,
}
}
</script>

<style lang="scss" scoped>
main {
    background-color: hsl(209deg, 33%, 17%);
}

.container {
    width: 1200px;
    margin: 0 auto;
    padding: 30px 0;

}
.card {
    width: calc(100% / 5 - 40px);
    margin:20px;
    text-align: center;
    height: 350px;
    background-color: hsl(210deg 22% 23%);
    color: white;
    align-items: center;
    padding-top: 15px;

;
    .box-card {
        width: 150px;
        height: 150px;
        
        
    }
}
h6 {
    color: rgb(88, 100, 112);
}

</style>