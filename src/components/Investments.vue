<template>
    <div class="investments container-fluid">
        <div class="container">
            <div class="row">
                <div class="col-md-6">
                    <div class="main__wrapper">
                        <div class="header__wrapper text-center">
                            <h5>10% - 15%</h5>
                        </div><br><br><br>
                        <p>Lorem, ipsum dolor sit amet consectetur adipisicing elit. Omnis eius illum commodi voluptatem similique vel exercitationem nam? Pariatur porro voluptas eaque quaerat error nostrum sapiente.</p>
                    </div>
                </div>
                <div class="col-md-1"></div>
                <div class="col-md-5 invest">
                    <h3>Invest and manage your assets in one platform!</h3>
                    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Dolore sit voluptate optio repellat quod praesentium deleniti earum eveniet libero explicabo, corporis quaerat tenetur suscipit maiores, voluptatum nostrum dolores fugit molestias.</p>
                    <router-link to="/register" class="register__btn">Register now</router-link>
                </div>
            </div>
        </div>
    </div>
</template>
<style lang="scss" scoped>
@import '../styles/colors';
.investments{
    padding: 5rem 0;
    background: #fafafa;
    .main__wrapper{
        background: #fff;
        padding: .8rem .7rem;
        border-radius: 4px;
        box-shadow: 7px 5px 30px 0 rgba(71,72,121,.15);
        .header__wrapper{
            background: $primary-color;
            color: #fff;
            padding: 4rem;
            border-radius: 5px;
            margin-bottom: 1rem;
        }
        p{
            font-size: .9rem;
            color: #627081;
            opacity: .9;
        }
    }
    .invest{
        h3{
            font-weight: bold;
            padding-bottom: .7rem;
            color: $primary-color;
            line-height: 1.3;
            text-transform: capitalize;
        }
        p{
            color: #627081;
            font-size: .85rem;
            padding-bottom: 1.4rem;
            opacity: .9;
        }
        .register__btn{
            background: #fff;
            color:$primary-color;
            font-size: .9rem;
            text-decoration: none;
            padding: 1.3rem 3rem;
            font-weight: normal;
            border-radius: 3px;
            opacity: .9;
            box-shadow:  2px 2px 0px rgba(231, 231, 238, 0.9);
        }
        .register__btn:hover{
            background: $primary-color;
            color:#fff;
            transition: all ease-in .5s;
            box-shadow: none !important;
        }
    }
}

@media only screen and (max-width: 768px){
    .invest{
        h3{
            padding-top: 3rem;
            font-size: 1.2rem;
        }
        p{
            font-size: .85rem;
        }
    }
}
</style>