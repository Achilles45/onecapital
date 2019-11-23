<template>
    <div class="banner__wrapper container-fluid">
            <div class="navbar__wrapper">
                <nav class="navbar navbar-expand-lg">
                    <div class="container">
                <router-link to="/" class="logo"><img src="../assets/logo-img.png" alt=""></router-link>
                <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
                    <i class="fa fa-bars"></i>
                </button>

                <div class="collapse navbar-collapse" id="navbarSupportedContent">
                    <ul class="navbar-nav ml-auto">
                    <li class="nav-item active">
                       <router-link to="/" class="nav-link">Home</router-link>
                    </li>
                    <li class="nav-item">
                        <router-link to="/about" class="nav-link">About</router-link>
                    </li>
                    <li class="nav-item">
                        <router-link to="/about" class="nav-link">Team</router-link>
                    </li>
                     <li class="nav-item">
                        <router-link to="/about" class="nav-link">Contact</router-link>
                    </li>
                     <li class="nav-item">
                        <router-link to="/about" class="nav-link">Signup</router-link>
                    </li>
                     <li class="nav-item">
                        <router-link to="/about" class="nav-link">Login</router-link>
                    </li>
                    </ul>
                </div>
                </div>
                </nav>
            </div>
            <!--End of navbar section
            ==============-->
            <!--Hero section
            =================-->
            <div class="hero-section container">
                <div class="row">
                    <div class="col-md-6">
                        <h1>The most trusted digital assets exchange</h1>
                        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Beatae aut modi pariatur officia harum assumenda voluptas laudantium quibusdam aliquid totam!</p>
                        <router-link to="/register" class="register__btn">Create a free Account &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; <i class="fa fa-arrow-right icons"></i></router-link>
                    </div>
                    <div class="col-md-6 img__wrapper">
                        <div class="balls one"></div>
                        <div class="balls two"></div>
                        <div class="balls three"></div>
                        <div class="balls four"></div>
                        <div class="balls five"></div>
                        <div class="balls six"></div>
                        <div class="balls seven"></div>
                        <div class="balls eight"></div>
                        <img src="../assets/map.png" class="img-fluid map d-none d-md-block" alt="">
                    </div>
                </div>
            </div>
    </div>
</template>
<script>
export default {
    // mounted(){
    //    this.fixNav();
    // },
    methods:{
        fixNav:function(){
            const nav = document.querySelector('.navbar__wrapper');
            window.onscroll =function(){
                if(pageYOffset > 50){
                    nav.classList.add('fixnav');
                }else{
                    nav.classList.remove('fixnav');
                }
            }
        }
    }
}
</script>
<style lang="scss" scoped>
@import '../styles/colors';
.banner__wrapper{
    background: $primary-color;
    color:#fff;
    height: 100vh;
    width: 100%;
    .navbar__wrapper{
        padding-top: 1.8rem;
        .nav-item{
            margin: 0 .7rem;
        }
        // .logo{
        //     color: #fff;
        //     font-weight: bolder;
        //     text-decoration: none;
        //     // font-family: 'Varela Round' !important;
        // }
        .nav-link{
            text-decoration: none;
            text-transform: uppercase;
            font-size: .75rem;
            color: #f4f4f4;
            font-weight: normal;
            opacity: .85;
        }
        .nav-item:nth-child(1), .nav-item:nth-child(2), .nav-item:nth-child(3), .nav-item:nth-child(4){
            padding-top: .3rem;
        }
        .nav-item:nth-child(5), .nav-item:nth-child(6){
            border: .8px solid #fff;
            border-radius: 2px;
            padding: .3rem 1.8rem;
        }
        .fa-bars{
            color: #fff;
        }
    }

    .hero-section{
        padding-top: 9rem;
        h1{
            padding-bottom: .8rem;
            text-transform: capitalize;
            text-shadow: 0.03em 0.03em 0.05em rgba(0,0,0,.10);
            font-weight: 800;
        }
        p{
            opacity: .8;
            font-size: .9rem;
            line-height: 1.6;
            padding-bottom: 1rem;
        }
        .register__btn{
            background: #fff;
            color:$primary-color;
            font-size: .9rem;
            text-decoration: none;
            padding: 1.3rem 3rem;
            font-weight: bold;
            border-radius: 3px;
            opacity: .9;
            box-shadow:  5px 5px 0px rgba(72,73,121,.10);
        }
        .icons{
            animation-name: move;
            animation-duration: 2s;
            animation-iteration-count: infinite;
            animation-direction: alternate;
        }
        .img__wrapper{
            position:relative;
        }
        .balls{
            position: absolute;
            padding: .2rem;
            border-radius: 50%;
            background:#fafafa !important;
            animation-name: animate;
            animation-duration: 1s;
            animation-iteration-count: infinite;
            animation-direction: alternate;
         }
         .one{
             right: 40% !important;
             top: 60%;
         }
         .two{
             right: 300px !important;
         }
         .three{
             right: 600px !important;
         }
         .four{
             right: 100px !important;
         }
         .five{
             bottom: 20%;
             right: 100px;
         }
         .six{
             bottom: 70%;
             right: 180px;
         }
         .seven{
             bottom: 20%;
             left: 100px;
         }
         .eight{
             bottom: 50%;
             right: 60%;
         }
    }
}

//Animate
@keyframes animate{
    from{
        opacity: .4;
    }
    to{
        opacity: 1;
         color: #efefef !important;
    }
}
//Animate
@keyframes move{
    from{
        transform: translateX(0px);
    }
    to{
        transform: translateX(10px);
    }
}
@media only screen and (max-width: 768px) {
    .banner__wrapper{
        height: 92vh !important;
    }
     .nav-item:nth-child(5), .nav-item:nth-child(6){
            border: none !important;
            border-radius: 0px !important;
            padding: 0 !important;
        }
    .hero-section{
        padding-top: 5rem !important;
        h1{
            font-size: 1.8rem;
        }
        p{
            font-size: .85rem;
            padding-bottom: 1.2rem;
        }
    }
    .map{
        max-width: 320px;
        height: auto;
        margin-top: 3rem;
    }
}

.fixnav{
    position: fixed;
    top: 0;
    z-index: 1000;
    box-shadow: 5px 0px 30px rgba(0,0,0,.10) !important;
    background: #fff;
    width: 100% !important;
    left: 0;
    .logo{
        color: $primary-color !important;
        font-weight: bolder !important;
    }
    .nav-link{
        color: $primary-color !important;
        font-weight: bold !important;
    }
    .nav-item:nth-child(5), .nav-item:nth-child(6){
            border: .8px solid $primary-color !important;
            border-radius: 2px;
            padding: .3rem 1.8rem;
        }
        .fa-bars{
            color: #627081 !important;
        }
        @media only screen and (max-width: 768px){
            .nav-item:nth-child(5), .nav-item:nth-child(6){
            border: none !important;
            border-radius: 0px !important;
            padding: 0 !important;
        }
        }
}
</style>