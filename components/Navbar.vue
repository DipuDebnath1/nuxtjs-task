
<template>
    <nav class="container">
        <div class="nav">
                <figure>
                    <img src="~/assets/image/logo.png" />
                </figure>
            <BtnPrimary />
        </div>
        </nav>
</template>

<style>
.container{
    width:90%;
    margin:auto;
}
.nav{
    display:flex;
    align-items:center;
    justify-content:space-between;
    color: #ED2D66;
}
.nav figure img{
    width: 8rem ;
    height: auto;
}
</style>