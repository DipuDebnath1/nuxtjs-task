<template>
 <div  class="container carousel-container" id="carousel-container">
         <div class="carousel-item">
            <div class="carousel-img">
                <img src="~/assets/image/carousel1.png" alt="">
                <svg xmlns="http://www.w3.org/2000/svg" width="400" height="400" viewBox="0 0 519 515" fill="none">
                    <path opacity="0.5" fill-rule="evenodd" clip-rule="evenodd" d="M259.5 0C402.818 0 519 115.287 519 257.5C519 399.713 402.818 515 259.5 515C116.182 515 0 399.713 0 257.5C0 115.287 116.182 0 259.5 0Z" fill="#ED2D66"/>
                  </svg>
            </div>
            <div class="carousel-text">
                <h2 class="primary">Streamlined Salon Management:</h2>
                <p class="text">Effortlessly manage appointments, staff schedules, and customer information all in one place. Say goodbye to paperwork and hello to efficiency.</p>
            </div>
         </div>
         <div class="carousel-item">
            <div class="carousel-img">
                <svg xmlns="http://www.w3.org/2000/svg" width="400" height="400" viewBox="0 0 519 515" fill="none">
                    <path opacity="0.5" fill-rule="evenodd" clip-rule="evenodd" d="M259.5 0C402.818 0 519 115.287 519 257.5C519 399.713 402.818 515 259.5 515C116.182 515 0 399.713 0 257.5C0 115.287 116.182 0 259.5 0Z" fill="#ED2D66"/>
                  </svg>
                <img src="~/assets/image/carousel2.png" alt="">
            </div>
            <div class="carousel-text">
                <h2 class="primary">Intuitive Interface:</h2>
                <p class="text">Our user-friendly interface makes navigating the software a breeze. No steep learning curves—just a seamless experience for you and your team.</p>
            </div>
         </div>
         <div class="carousel-item">
            <div class="carousel-img">
                <svg xmlns="http://www.w3.org/2000/svg" width="400" height="400" viewBox="0 0 519 515" fill="none">
                    <path opacity="0.5" fill-rule="evenodd" clip-rule="evenodd" d="M259.5 0C402.818 0 519 115.287 519 257.5C519 399.713 402.818 515 259.5 515C116.182 515 0 399.713 0 257.5C0 115.287 116.182 0 259.5 0Z" fill="#ED2D66"/>
                  </svg>
                <img src="~/assets/image/carousel3.png" alt="">
            </div>
            <div class="carousel-text">
                <h2 class="primary">Powerful Features:</h2>
                <p class="text">From appointment booking and inventory management to marketing tools, our software offers a comprehensive suite of features tailored to salon needs.</p>
            </div>
         </div>
         <div>
            <span id="arrow-left" class="carousel-prev"><</span>
            <span id="arrow-right" class="carousel-next">></span>
         </div>
        </div>
        <div class="slider-buttons">
            <i onclick="slideLeftbtn()" class="fa-solid fa-arrow-left"></i>
                <i class="handleSliderID" onclick="handleSliderID(0)">o</i>
                <i class="handleSliderID" onclick="handleSliderID(1)">o</i>
                <i class="handleSliderID" onclick="handleSliderID(2)">o</i>
            <i onclick="slideRightbtn()" class="fa-solid fa-arrow-right"></i>
        </div>
</template>

<style scoped>

.primary-title{
        font-size: 2rem;
        color: white;
    }
.secondary-title{
        font-size: 1.5rem;
        color: white;
        font-weight: 600;

    }
    .text{
        font-size: 1.2rem;
        line-height: 1.5rem;
    }
.carousel-container{
    position: relative;
    /* height: 50vh; */
}
.carousel-item{
    width: 90%;
    margin: auto;
    align-items: center;
    color: #002478;
    display: flex;
}
.carousel-item > .carousel-img{
    flex-basis: 55%;
    padding: 3rem 0;
    margin-top: 1rem;
    position: relative;
    display: flex ;
    justify-content: center;
    align-items: center;
    }
.carousel-item > .carousel-img img{
    width: 100%;
    position: absolute;

}
.carousel-item > .carousel-text{
flex-basis: 45%;
}
.carousel-prev,
.carousel-next{
    position: absolute;
    font-size: 2rem;
    padding: 0 1rem;
    border-radius: 50%;
    top: 45%;
    color: gray;
    border: 1px solid ;
    transition: .3s all ease;
}
.carousel-next{
   right: 0;
}
.carousel-prev:hover,
.carousel-next:hover{
    background-color: #202047;
}

.slider-buttons{
    width: 200px;
    margin: auto;
    padding: 1rem 0;
    color: gray;
    display: flex;
    align-items: center;
    gap: 10px;
}
.slider-buttons-active{
    padding: 1px 5px;
    border:1px solid gray;
    border-radius: 50%;
}
</style>

<script>
export default {
    mounted() {
    
//****carousel slide start here *** */ 
let carouselItem = document.querySelectorAll(".carousel-item"),
	arrowLeft = document.querySelector("#arrow-left"),
	arrowRight = document.querySelector("#arrow-right"),
	slidersID = document.querySelectorAll('.handleSliderID'),
    current = 0;

// Clear all images
function reset() {
	for (let i = 0; i < carouselItem.length; i++) {
		carouselItem[i].style.display = "none";
	}
}

function startSlide() {
	reset();
	carouselItem[0].style.display = "flex";
}

// Show previous
function slideLeft() {
	reset();
	carouselItem[current - 1].style.display = "flex";
	current--;
}

// Show next
function slideRight() {
	reset();
	carouselItem[current + 1].style.display = "flex";
	current++;
}

// Left arrow click
arrowLeft.addEventListener("click", function () {
	if (current === 0) {
		current = carouselItem.length;
	}
	slideLeft();
});

// Right arrow click
arrowRight.addEventListener("click", function () {
	if (current === carouselItem.length - 1) {
		current = -1;
	}
	slideRight();
});

// slider bottom handle buttons 
const slideLeftbtn =()=>{
	if (current === 0) {
		current = carouselItem.length;
	}
	slideLeft();
}
const slideRightbtn =()=>{
	if (current === carouselItem.length - 1) {
		current = -1;
	}
	slideRight();
}

startSlide();

    },
}
</script>