<template>
    <div class="why__wrapper container-fluid">
        <div class="container">
            <div class="row">
                <div class="col-12 text-center">
                    <h4>Why Choose Us?</h4>
                </div>
            </div>
            <div class="card__wrapper">
                <div class="why__card">
                    <i class="fa fa-comments icons"></i>&nbsp;&nbsp;&nbsp;&nbsp; <h6>24/7 Support</h6>
                    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Possimus molestias exercitationem placeat quasi, obcaecati earum.</p>
                </div>
                 <div class="why__card">
                    <i class="fa fa-cubes icons"></i>&nbsp;&nbsp;&nbsp;&nbsp; <h6>Diverse Collections</h6>
                    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Possimus molestias exercitationem placeat quasi, obcaecati earum.</p>
                </div>
                 <div class="why__card">
                    <i class="fa fa-clock icons"></i>&nbsp;&nbsp;&nbsp;&nbsp; <h6>Realtime Info</h6>
                    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Possimus molestias exercitationem placeat quasi, obcaecati earum.</p>
                </div>
            </div>
        </div>
    </div>
</template>
<style lang="scss" scoped>
@import '../styles/colors';
.why__wrapper{
    padding: 5rem 0;
    background: #fff;
    h4{
        color: $primary-color;
    }
    .card__wrapper{
        display: grid;
        grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
        grid-gap: 20px;
        margin-top: 2rem;
        .why__card{
            box-shadow: 7px 5px 30px 0 rgba(71,72,121,.15);
            padding: 1.5rem;
            border-radius: 3px;
            .icons{
                color:$primary-color;
                font-size: 2.5rem;
                padding-bottom: .7rem;
            }
            h6{
                font-weight: normal;
                color:$primary-color;
                padding-bottom: .5rem;
            }
            p{
                color:#627081;
                font-size: .82rem;
                opacity: .85;
            }
        }
    }
}
</style>