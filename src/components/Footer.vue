<template>
    <footer class="container-fluid">
        <div class="container">
            <div class="row">
                <div class="col-md-4">
                    <h4>Company Address</h4>
                    <p><i class="fa fa-home icons"></i>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 1 Jinojah Street, Along Owhelogbo Road, Ozoro, Delta State, Nigeria.</p>
                    <p><i class="fa fa-envelope icons"></i>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; support@oncecapital.com</p>
                    <p><i class="fa fa-phone icons"></i>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; +2348103515205</p>
                </div>
                <div class="col-md-4">
                    <h4>Useful Links</h4>
                    <ul>
                        <li><router-link to="/">Terms & Conditions</router-link></li>
                        <li><router-link to="/">Investment policies</router-link></li>
                        <li><router-link to="/">Careers</router-link></li>
                        <li><router-link to="/">Team</router-link></li>
                        <li><router-link to="/">Home</router-link></li>
                    </ul>
                </div>
                <div class="col-md-4">
                    <h4>Newsletter</h4>
                    <p>Keep up to date with the latest Oncecapital strategies.</p><br>
                    <form action="">
                      <div class="form-group">
                            <input type="text" class="form-control" placeholder="First Name">
                      </div>
                        <div class="form-group">
                            <input type="email" class="form-control" placeholder="Enter Your Email">
                        </div>
                        <button type="submit" class="news__btn">SUBMIT</button>
                    </form>
                </div>
            </div>
        </div>
        <hr>
        <div class="container">
            <small>Onecapital &copy; Copyright 2019. All rights reserved.</small>
        </div>
    </footer>
</template>
<style lang="scss" scoped>
@import '../styles/colors';
footer{
    background: $primary-color;
    padding: 5rem 0;
    color: #fff;
    h4{
        padding-bottom: 1.2rem;
    }
    p{
        opacity: .8;
        font-size: .9rem;
    }
    a{
        color: #efefef;
        text-decoration: none;
        line-height: 2;
        font-size: .9rem;
    }
    // .icons{
    //     margin-right: 5rem !important;
    // }
    form{
        input{
            height: 2.94rem;
            border-radius: 0px;
            box-shadow: none !important;

        }
        .news__btn{
            background: #F7C039;
            border: none;
            padding: 1rem 2rem;
            border-radius: 30px;
            width: 50%;
        }
    }
}
</style>