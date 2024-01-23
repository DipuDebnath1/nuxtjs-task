<template>  
<div>  
    <div class="download-section">
        <div class="container">
            <div class="text-content">
                <h2 class="primary-title">Download the App</h2>
                <p class="text">Manage your appointments with Salonnz’s top-rated app</p>
                <button class="btn-primary">Book a Demo</button>
                <p class="text appLink">
                    <span><i class="fa-brands fa-apple"></i> App Store</span>
                    <span><i class="fa-brands fa-google-play"></i>Google Play</span>
                </p>
            </div>
            <div class="image-content">
                <figure>
                    <img  src="~/assets/image/duble-miboile.png " alt="">
                </figure>
            </div>

        </div>
     </div>
</div>
</template>

<style scoped>

.primary-title{
        font-size: 2rem;
        color: white;
    }
    .text{
        font-size: 1.2rem;
        line-height: 1.5rem;
    }
.download-section{
    background-color: #202047;
    margin-top: 2rem;
}
.download-section .container{
    display: grid;
    grid-template-columns: 1fr 1fr;
    align-items: center;
    color: white;
}
.download-section .text-content{
    padding: 2rem 0;
}
.download-section .text-content button{
    margin: 1rem 0;
}
.appLink{
    display:flex;
    gap:1rem;
}
.download-section .text-content p span{
    border: 1px solid white;
    width: 8rem;
    text-align: center;
    padding: 10px 0;
    border-radius: 3px;
}
.download-section .image-content figure img{
    width: 60%;
    display: block;
    position: relative;
    margin-top: -3.5rem;
    margin-bottom: -3.5rem;

}

</style>

<script>
export default {
    
}
</script>