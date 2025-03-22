<script setup>
import {ref, onMounted} from "vue";
import Swiper from "swiper";
import "swiper/css";
import "swiper/css/pagination";
import {Pagination} from "swiper/modules";

const swiperContainer = ref(null);

onMounted(() => {
    if (swiperContainer.value) {
        new Swiper(swiperContainer.value, {
            modules: [Pagination],
            slidesPerView: 1,
            spaceBetween: 25,
            grabCursor: true,
            pagination: {
                el: ".swiper-pagination",
                clickable: true,
            },
            loop: true,
        });
    }
});

</script>


<template>
    <section class="real-estate-section">
        <div class="responsive-container">
            <div class="real-estate-wrapper">
                <div class="real-estate-content">
                    <h1 class="common-heading">REAL ESTATE LENDING PROGRAMS FOR YOUR BUSINESS</h1>
                    <p class="common-paragraph">With over 25 years of real estate finance experience, we provide
                        creative funding for property or development projects. Our flexible lending capacity helps us
                        overcome transaction hurdles easily.
                    </p>
                    <p class="common-paragraph p-0">You know what you’re looking for.</p>
                    <p class="common-paragraph pb-4 p-0">We know how to get you there.</p>
                    <div class="real-estate--button-wrapper d-flex align-items-center gap-4">
                        <button class="common-button real-estate-button">
                            I’M A BROKER
                        </button>
                        <button class="common-button real-estate-button">
                            I’M A BORROWER
                        </button>
                    </div>
                </div>
                <div class="real-estate-image">
                    <img src="~/assets/images/real-estate-image.png" class="img-fluid" alt="real-estate-image">
                </div>
            </div>
        </div>

    </section>
    <section class="everpeak-categories-section">
        <div class="responsive-container">
            <div class="everpeak-categories-wrapper d-flex  justify-content-center gap-4">
                <div class="four-categories-cards">
                    <div class="speed-category-card">
                        <img src="~/assets/images/speed-image.png" class="img-fluid speed-image" alt="speed-image">
                        <h2 class="card-heading">Speed</h2>
                    </div>
                    <div class="flexibility-category-card">
                        <img src="~/assets/images/flexibility-image.png" class="img-fluid" alt="flexibility-image">
                        <h2 class="card-heading">FLEXIBILITY</h2>
                    </div>
                    <div class="trust-category-card">
                        <img src="~/assets/images/trust-image.png" class="img-fluid" alt="trust-image">
                        <h2 class="card-heading">TRUST</h2>
                    </div>
                    <div class="custom-category-card">
                        <img src="~/assets/images/custom-image.png" class="img-fluid" alt="custom-image">
                        <h2 class="card-heading">CUSTOM</h2>
                    </div>
                </div>
                <div class="speed-content">
                    <h1 class="common-heading">SPEED</h1>
                    <p class="common-paragraph pt-0">Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed arcu
                        leo,
                        vehicula ac ex eu, fermentum pharetra orci. Nunc semper, ligula eget placerat sollicitudin,
                        felis lacus accumsan dui, eget rhoncus massa nulla in dolor. Sed tempor maximus neque, et
                        facilisis enim bibendum sed.
                    </p>
                    <p class="common-paragraph">Maecenas vulputate arcu eu eros cursus ultrices. Aliquam tincidunt
                        finibus consequat. Curabitur facilisis mauris nec ligula ullamcorper varius. Suspendisse id
                        condimentum quam. Maecenas sodales semper maximus.
                    </p>
                </div>
            </div>
        </div>
    </section>
    <section class="lending-criteria-section">
        <div class="responsive-container">
            <div class="lending-criteria-wrapper">
                <div class="lending-criteria-content real-estate-content">
                    <h1 class="common-heading text-white">LENDING CRITERIA</h1>
                    <p class="common-paragraph text-white">Our team delivers rapid, adaptable solutions with unmatched
                        reliability, ensuring you can trust us to meet your needs efficiently and effectively in any
                        situation. We prioritize exceptional service and satisfaction, providing solutions that are both
                        timely and dependable.
                    </p>
                    <div class="d-flex align-items-center gap-4 pt-3">
                        <button class="common-button lending-criteria-button real-estate-button">
                            I’M A BROKER
                        </button>
                        <button class="common-button lending-criteria-button real-estate-button">
                            I’M A BORROWER
                        </button>
                    </div>

                </div>
            </div>
        </div>
    </section>
    <section class="from-the-blog-section">
        <div class="responsive-container">
            <h1 class="blog-heading">FROM THE BLOG</h1>
            <div class="blog-card-wrapper d-flex align-items-center justify-content-center gap-4 flex-wrap">
                <div class="blog-card">
                    <img src="~/assets/images/blog-image-1.png" alt="Blog Image" class="card-image">
                    <div class="blog-card-content">
                        <div class="card-content d-flex align-items-center justify-content-between">
                            <p class="featured-label">FEATURED PROJECT</p>
                            <span class="author-date">Author’s Name - DD/MM/YYYY</span>
                        </div>
                        <h2 class="blog-title card-heading p-0">BLOG’S TITLE GOES HERE IN ONE OR TWO LINES IF
                            NEEDED
                        </h2>
                        <a class="navbar-link" href="#">Read more</a>
                    </div>
                </div>

                <div class="blog-card">
                    <img src="~/assets/images/blog-image-2.png" alt="Blog Image" class="card-image">
                    <div class="blog-card-content">
                        <div class="card-content d-flex align-items-center justify-content-between">
                            <p class="featured-label">LATEST NEWS</p>
                            <span class="author-date">Author’s Name - DD/MM/YYYY</span>
                        </div>
                        <h2 class="blog-title card-heading p-0">BLOG’S TITLE GOES HERE IN ONE OR TWO LINES IF
                            NEEDED
                        </h2>
                        <a class="navbar-link" href="#">Read more</a>
                    </div>
                </div>
                <div class="blog-card">
                    <img src="~/assets/images/blog-image-3.png" alt="Blog Image" class="card-image">
                    <div class="blog-card-content">
                        <div class="card-content d-flex align-items-center justify-content-between">
                            <p class="featured-label">FEATURED PROJECT</p>
                            <span class="author-date">Author’s Name - DD/MM/YYYY</span>
                        </div>
                        <h2 class="blog-title card-heading p-0">BLOG’S TITLE GOES HERE IN ONE OR TWO LINES IF
                            NEEDED
                        </h2>
                        <a class="navbar-link" href="#">Read more</a>
                    </div>
                </div>
            </div>
        </div>
    </section>
    <section class="why-choose-everpeak">
        <div class="responsive-container">
            <div class="why-choose-everpeak-wrapper d-flex justify-content-between">
                <div class="why-choose-everpeak-content">
                    <div class="why-choose-everpeak-heading d-flex align-items-center gap-2">
                        <h1 class="common-heading p-0">BUT... WHY CHOOSING</h1>
                        <img src="~/assets/images/ever-peak-image.png" alt="ever-peak-image.png">
                    </div>
                    <p class="common-paragraph p-0">We simplify the Loan process into 4 simple steps:</p>
                    <div class="why-choose-everpeak-points">
                        <div class="why-choose-everpeak-points-content">
                            <h3 class="points-no card-heading p-0 m-0">1</h3>
                            <h4 class="points-title m-0">SUBMIT PRE-QUAL</h4>
                        </div>
                        <p class="common-paragraph p-0">Fill out the form below to get started. We'll be in touch with
                            you
                            shortly!
                        </p>
                    </div>
                    <div class="why-choose-everpeak-points">
                        <div class="why-choose-everpeak-points-content">
                            <h3 class="points-no card-heading p-0 m-0">2</h3>
                            <h4 class="points-title m-0">Complete Quick Application Form</h4>
                        </div>
                        <p class="common-paragraph p-0">Fill out this quick application form, and we'll contact you
                            shortly.
                        </p>
                    </div>
                    <div class="why-choose-everpeak-points">
                        <div class="why-choose-everpeak-points-content">
                            <h3 class="points-no card-heading p-0 m-0">3</h3>
                            <h4 class="points-title m-0">Schedule Call with Loan Origination Team</h4>
                        </div>
                        <p class="common-paragraph p-0">Schedule a call with our loan origination team for personalized
                            assistance.</p>
                    </div>
                    <div class="why-choose-everpeak-points">
                        <div class="why-choose-everpeak-points-content">
                            <h3 class="points-no card-heading p-0 m-0">4</h3>
                            <h4 class="points-title m-0">Complete Financing</h4>
                        </div>
                        <p class="common-paragraph p-0">Complete your financing with our straightforward and efficient
                            application process.</p>
                    </div>
                    <button class="common-button get-started-button">GET STARTED</button>
                </div>
                <div class="why-choose-everpeak-image">
                    <img class="img-fluid" src="~/assets/images/why-choos-everpeak-image.png" alt="why-choose-everpeak-image">
                </div>
            </div>
        </div>
    </section>
    <section class="our-private-investment">
        <div class="responsive-container">
            <h1 class="blog-heading">SEE THE REAL-WORLD IMPACT OF</h1>
            <h1 class="blog-heading">OUR PRIVATE INVESTMENT PROPERTY LOANS</h1>
            <div class="blog-card-wrapper swiper" ref="swiperContainer">
                <div class="swiper-wrapper">
                    <div class="blog-card our-private-investment-card swiper-slide">
                        <img src="~/assets/images/our-private-investment-1.png" alt="Blog Image" class="card-image">
                        <div class="our-private-investment-card-content p-4">
                            <div class="info">
                                <div class="label">Loan Amount</div>
                                <div class="value">$3.4M</div>
                            </div>
                            <div class="info">
                                <div class="label">Closing Time</div>
                                <div class="value">9 Days</div>
                            </div>
                            <div class="info">
                                <div class="label">Loan Type</div>
                                <div class="value">Construction Loan</div>
                            </div>
                            <div class="info">
                                <div class="label">Location</div>
                                <div class="value">Rockaway, NJ</div>
                            </div>
                        </div>
                    </div>
                    <div class="blog-card our-private-investment-card swiper-slide">
                        <img src="~/assets/images/our-private-investment-2.png" alt="Blog Image" class="card-image">
                        <div class="our-private-investment-card-content p-4">
                            <div class="info">
                                <div class="label">Loan Amount</div>
                                <div class="value">$3.4M</div>
                            </div>
                            <div class="info">
                                <div class="label">Closing Time</div>
                                <div class="value">9 Days</div>
                            </div>
                            <div class="info">
                                <div class="label">Loan Type</div>
                                <div class="value">Construction Loan</div>
                            </div>
                            <div class="info">
                                <div class="label">Location</div>
                                <div class="value">Rockaway, NJ</div>
                            </div>
                        </div>
                    </div>
                    <div class="blog-card our-private-investment-card swiper-slide">
                        <img src="~/assets/images/our-private-investment-3.png" alt="Blog Image" class="card-image">
                        <div class="our-private-investment-card-content p-4">
                            <div class="info">
                                <div class="label">Loan Amount</div>
                                <div class="value">$3.4M</div>
                            </div>
                            <div class="info">
                                <div class="label">Closing Time</div>
                                <div class="value">9 Days</div>
                            </div>
                            <div class="info">
                                <div class="label">Loan Type</div>
                                <div class="value">Construction Loan</div>
                            </div>
                            <div class="info">
                                <div class="label">Location</div>
                                <div class="value">Rockaway, NJ</div>
                            </div>
                        </div>
                    </div>
                </div>
                <div class="swiper-pagination"></div>
            </div>

        </div>
    </section>
    <section id="invest" class="become-an-investor">
        <div class="responsive-container">
            <div class="become-an-investor-wrapper">
                <div class="card p-4 shadow become-an-investor-card">
                    <h2 class="blog-heading pb-3">BECOME AN INVESTOR</h2>
                    <form>
                        <div class="row mb-3 input-wrapper">
                            <div class="col-sm-12 col-md-6">
                                <input type="text" class="form-control investor-input-text"
                                       placeholder="Name (required)" required>
                            </div>
                            <div class="col-sm-12 col-md-6">
                                <input type="text" class="form-control investor-input-text"
                                       placeholder="Last name (required)" required>
                            </div>
                        </div>
                        <div class="row mb-3 input-wrapper">
                            <div class="col-sm-12 col-md-6">
                                <input type="email" class="form-control investor-input-text"
                                       placeholder="Email (required)" required>
                            </div>
                            <div class="col-sm-12 col-md-6">
                                <input type="tel" class="form-control investor-input-text"
                                       placeholder="Phone number (required)" required>
                            </div>
                        </div>
                        <div class="mb-3">
                            <select class="form-select investor-input-text">
                                <option selected>Select a Loan Program</option>
                            </select>
                        </div>
                        <div class="row mb-3">
                            <div class="col-auto">
                                <label class="form-label investor-form-label investor-input-text p-0">Any active deal(s)
                                    that need funding?
                                </label>
                                <div class="radio-check-button-wrapper">
                                    <div class="radio-check-button">
                                        <input type="radio" id="yes" name="funding" class="form-check-input">
                                        <label for="yes"
                                               class="form-check-label investor-form-label investor-input-text p-0 radio-label">Yes</label>
                                    </div>
                                    <div class="radio-check-button">
                                        <input type="radio" id="no" name="funding" class="form-check-input">
                                        <label for="no"
                                               class="form-check-label investor-form-label investor-input-text p-0 radio-label">No</label>
                                    </div>
                                </div>
                            </div>
                            <div class="col">
                                <label class="form-label investor-form-label investor-input-text p-0">Experience (number
                                    of deals sold)</label>
                                <select class="form-select investor-input-text">
                                    <option selected>Beginner (0 to 4 deals)</option>
                                </select>
                            </div>
                        </div>
                        <div class="mb-3">
                            <textarea class="form-control investor-input-text" rows="4"
                                      placeholder="Describe the deal summary"></textarea>
                        </div>
                    </form>
                </div>
            </div>
            <div class="investor-form-button">
                <button class="common-button submit-button">SUBMIT</button>
            </div>
        </div>
    </section>

</template>


<style scoped>
.swiper-wrapper {
    padding: 32px 0 50px 0;
}
.swiper-slide {
    width: 384px !important;
}
</style>