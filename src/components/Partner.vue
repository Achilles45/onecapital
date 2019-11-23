<template>
    <div class="partners__wrapper">
        <div class="container">
            <div class="row pb-2">
                <div class="col-md-4"></div>
                <div class="col-md-4 text-center">
                    <h3>Our Awards and Mentions</h3>
                    <hr>
                </div>
                <div class="col-md-4"></div>
            </div>
            <div class="row">
                <div class="col-md-3 col-sm-6 col-xs-6">
                    <img src="../assets/brand1.png" class="img-fluid brand brand1" alt="">
                </div>
                 <div class="col-md-3 col-sm-6 col-xs-6">
                    <img src="../assets/brand2.png" class="img-fluid brand brand1" alt="">
                </div>
                 <div class="col-md-3 col-sm-6 col-xs-6">
                    <img src="../assets/brand3.jpg" class="img-fluid brand brand1" alt="">
                </div>
                 <div class="col-md-3 col-sm-6 col-xs-6">
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
    h3{
        color: $primary-color;
        font-weight: bold;
    }
    .brand1{
        max-width: 120px;
        height: auto;
    }
}
@media only screen and (max-width: 768px){
    .brand1{
        max-width: 80px !important;
        height: auto;
    }
}
</style>