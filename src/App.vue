<template>
  <div>
        <!-- navbar -->
        <nav class="navbar fixed-top navbar-expand-lg">
      <div class="container">
        <a class="navbar-brand" href="#">
          <img src="@/assets/logo.svg" alt="Logo" width="120" height="96" class="d-inline-block align-text-top">
        </a>
        <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav" aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
          <span class="navbar-toggler-icon"></span>
        </button>
        <div class="collapse navbar-collapse" id="navbarNav">
          <ul class="navbar-nav ms-auto">
            <li class="nav-item">
              <a class="nav-link" href="#home">Home</a>
            </li>
            <li class="nav-item">
              <a class="nav-link ms-4" href="#menu">Order</a>
            </li>
            <li class="nav-item">
              <a class="nav-link ms-4" href="#testimoni">About</a>
            </li>
            <li class="nav-item">
              <a class="nav-link ms-4" href="#testimoni">Blog</a>
            </li>
            <li class="nav-item">
              <a class="nav-link ms-4" href="#testimoni">Contact Us</a>
            </li>
          </ul>
        </div>
      </div>
      <button type="button" class="btn btn-warning">Register</button>
    </nav>
    <!-- end navbar -->

    <!-- hero -->
    <section class="hero" id="hero">
      <div class="card rounded-0 bg-dark text-white">
        <img src="@/assets/hero.png" class="card-img" alt="hero image">
        <div class="card-img-overlay text-center">
          <h1 class="card-title">Pizza Food</h1>
        </div>
      </div>
    </section>
    <!-- end hero -->

    <!-- menu -->
    <section class="menu py-5" id="menu">
      <div class="container">
        <h2 class="section-title text-center h3">Choose your pizza</h2>
        <div class="row justify-content-center gy-3">

          <div class="card mb-3" style="max-width: 540px;">
            <div class="row g-0">
              <div class="col-md-4">
                <img src="@/assets/pizza/Cheese Pizza.png" class="img-fluid rounded-start" alt="...">
              </div>
              <div class="col-md-8">
                <div class="card-body">
                  <h5 class="card-title">Cheese Pizza</h5>
                  <p class="card-text">$8.00</p>
                </div>
              </div>
            </div>
          </div>
          <div class="card mb-3" style="max-width: 540px;">
            <div class="row g-0">
              <div class="col-md-4">
                <img src="@/assets/pizza/Veggie Pizza.png" class="img-fluid rounded-start" alt="...">
              </div>
              <div class="col-md-8">
                <div class="card-body">
                  <h5 class="card-title">Veggie Pizza</h5>
                  <p class="card-text">$8.50</p>
                  <p class="card-text">$10.00</p>
                </div>
              </div>
            </div>
          </div>
          <div class="card mb-3" style="max-width: 540px;">
            <div class="row g-0">
              <div class="col-md-4">
                <img src="@/assets/pizza/Classical Pizza.png" class="img-fluid rounded-start" alt="...">
              </div>
              <div class="col-md-8">
                <div class="card-body">
                  <h5 class="card-title">Clasiccal Pizza</h5>
                  <p class="card-text">$12.00</p>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </section>
    <!-- end menu -->

    <!-- custom pizza -->
    <section class="menu py-5" id="menu">
      <div class="container">
        <h1 class="section-title text-left h3">Custom Pizza</h1>
        <div class="row justify-content-left gy-3">
          <div class="form-check">
            <input class="form-check-input" type="radio" name="flexRadioDefault" id="flexRadioDefault1" checked>
            <label class="form-check-label" for="flexRadioDefault1">
              Small
            </label>
          </div>
          <div class="form-check">
            <input class="form-check-input" type="radio" name="flexRadioDefault" id="flexRadioDefault2">
            <label class="form-check-label" for="flexRadioDefault2">
              Medium (+5$)
            </label>
          </div>
          <div class="form-check">
            <input class="form-check-input" type="radio" name="flexRadioDefault" id="flexRadioDefault3">
            <label class="form-check-label" for="flexRadioDefault3">
              Large (+7$)
            </label>
          </div>
        </div>
      </div>
      <div class="container">
        <h1 class="section-title text-left h3">Toppings</h1>
        <div class="row justify-content-left">
      <div class="row">
          <button type="button" class="btn btn-outline-secondary" checked>Avocado</button>
          <button type="button" class="btn btn-outline-secondary">Brocoli</button>
          <button type="button" class="btn btn-outline-secondary">Onions</button>
          <button type="button" class="btn btn-outline-secondary">Zucchini</button>
          <button type="button" class="btn btn-outline-secondary">Lobster</button>
          <button type="button" class="btn btn-outline-secondary">Oyster</button>
        </div>
        </div>
        <div class="row">
          <button type="button" class="btn btn-outline-secondary" checked>Salmon</button>
          <button type="button" class="btn btn-outline-secondary">Tuna</button>
          <button type="button" class="btn btn-outline-secondary">Bacon</button>
          <button type="button" class="btn btn-outline-secondary">Duck</button>
          <button type="button" class="btn btn-outline-secondary">Ham</button>
          <button type="button" class="btn btn-outline-secondary">Sausage</button>
        </div>
      </div>
    </section>
    <!-- end custom pizza -->
<!-- Footer -->
<footer
          class="text-center text-lg-start text-white"
          style="background-color: #1c2331"
          >
    <!-- Section: Social media -->
    <section
             class="d-flex justify-content-between p-4"
             style="background-color: #6351ce"
             >
      <!-- Left -->
      <div class="me-5">
        <span>Get connected with us on social networks:</span>
      </div>
      <!-- Left -->

      <!-- Right -->
      <div>
        <a href="" class="text-white me-4">
          <i class="fab fa-facebook-f"></i>
        </a>
        <a href="" class="text-white me-4">
          <i class="fab fa-twitter"></i>
        </a>
        <a href="" class="text-white me-4">
          <i class="fab fa-google"></i>
        </a>
        <a href="" class="text-white me-4">
          <i class="fab fa-instagram"></i>
        </a>
        <a href="" class="text-white me-4">
          <i class="fab fa-linkedin"></i>
        </a>
        <a href="" class="text-white me-4">
          <i class="fab fa-github"></i>
        </a>
      </div>
      <!-- Right -->
    </section>
    <!-- Section: Social media -->

    <!-- Section: Links  -->
    <section class="">
      <div class="container text-center text-md-start mt-5">
        <!-- Grid row -->
        <div class="row mt-3">
          <!-- Grid column -->
          <div class="col-md-3 col-lg-4 col-xl-3 mx-auto mb-4">
            <!-- Content -->
            <h6 class="text-uppercase fw-bold">Company name</h6>
            <hr
                class="mb-4 mt-0 d-inline-block mx-auto"
                style="width: 60px; background-color: #7c4dff; height: 2px"
                />
            <p>
              Here you can use rows and columns to organize your footer
              content. Lorem ipsum dolor sit amet, consectetur adipisicing
              elit.
            </p>
          </div>
          <!-- Grid column -->

          <!-- Grid column -->
          <div class="col-md-2 col-lg-2 col-xl-2 mx-auto mb-4">
            <!-- Links -->
            <h6 class="text-uppercase fw-bold">Products</h6>
            <hr
                class="mb-4 mt-0 d-inline-block mx-auto"
                style="width: 60px; background-color: #7c4dff; height: 2px"
                />
            <p>
              <a href="#!" class="text-white">MDBootstrap</a>
            </p>
            <p>
              <a href="#!" class="text-white">MDWordPress</a>
            </p>
            <p>
              <a href="#!" class="text-white">BrandFlow</a>
            </p>
            <p>
              <a href="#!" class="text-white">Bootstrap Angular</a>
            </p>
          </div>
          <!-- Grid column -->

          <!-- Grid column -->
          <div class="col-md-3 col-lg-2 col-xl-2 mx-auto mb-4">
            <!-- Links -->
            <h6 class="text-uppercase fw-bold">Useful links</h6>
            <hr
                class="mb-4 mt-0 d-inline-block mx-auto"
                style="width: 60px; background-color: #7c4dff; height: 2px"
                />
            <p>
              <a href="#!" class="text-white">Your Account</a>
            </p>
            <p>
              <a href="#!" class="text-white">Become an Affiliate</a>
            </p>
            <p>
              <a href="#!" class="text-white">Shipping Rates</a>
            </p>
            <p>
              <a href="#!" class="text-white">Help</a>
            </p>
          </div>
          <!-- Grid column -->

          <!-- Grid column -->
          <div class="col-md-4 col-lg-3 col-xl-3 mx-auto mb-md-0 mb-4">
            <!-- Links -->
            <h6 class="text-uppercase fw-bold">Contact</h6>
            <hr
                class="mb-4 mt-0 d-inline-block mx-auto"
                style="width: 60px; background-color: #7c4dff; height: 2px"
                />
            <p><i class="fas fa-home mr-3"></i> New York, NY 10012, US</p>
            <p><i class="fas fa-envelope mr-3"></i> info@example.com</p>
            <p><i class="fas fa-phone mr-3"></i> + 01 234 567 88</p>
            <p><i class="fas fa-print mr-3"></i> + 01 234 567 89</p>
          </div>
          <!-- Grid column -->
        </div>
        <!-- Grid row -->
      </div>
    </section>
    <!-- Section: Links  -->

    <!-- Copyright -->
    <div
         class="text-center p-3"
         style="background-color: rgba(0, 0, 0, 0.2)"
         >
      © 2020 Copyright Foodnow. All Rights Reserved. Powered by Pt. TImedoor Indonesia | Privacy Policy
      <a class="text-white" href="https://mdbootstrap.com/"
         >This sites is protected by reCAPTCHA and the Google Privacy Policy and Terms of Service apply</a
        >
    </div>
    <!-- Copyright -->
  </footer>
  <!-- Footer -->
    </div>
</template>


<script>
import HelloWorld from './components/HelloWorld.vue'

export default {
  name: 'app',
  components: {
    HelloWorld
  },
  data() {
    return {
      items: [
          { isActive: true, age: 40, first_name: 'Dickerson', last_name: 'Macdonald' },
          { isActive: false, age: 21, first_name: 'Larsen', last_name: 'Shaw' },
          { isActive: false, age: 89, first_name: 'Geneva', last_name: 'Wilson' },
          { isActive: true, age: 38, first_name: 'Jami', last_name: 'Carney' }
        ],
      showDismissibleAlert: false,
      form: {
        email: '',
        password: '',
        food: null,
        checked: []
      },
      foods: [
        { text: 'Select One', value: null },
        'Carrots', 'Beans', 'Tomatoes', 'Corn'
      ],
      show: true
    }
  },
  methods: {
    handleClick() {
      this.showDismissibleAlert = true
    },
    onSubmit (evt) {
      evt.preventDefault();
      alert(JSON.stringify(this.form));
    },
    onReset (evt) {
      evt.preventDefault();
      /* Reset our form values */
      this.form.email = '';
      this.form.password = '';
      this.form.food = null;
      this.form.checked = [];
      /* Trick to reset/clear native browser form validation state */
      this.show = false;
      this.$nextTick(() => { this.show = true });
    }
  }
}
</script>

<style>
  @import url('https://fonts.googleapis.com/css?family=Lato:400,700');

  body {
    background: #F8F8F6 !important;
    font-family: 'Lato', sans-serif !important;
  }

  .nav-background {
    background: #353535;
  }
</style>
