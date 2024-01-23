<template>
   <div class="unlock-ultimate-slaon">
            <div>
                <div class="text-content">
                    <h2 class="primary-title">
                        Unlock the Ultimate Salon Experience with Our 30-Day Free Trial and Earn Exclusive Rewards !!!
                    </h2>
                    <p class="text">Are you ready to elevate your salon business to new heights? Step into the future of beauty and efficiency with our cutting-edge salon software. We're thrilled to offer you an exclusive 30-day free trial packed with features designed to streamline your operations, enhance client experiences, and boost your bottom line.</p>
                    <button class="btn-primary">Request Demo</button>
                </div>
                <figure class="image-content">
                    <img src="/assets/image/salon.png" alt="">
                </figure>
            </div>
        </div>
</template>
<style scoped>

.container{
    width: 90%;
    margin: auto;
} 

.primary-title{
        font-size: 2rem;
        color: white;
    }
    .text{
        font-size: 1.2rem;
        line-height: 1.5rem;
    }

.unlock-ultimate-slaon{
    background: #202047;
    color: white;
 }
 .unlock-ultimate-slaon > div{
    display: grid; 
    grid-template-columns: 1fr 1fr;
    align-items: center;
    padding-left: 5%;
 }
 .unlock-ultimate-slaon .text-content{
    padding: 1rem 1rem  3rem 0;
    flex: 1;
 }
.unlock-ultimate-slaon .image-content{
    flex: 1;
    height: 100%;
    width:95%;
}
.unlock-ultimate-slaon .image-content img{
    height: 100%;
    width: 100%;
    object-fit: cover;
}
</style>