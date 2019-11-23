<template>
    <div class="partners__wrapper">
        <div class="container">
            <div class="row pb-2">
                <div class="col-md-4"></div>
                <div class="col-md-4 text-center">
                    <h4>Our Awards and Mentions</h4>
                    <hr>
                </div>
                <div class="col-md-4"></div>
            </div>
           <div class="brand__wrapper">
               <div class="brand__box">
                   <img src="../assets/brand1.png" class="img-fluid brand brand1" alt="">
               </div>
                <div class="brand__box">
                   <img src="../assets/brand2.png" class="img-fluid brand brand1" alt="">
               </div>
                <div class="brand__box">
                   <img src="../assets/brand3.jpg" class="img-fluid brand brand1" alt="">
               </div>
                <div class="brand__box">
                   <img src="../assets/brand4.png" class="img-fluid brand brand1" alt="">
               </div>
           </div>
        </div>
    </div>
</template>
<style lang="scss" scoped>
@import '../styles/colors';
.partners__wrapper{
    padding: 3rem 0;
    background: #fff;
    h4{
        color: $primary-color;
        font-weight: bold;
    }
    .brand1{
        max-width: 120px;
        height: auto;
    }
}
.brand__wrapper{
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(50px, 1fr));
    grid-gap: 30px;
}
@media only screen and (max-width: 768px){
    .brand1{
        max-width: 60px !important;
        height: auto;
    }
}
</style>