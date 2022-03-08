<template>
  <head>
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <link href="https://fonts.googleapis.com/css?family=Nunito+Sans:300i,400,700&amp;display=swap" rel="stylesheet">
    <title>NetflixMuniGT</title>
  </head>
  <body>
    <nav class="navbar navbar-light p-0">
      <div class="container-fluid px-5">
        <a class="navbar-brand">NetflixMuni</a>
        <form class="d-flex">
          <select class="form-select mx-4 text-white" aria-label="Default select example">
            <option selected="">English</option>
            <option value="1">Español</option>
          </select>
          <button type="button" class="btn btn-danger top-sign-in" style="">Log in</button>
        </form>
      </div>
    </nav>
    <div class="bg-img">
      <div class="layer">
        <div class="row">
          <div class="col-md-12 text-center">
            <h1>Películas ilimitadas, TV <br>shows y más.</h1>
            <h3>Mira a cuaquier hora. Cancela a cualquier hora.</h3>
            <h5>¿Listo para entrar? Ingresa tu email para empezar o para actualizar tu membresía.</h5>
          </div>
        </div>
        <div class="row w-100">
          <div class="col-md-2 col-1"></div>
          <div class="col-md-8 col-10 p-0 main-search">
            <div class="input-group mb-3">
              <input type="text" class="form-control" placeholder="Email address">
              <span class="input-group-text" id="basic-addon2">Empecemos <i class="bi bi-chevron-right text-white"></i></span>
            </div>
          </div>
          <div class="col-md-2 col-1"></div>
        </div>
      </div>
    </div>
   </body>
</template>

<script>
export default {
  name: 'InicioComponent',
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
:root {
   --bs-red: #83bd3f;
}

#app>nav {
   display:none !important;
}

body {
   padding: 0;
   margin: 0;
   font-family: "Nunito Sans";
}

img {
   max-width: 100%;
}

section {
   border-top: 8px solid #222;
   padding-top: 50px;
   padding-bottom: 40px;
   background-color: #000000;
}

section h2 {
   font-size: 55px;
   color: #fff;
   font-weight: bold;
}

section p {
   font-size: 22px;
   color: #fff;
}

h1 {
   color: #fff;
   font-size: 80px;
}

h3,
h5 {
   color: #fff;
}

.text-common {
   color: #757575;
}

.row {
   margin: 0px;
}

.navbar {
   position: absolute;
   width: 100%;
}

.form-select {
   background-color: #333;
   border: 1px solid #757575;
   color: #757575;
   height: 52px;
}

a.navbar-brand {
   color: #83bd3f !important;
   font-size: 44px;
   font-weight: bold;
}

.top-sign-in[data-v-c549cbd6] {
    height: auto;
    margin-top: 0;
    padding-top: 5px;
    width: 10vw;
    background-color: #83bd3f;
    border-color: transparent;
}

.bg-img {
   background-image: url('@/assets/bg.jpg');
   height: 700px;
}

.layer {
   background-color: rgba(3, 13, 158, 0.288);
   display: flex;
   align-items: center;
   justify-content: center;
   flex-direction: column;
   width: 100%;
   height: 100%;
}

.top-sign-in {
   height: 34px;
   margin-top: 10px;
   padding-top: 5px;
}

.input-group-text {
   font-size: 28px;
   background-color: #83bd3f;
   color: #fff;
   border: 0px;
   cursor: pointer;
}

.btn-check:focus+.btn,
.btn:focus {
   box-shadow: none;
}

.main-search input {
   height: 70px;
}

.faq .btn {
   width: 100%;
   height: 72px;
   background-color: #303030;
   font-size: 30px;
   padding-top: 12px;
   text-align: left;
   padding-left: 30px;
   margin-bottom: 10px;
   border-radius: 0px;
}

.multi-collapse.show {
   margin-bottom: 10px;
}

.faq .card {
   background-color: #303030;
   font-size: 26px;
   color: #fff;
   padding-left: 30px;
}

footer {
   background-color: #000000;
   padding-top: 40px;
   border-top: 8px solid #222;
}

footer ul {
   list-style-type: none;
}

footer ul li {
   color: #757575;
   margin-bottom: 15px;
}

footer a {
   text-decoration: none;
   color: #757575;
}

footer a:hover {
   color: #757575;
   text-decoration: underline;
}

@media(min-width: 1200px) {
   .main-search .input-group {
      width: 60%;
      margin: 0 auto;
   }
}

@media(max-width: 800px) {
   .layer h1 {
      font-size: 60px;
   }
}

@media(max-width: 768px) {
   .reverse {
      flex-direction: column-reverse;
   }
}

@media(max-width: 612px) {
   .layer h1 {
      font-size: 50px;
   }
   .layer h5 {
      font-size: 20px;
   }
   section h2 {
      font-size: 40px;
   }
   .main-search input,
   .input-group-text {
      width: 100% !important;
      border-radius: 0px;
      border: 0px;
   }
   .input-group-text {
      margin-top: 5px;
   }
   .faq .btn {
      font-size: 20px;
      height: auto;
      padding-top: 5px;
      padding-left: 10px;
   }
   .faq .card {
      font-size: 16px;
      padding-left: 10px;
   }
   section p {
      font-size: 18px;
   }
}

@media(max-width: 515px) {
   .layer h1 {
      font-size: 40px;
   }
   .layer h5 {
      font-size: 16px;
   }
   .bottom-search p {
      padding-left: 10px;
      padding-right: 10px;
   }
   a.navbar-brand {
      font-size: 32px;
   }
   .form-select {
      height: 40px;
   }
   .top-sign-in {
      margin-top: 3px;
   }
   .px-5 {
      padding-right: 10px!important;
      padding-left: 10px!important;
   }
   .layer h3 {
      font-size: 20px;
   }
   .layer h5 {
      font-size: 14px;
   }
}

@media(max-width:425px) {
   .layer h1 {
      font-size: 34px;
   }
}
</style>
