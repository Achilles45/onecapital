<template>
    <div class="about__wrapper container-fluid">
        <div class="container">
            <div class="row">
                <div class="col-md-6">
                    <h3>We provide you with realtime  data to help you make informed investments</h3>
                    <P>Lorem ipsum dolor sit amet consectetur adipisicing elit. Quia provident ipsum ducimus nesciunt, sequi repellendus aliquam esse dolorem qui ab. Animi rem quisquam blanditiis nisi corporis tempora quod natus, quos error tempore alias at dolor dignissimos ipsam amet, reiciendis necessitatibus?</P>
                </div>
                <div class="col-md-1"></div>
                <div class="col-md-5">
                    <div class="box__wrapper">
                        <div class="content__overlay">
                            <small>Lorem ipsum dolor sit amet consectetur adipisicing.</small>
                        </div>
                       <small class="small">Lorem ipsum dolor sit amet consectetur adipisicing elit. Ducimus, consequatur. Omnis quas asperiores dolor neque ipsum excepturi suscipit iure a explicabo velit voluptatibus sed consequuntur</small><br>
                       <small class="small">Lorem ipsum dolor sit amet consectetur adipisicing elit. Iure recusandae repellat magni officiis animi error? Ipsa repellendus eligendi quo explicabo cumque..</small>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>
<style lang="scss" scoped>
@import '../styles/colors';
.about__wrapper{
background: #F6F7FF;
padding: 5rem 0;
h3{
    font-weight: bold;
    padding-bottom: .7rem;
    color: $primary-color;
    text-transform: capitalize;
}
p{
    color: #627081;
    font-size: .9rem;
    opacity: .9;
}
}

.box__wrapper{
    box-shadow: 7px 5px 30px 0 rgba(71,72,121,.15);
    padding: 1.8rem 1.5rem;
    border-radius: 4px;
    position: relative;
    .small{
        color: #627081;
    }
    .content__overlay{
        position: absolute;
        background: $primary-color;
        color: #fff !important;
        top: 34px;
        padding: 2rem;
        border-radius: 4px;
        left: -40px;
        animation-name: animate;
        animation-duration: 2s;
        animation-iteration-count: infinite;
        animation-direction: alternate;
    }
}

//Animate
@keyframes animate{
    from{
        transform: translateX(-20px);
    }
    to{
        transform: translateX(20px);
    }
}
@media only screen and (max-width: 768px){
    h3{
        font-size: 1rem;
    }
    .small{
        font-size: .85rem;
    }
    .content__overlay{
        width: 85%;
        left: 7% !important;
    }
}
</style>