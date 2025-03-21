<script setup>
</script>
<template>
    <section class="apply-and-get">
        <div class="responsive-container">
            <h2 class="blog-heading apply-and-get-heading">Apply and get pre-qualified now</h2>
            <div class="apply-and-get-container d-flex align-items-center justify-content-between gap-4">
                <div class="apply-get-qualified-wrapper card p-4 become-an-investor-card">
                    <div class="mb-3">
                        <label class="form-label investor-form-label investor-input-text p-0">Property/Collateral
                            (required)</label>
                        <select class="form-select investor-input-text">
                            <option>Select a real estate collateral</option>
                        </select>
                    </div>
                    <div class="mb-3">
                        <label class="form-label  investor-form-label investor-input-text p-0">Property
                            Location (required)</label>
                        <select class="form-select investor-input-text">
                            <option>Select one</option>
                        </select>
                    </div>
                    <div class="verify-your-loan-program">
                        <p class="verify-your-loan-program-content">To verify your loan to property value ratio meets
                            our criteria, please provide specific loan and property amounts:
                        </p>
                        <div class="row g-3">
                            <div class="col-md-6">
                                <label class="form-label  investor-form-label investor-input-text p-0">Loan amount
                                    (required)</label>
                                <div class="input-group">
                                    <span class="input-group-text investor-input-text">$</span>
                                    <input type="number" id="loanAmount" class="form-control investor-input-text"
                                           value="0.00">
                                </div>
                            </div>
                            <div class="col-md-6">
                                <label class="form-label  investor-form-label investor-input-text p-0">Property value
                                    (required)</label>
                                <div class="input-group">
                                    <span class="input-group-text investor-input-text">$</span>
                                    <input type="number" id="propertyValue" class="form-control investor-input-text"
                                           value="0.00">
                                </div>
                            </div>
                        </div>
                        <div class="row g-3 align-items-center mt-2">
                            <div class="col-md-6">
                                <div class="ltv-input">
                                    <label class="form-label ltv-label">LTV</label>
                                    <input type="text" id="ltv" class="form-control investor-input-text" value="0.0%"
                                           disabled>
                                </div>
                            </div>
                            <div class="col-md-6">
                                <label class="form-label  investor-form-label investor-input-text p-0">Loan Term
                                    (Required)</label>
                                <select class="form-select investor-input-text">
                                    <option>Select loan term</option>
                                </select>
                            </div>
                        </div>
                    </div>
                    <div class="row mb-3">
                        <div class="col">
                            <input type="text" class="form-control investor-input-text"
                                   placeholder="Name (required)" required>
                        </div>
                        <div class="col">
                            <input type="text" class="form-control investor-input-text"
                                   placeholder="Last name (required)" required>
                        </div>
                    </div>
                    <div class="row mb-3">
                        <div class="col">
                            <input type="email" class="form-control investor-input-text"
                                   placeholder="Email (required)" required>
                        </div>
                        <div class="col">
                            <input type="tel" class="form-control investor-input-text"
                                   placeholder="Phone number (required)" required>
                        </div>
                    </div>
                    <p class="verify-your-loan-program-content submit-content">By submitting this form, you agree to
                        receive recurring automated promotional and
                        personalized marketing text messages (e.g. appointment reminders) from Spectra Lending at the
                        cell number used when signing up. Consent is not a condition of any purchase. Reply HELP for
                        help and STOP to cancel. Msg frequency varies. Msg and data rates may apply.
                        View Terms Privacy Policy.
                    </p>
                    <button class="common-button real-estate-button" style="width: 170px">SUBMIT</button>
                </div>
                <div class="apply-and-get-image-content">
                    <img src="~/assets/images/apply-image.png" alt="apply-image">
                    <p class="apply-and-get-content">Lorem ipsum dolor sit amet, consectetur adipiscing elit. Curabitur id
                        ipsum a eros vehicula eleifend. Lorem ipsum dolor sit amet, consectetur adipiscing elit. In vitae
                        fermentum ex. Sed luctus nibh ut malesuada vulputate. In hac habitasse platea dictumst. Ut faucibus
                        volutpat tortor, vitae tempus libero ullamcorper non. Vivamus in turpis nunc.
                    </p>
                    <div dir="rtl" class="about-contact-wrapper d-flex flex-column gap-3">
                        <p class="about-title contact-title m-0">CONTACT US</p>
                        <p class="about-title contact-title contact-info m-0">+1 (555) 555-5555</p>
                        <p class="about-title contact-title contact-info m-0">info@everpeaklending.com</p>
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>

<style scoped>

</style>