<template>
    <div id="carouselExampleCaptions" class="carousel slide" data-bs-ride="carousel">
        <div class="carousel-indicators home_carousel-indicators carousel-indicators_item">
            <button type="button" data-bs-target="#carouselExampleCaptions" data-bs-slide-to="0" class="active" aria-current="true" aria-label="Slide 1"><div class="carousel-indicator_bg"></div></button>
            <button type="button" data-bs-target="#carouselExampleCaptions" data-bs-slide-to="1" aria-label="Slide 2"></button>
            <button type="button" data-bs-target="#carouselExampleCaptions" data-bs-slide-to="2" aria-label="Slide 3"></button>
        </div>
        <div class="carousel-inner">
            <div class="carousel-item active">
            <img src="../assets/images/slide.png" class="d-block w-100" alt="">
            <div class="carousel-caption d-none d-md-block carousel-caption_fontsize">
                <h5>120 Anastasia Avenue, Coral Gables</h5>
                <p>$625,000</p>
                <button type="button" class="btn btn-outline-dark">MORE INFO</button>
            </div>
            </div>
            <div class="carousel-item">
            <img src="../assets/images/slide2.png" class="d-block w-100" alt="">
            <div class="carousel-caption d-none d-md-block carousel-caption_fontsize">
                <h5>Second slide label</h5>
                <p>Some representative placeholder content for the second slide.</p>
                <button type="button" class="btn btn-outline-dark">MORE INFO</button>
            </div>
            </div>
            <div class="carousel-item">
            <img src="../assets/images/slide.png" class="d-block w-100" alt="">
            <div class="carousel-caption d-none d-md-block carousel-caption_fontsize">
                <h5>Third slide label</h5>
                <p>Some representative placeholder content for the third slide.</p>
                <button type="button" class="btn btn-outline-dark">MORE INFO</button>
            </div>
            </div>
        </div>
        <button class="carousel-control-prev" type="button" data-bs-target="#carouselExampleCaptions" data-bs-slide="prev">
            <span class="carousel-control-prev-icon" aria-hidden="true"></span>
            <span class="visually-hidden">Previous</span>
        </button>
        <button class="carousel-control-next" type="button" data-bs-target="#carouselExampleCaptions" data-bs-slide="next">
            <span class="carousel-control-next-icon" aria-hidden="true"></span>
            <span class="visually-hidden">Next</span>
        </button>
    </div>
</template>


<style scoped lang="scss">
    .home_carousel-indicators {
        bottom: 290px;
    }


    .carousel-indicators_item button {
        width: 17px;
        height: 17px;
        border-radius: 50%;
    }

    .carousel-caption_fontsize h5{
        font-size: 48px;
    }

    .carousel-caption_fontsize p {
        font-size: 36px;
    }

</style>