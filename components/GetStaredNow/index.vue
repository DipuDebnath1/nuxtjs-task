<template>
     <div class="container get-started">
            <h2 class="primary-title">How To Get Started ?</h2>
            <div class="content">
                <div style="border-right: 1px solid #ED2D66;">
                    <figure>
                        <img src="~/assets/image/login.png" alt="">
                    </figure>
                    <div>
                        <h4 class="secondary-title">Explore Features</h4>
                        <span class="number one">2</span>
                        <p class="text">Dive into the features that will transform your salon. Get familiar with the intuitive interface and discover the tools that will make your life easier.</p>
                    </div>
                    <figure>
                        <img src="~/assets/image/rewards.png" alt="">
                    </figure>
                </div>
                <div>
                    <div>
                        <h4 class="secondary-title">Sign Up</h4>
                        <span class="number two">1</span>
                        <p class="text">Visit our website and sign up for the 30-day free trial. It's quick, easy, and requires no commitment.</p>
                    </div>
                    <figure><img src="~/assets/image/feature.png" alt=""></figure>
                    <div>
                        <h4 class="secondary-title">Claim Your Rewards</h4>
                        <span class="number three">3</span>
                        <p class="text">As you explore the software, keep an eye out for notifications guiding you on how to claim your exclusive rewards. We want to make sure you get the most out of your trial!</p>
                    </div>
                </div>
            </div>

        </div>
</template>

<style scoped>
 .primary-title{
        font-size: 2rem;
    }
.secondary-title{
        font-size: 1.5rem;
        font-weight: 600;

    }
    .text{
        font-size: 1.2rem;
        line-height: 1.5rem;
    }
.get-started{
    padding: 3rem 0;
    color: #002478;
} 
.get-started h2{
    text-align: center;
    color: #002478;
} 
.get-started .content{
    padding-top: 2rem;
    display: grid;
    grid-template-columns: 1fr 1fr;
}
.get-started .content > div{
    position: relative;
    display: grid;
    grid-template-rows: 1fr 1fr 1fr;
    align-items: center;
}

.get-started .content > div div{
  width: 50%;
  margin: auto;
}
.get-started .content > div div .number{
  background-color: #ED2D66;
  width: 25px;
  height:25px;
  color: white;
  border-radius: 50%;
  display: flex;
  align-items: center;
  justify-content: center;

}
.get-started .content > div div h4{
  font-size: 1.5rem;
  margin:0;
  /* padding-bottom: 1rem; */
}
.get-started .content > div:nth-of-type(odd){
 text-align: right;
}
.get-started .content img{
    height: auto;
    width: 50%; 
    display: block;
    margin: auto;
}
.get-started .two,
.get-started .three{
    position: absolute;
    left: -14px;
}
.get-started .one{
    position: absolute;
    right: -14px;
}

 </style>