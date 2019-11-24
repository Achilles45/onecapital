<template>
    <div class="signin container-fluid">
        <div class="container">
            <div class="signin__contents">
                <div class="form__wrapper">
                    <div class="heading">
                        <h4>Login</h4>
                        <small>Please provide your credentials to continue</small>
                    </div>
                     <form action="">
                    <div class="form-group">
                        <label for="email">Email Address *</label>
                        <input type="email" class="form-control" v-model="email" placeholder="Your Email">
                    </div>
                    <div class="form-group">
                        <label for="password">Password *</label>
                        <input type="password" class="form-control" v-model="password" placeholder="Password">
                    </div>
                    <button type="submit" class="register__btn">Signin</button>
                </form>
                <div class="bottom text-center">
                    <p>Yet to register? <router-link to="/register">Create account</router-link></p>
                </div>
                </div>
            </div>
        </div>
    </div>
</template>
<script>
export default {
    data(){
        return{
            email:null,
            password:null,
            errors:[]
        }
    }
}
</script>
<style lang="scss" scoped>
@import '../styles/colors';
.signin{
    background: #F6F7FF;
    height: 100vh;
    .signin__contents{
        padding: 7rem 0;
    }
    .form__wrapper{
        max-width: 450px;
        background: #fff;
        border-radius: 4px;
        margin: 0 auto;
        padding: 2rem;
        box-shadow: 7px 5px 30px 0 rgba(71,72,121,.15);
    }
    .heading h4{
        color: #404040;
        font-weight: bold;
    }
    .heading small{
        color: #627081;
        font-weight: bold;
    }
      form{
            padding-top: 2.5rem;
            label{
                color: #627081;
                font-weight: bold;
                font-size: .87rem;
            }
            input{
                height: 2.7rem;
                 border-radius: 3px;
                font-size: .9rem;
                box-shadow: none;
            }
            button{
                width: 100%;
                background: $primary-color;
                color: #fff;
                border:none;
                padding: .7rem 0;
                border-radius: 3px;
            }
        }
        .bottom{
            padding-top: 1rem;
            p{
                font-size: .9rem;
            }
        }
}
</style>