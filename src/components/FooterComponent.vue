<template>
    <footer>
        <div class="top-footer">
            <div class="container">
                   <BannerFooter
                   :BannerList="BannerItems"
                   />                                                                                                            
            </div>
        </div>
        <div class="middle-footer">
            <div class="container">
                <div class="col-sx">
                    <div class="list-col">
                        <h4>DC COMICS</h4>
                        <ul>
                            <li><a href="#">Characters</a></li>
                            <li><a href="#">Comics</a></li>
                            <li><a href="#">Movies</a></li>
                            <li><a href="#">TV</a></li>
                            <li><a href="#">Games</a></li>
                            <li><a href="#">Videos</a></li>
                            <li><a href="#">News</a></li>
                        </ul>
                    </div>
                    <div class="list-col">
                        <h4>DC</h4>
                        <ul>
                            <li><a href="#">Terms of Use</a></li>
                            <li><a href="#">Privacy policy (New)</a></li>
                            <li><a href="#">Ad Choice</a></li>
                            <li><a href="#">Advertising</a></li>
                            <li><a href="#">Jobs</a></li>
                            <li><a href="#">Subscripions</a></li>
                            <li><a href="#">Talent Workshops</a></li>
                            <li><a href="#">CPSC Certifications</a></li>
                            <li><a href="#">Ratings</a></li>
                            <li><a href="#">Shop Help</a></li>
                            <li><a href="#">Contact Us</a></li>
                        </ul>
                    </div>
                    <div class="list-col">
                        <h4>SITES</h4>
                        <ul>
                            <li><a href="#">DC</a></li>
                            <li><a href="#">MAD Magazine</a></li>
                            <li><a href="#">DC Kids</a></li>
                            <li><a href="#">DC Universe</a></li>
                            <li><a href="#">DC Power Visa</a></li>
                        </ul>
                    </div>
                    <div class="list-col">
                        <h4>SHOP</h4>
                        <ul>
                            <li><a href="#">Shop DC</a></li>
                            <li><a href="#">Shop Dc Collectibles</a></li>
                        </ul>
                    </div>
                </div>
                <div class="col-dx">
                    <img src="../assets/img/dc-logo-bg.png" alt="">
                </div>
            </div>
        </div>
        <div class="bottom-footer">
            <div class="container">
                <button><a href="#">SIGN-UP NOW!</a></button>
                <div class="bf-col-dx">
                    <span>FOLLOW US</span>
                    <img src="../assets/img/footer-facebook.png" alt="facebook">
                    <img src="../assets/img/footer-twitter.png" alt="twitter">
                    <img src="../assets/img/footer-youtube.png" alt="youtube">
                    <img src="../assets/img/footer-pinterest.png" alt="pinterest">
                    <img src="../assets/img/footer-periscope.png" alt="periscope">
                </div>
            </div>
        </div>
    </footer>
</template>

<script>
import BannerFooter from './BannerFooter.vue';
import BannerItemsArr from '../assets/data/BannerItems';
export default {
    name:'FooterComponent',
    components: {
        BannerFooter
        },
    data(){
    return{ 
        BannerItems:BannerItemsArr
    }
    },
}
</script>

<style lang="scss" scoped>
.top-footer{
    height: 100px;
    background-color: #0E88F9;
    .container{
        height: 100%;
    }
}

.middle-footer{
    height: 400px;
    overflow: hidden;
    background-image: url(../assets/img/footer-bg.jpg);
    .container{
        margin-top: -50px;
        display: flex;
        .col-sx{
        display: flex;
        flex-wrap: wrap;
        width: 40%;
        margin-top: 50px;
        .list-col{
        width: calc(100% / 3);
        color: white;
            h4{
                padding-top: 20px;
                padding-bottom: 15px;
            }
            ul{
                list-style: none;
                li{
                    padding-bottom: 5px;
                }
            }
        }
        }
        .col-dx{
            display: flex;
            align-items: center;
            justify-content: center;
            width: 60%;
            img{
                width: 80%;
            }
        }
    }
    
}

.bottom-footer{
    height: 60px;
    background-color: #303030;
    .container{
        display: flex;
        justify-content: space-between;
        align-items: center;
        height: 100%;
        button{
            border: 1px solid #0E88F9;
            padding: 10px 15px;
            background-color: #303030;
            align-self: center;
        }
        .bf-col-dx{
            display: flex;
            align-items: center;
            span{
                padding: 0 15px;
                color: #0E88F9;
                font-weight: bold;
            }
            img{
                padding: 0 7px;
                width: 40px;
            }
        }
    }
}
</style>