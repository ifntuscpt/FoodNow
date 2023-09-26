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
      <button type="button" class="btn btn-warning">Warning</button>
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
        <h1 class="section-title text-center h3">Custom Pizza</h1>
        <div class="row justify-content-center gy-3">
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
    </section>
    <!-- end custom pizza -->
    <!-- footer -->
    <footer class="text-center text-white py-3">
      <p class="m-0">Copyright &copy; 2022. Ngoffee</p>
    </footer>
    <!-- end footer -->
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
