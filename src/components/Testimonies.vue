<template>
    <div class="testimonies__section container-fluid">
        <div class="container">
            <div class="row">
                <div class="col-md-4">
                    <h4>Testimonials</h4>
                    <!-- <hr> -->
                </div>
            </div>
            <div class="scrolling-wrapper">
               <div class="testimony__card">
                    <p>Lorem ipsum dolor, sit amet consectetur adipisicing elit. Earum ea iure corrupti animi excepturi obcaecati deserunt ab amet, ipsum praesentium?</p>
                    <hr>
                    <small>Achilles Usuoyibo</small>
               </div>
               <div class="testimony__card">
                    <p>Lorem ipsum dolor, sit amet consectetur adipisicing elit. Earum ea iure corrupti animi excepturi obcaecati deserunt ab amet, ipsum praesentium?</p>
                    <hr>
                    <small>Achilles Usuoyibo</small>
               </div>
               <div class="testimony__card">
                    <p>Lorem ipsum dolor, sit amet consectetur adipisicing elit. Earum ea iure corrupti animi excepturi obcaecati deserunt ab amet, ipsum praesentium?</p>
                    <hr>
                    <small>Achilles Usuoyibo</small>
               </div>
               <div class="testimony__card">
                    <p>Lorem ipsum dolor, sit amet consectetur adipisicing elit. Earum ea iure corrupti animi excepturi obcaecati deserunt ab amet, ipsum praesentium?</p>
                    <hr>
                    <small>Achilles Usuoyibo</small>
               </div><div class="testimony__card">
                    <p>Lorem ipsum dolor, sit amet consectetur adipisicing elit. Earum ea iure corrupti animi excepturi obcaecati deserunt ab amet, ipsum praesentium?</p>
                    <hr>
                    <small>Achilles Usuoyibo</small>
               </div>
               <div class="testimony__card">
                    <p>Lorem ipsum dolor, sit amet consectetur adipisicing elit. Earum ea iure corrupti animi excepturi obcaecati deserunt ab amet, ipsum praesentium?</p>
                    <small>Achilles Usuoyibo</small>
               </div>
               <div class="testimony__card">
                    <p>Lorem ipsum dolor, sit amet consectetur adipisicing elit. Earum ea iure corrupti animi excepturi obcaecati deserunt ab amet, ipsum praesentium?</p>
                    <hr>
                    <small>Achilles Usuoyibo</small>
               </div>
            </div>
        </div>
    </div>
</template>
<style lang="scss" scoped>
@import '../styles/_colors';
.testimonies__section{
    background: $primary-color;
    padding: 4rem 0;
    color: #fff;
    position: relative;
    hr{
        background: #fafafa;
        // opacity: .2;
    }
    .scrolling-wrapper {
       display: flex;
       min-width: 100%;
       min-height: 200px;
       overflow-x: auto;
       .testimony__card{
           min-width: 300px;
           background: #fff;
           color:#627081;
           padding: 1.5rem;
           box-shadow: 7px 5px 30px 0 rgba(71,72,121,.15) !important;
           margin: 2rem .5rem;
           border-radius: 3px;
           p{
               font-size: .8rem;
               opacity: .8;
           }
           small{
               font-weight: bold;
           }
       }
        .scrolling-wrapper {
        -webkit-overflow-scrolling: touch;
        }
    }
}
</style>