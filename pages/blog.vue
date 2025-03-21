<script setup>
import { ref } from "vue";

const tabs = ref([
    "All",
    "Latest News",
    "Tips and Advice",
    "Market Intel",
    "Rental",
    "Trends",
    "Fix and Flip",
    "Construction",
]);

const activeTab = ref("All");
</script>
<template>
    <section class="from-the-blog-section">
        <div class="responsive-container">
            <h1 class="blog-heading">BLOG</h1>
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
    <section class="newsletter-section">
        <div class="responsive-container">
            <div class="newsletter-wrapper">
                <h4 class="newsletter-heading pb-3">STAY UP TO DATE</h4>
                <p class="newsletter-heading newsletter-content">Subscribe to receive our monthly newsletter with the latest news </p>
                <form>
                    <div class="row g-2">
                        <div class="col-md-4">
                            <input type="text" class="form-control investor-input-text" placeholder="Name">
                        </div>
                        <div class="col-md-4">
                            <input type="email" class="form-control investor-input-text" placeholder="Email">
                        </div>
                        <div class="col-md-4">
                            <select class="form-select investor-input-text">
                                <option selected>I'm a real estate investor</option>
                            </select>
                        </div>
                    </div>
                    <p class="newsletter-paragraph newsletter-content">
                        By clicking the "Submit" button below, I expressly consent for Anchor Loans to contact me for
                        marketing/promotional purposes– including via SMS text messages and calls made using an
                        automatic telephone dialing system - related to the mortgage products or services I am inquiring
                        about at the number I provided above. My consent to receive marketing/promotional communications
                        is not required to obtain any good or service. I consent to Anchor Loans contacting me by mail,
                        telephone or email in connection with my request even if my telephone number or email address
                        appears on a State or National Do Not Call Registry, or any other Do Not Contact List/Do Not
                        Email List. Message frequency varies. Message and data rates may apply.
                    </p>
                    <button class="common-button newsletter-submit-button">SUBMIT</button>
                </form>
            </div>

        </div>
    </section>
    <section class="blog-buttons">
        <div class="responsive-container">
            <div class="position-relative w-100">
                <div class="d-flex overflow-x-auto custom-scrollbar blog-button-wrapper">
                    <button
                        v-for="tab in tabs"
                        :key="tab"
                        @click="activeTab = tab"
                        class="common-button blog-btn"
                        :class="{ 'active-tab': activeTab === tab }"
                    >
                        {{ tab }}
                    </button>
                </div>
            </div>

        </div>
    </section>
    <section class="from-the-blog-section">
        <div class="responsive-container">
            <div class="blog-card-wrapper d-flex align-items-center justify-content-center gap-4 flex-wrap pt-0">
                <div class="blog-card">
                    <img src="~/assets/images/from-blog-image-1.png" alt="Blog Image" class="card-image">
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
                    <img src="~/assets/images/from-blog-image-2.png" alt="Blog Image" class="card-image">
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
                    <img src="~/assets/images/blog-image-2.png" alt="Blog Image" class="card-image">
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
                    <img src="~/assets/images/from-blog-image-3.png" alt="Blog Image" class="card-image">
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
                    <img src="~/assets/images/blog-image-4.png" alt="Blog Image" class="card-image">
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
                    <img src="~/assets/images/blog-image-5.png" alt="Blog Image" class="card-image">
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
            </div>
        </div>
    </section>
</template>

<style scoped>

</style>