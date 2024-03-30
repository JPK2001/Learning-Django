# Step 3: Building the Web page for the App.
Now create a base.html page.
```html
{% load static %}
<html lang="en">
<head>
    <meta charset="utf-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <title>Boreal Management System | Dashboard</title>

    <!-- Font Awesome -->
    <link rel="stylesheet" href="{% static 'fontawesome-free/css/all.min.css' %}">

    <!-- Bootstrap CSS -->
    <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap@5.0.0-beta3/dist/css/bootstrap.min.css" integrity="sha384-eOJMYsd53ii+scO/bJGFsiCZc+5NDVN2yr8+0RDqr0Ql0h+rP48ckxlpbzKgwra6" crossorigin="anonymous">

    <!-- Ionicons -->
    <link rel="stylesheet" href="https://code.ionicframework.com/ionicons/2.0.1/css/ionicons.min.css">

    <!-- Tempusdominus Bbootstrap 4 -->
    <link rel="stylesheet" href="{% static 'tempusdominus-bootstrap-4/css/tempusdominus-bootstrap-4.min.css' %}">

    <!-- iCheck -->
    <link rel="stylesheet" href="{% static 'icheck-bootstrap/icheck-bootstrap.min.css' %}">

    <!-- JQVMap -->
    <link rel="stylesheet" href="{% static 'jqvmap/jqvmap.min.css' %}">

    <!-- Theme style -->
    <link rel="stylesheet" href="{% static 'dist/css/adminlte.min.css' %}">

    <!-- overlayScrollbars -->
    <link rel="stylesheet" href="{% static 'overlayScrollbars/css/OverlayScrollbars.min.css' %}">

    <!-- Daterange picker -->
    <link rel="stylesheet" href="{% static 'daterangepicker/daterangepicker.css' %}">

    <!-- Summernote -->
    <link rel="stylesheet" href="{% static 'summernote/summernote-bs4.css' %}">

    <!-- Google Font: Source Sans Pro -->
    <link href="https://fonts.googleapis.com/css?family=Source+Sans+Pro:300,400,400i,700" rel="stylesheet">
</head>
<body class="hold-transition sidebar-mini layout-fixed">
    {% block content %}
    {% endblock %}

    <!-- jQuery -->
    <script src="https://code.jquery.com/jquery-3.4.1.slim.min.js" integrity="sha384-J6qa4849blE2+poT4WnyKhv5vZF5SrPo0iEjwBvKU7imGFAV0wwj1yYfoRSJoZ+n" crossorigin="anonymous"></script>
    <!-- Bootstrap JS -->
    <script src="https://cdn.jsdelivr.net/npm/popper.js@1.16.0/dist/umd/popper.min.js" integrity="sha384-Q6E9RHvbIyZFJoft+2mJbHaEWldlvI9IOYy5n3zV9zzTtmI3UksdQRVvoxMfooAo" crossorigin="anonymous"></script>
    <script src="https://stackpath.bootstrapcdn.com/bootstrap/4.4.1/js/bootstrap.min.js" integrity="sha384-wfSDF2E50Y2D1uUdj0O3uMBJnjuUD4Ih7YwaYd1iqfktj0Uod8GCExl3Og8ifwB6" crossorigin="anonymous"></script>

    <!-- jQuery UI 1.11.4 -->
    <script src="{% static 'jquery-ui/jquery-ui.min.js' %}"></script>
    <!-- Resolve conflict in jQuery UI tooltip with Bootstrap tooltip -->
    <script>
        $.widget.bridge('uibutton', $.ui.button);
    </script>

    <!-- Bootstrap 4 -->
    <script src="{% static 'bootstrap/js/bootstrap.bundle.min.js' %}"></script>

    <!-- ChartJS -->
    <script src="{% static 'chart.js/Chart.min.js' %}"></script>

    <!-- Sparkline -->
    <script src="{% static 'sparklines/sparkline.js' %}"></script>

    <!-- JQVMap -->
    <script src="{% static 'jqvmap/jquery.vmap.min.js' %}"></script>
    <script src="{% static 'jqvmap/maps/jquery.vmap.usa.js' %}"></script>

    <!-- jQuery Knob Chart -->
    <script src="{% static 'jquery-knob/jquery.knob.min.js' %}"></script>

    <!-- Moment.js -->
    <script src="{% static 'moment/moment.min.js' %}"></script>

    <!-- daterangepicker -->
    <script src="{% static 'daterangepicker/daterangepicker.js' %}"></script>

    <!-- Tempusdominus Bootstrap 4 -->
    <script src="{% static 'tempusdominus-bootstrap-4/js/tempusdominus-bootstrap-4.min.js' %}"></script>

    <!-- Summernote -->
    <script src="{% static 'summernote/summernote-bs4.min.js' %}"></script>

    <!-- overlayScrollbars -->
    <script src="{% static 'overlayScrollbars/js/jquery.overlayScrollbars.min.js' %}"></script>

    <!-- AdminLTE App -->
    <script src="{% static 'dist/js/adminlte.js' %}"></script>

    <!-- AdminLTE dashboard demo (This is only for demo purposes) -->
    <script src="{% static 'dist/js/pages/dashboard.js' %}"></script>

    <!-- AdminLTE for demo purposes -->
    <script src="{% static 'dist/js/demo.js' %}"></script>
</body>
</html>
```
Now create a home.html page of our project in the student_management_app\templates folder.
```html
{% load static %}
<html lang="en" xmlns="http://www.w3.org/1999/html">
<head>
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <meta name="description" content="Boreal Management System - Dashboard">
    <title>College Management System | Home</title>

    <!-- Bootstrap CSS -->
    <link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/4.0.0/css/bootstrap.min.css">

    <!-- Custom CSS -->
    <style>
        body {
            background-color: #32373c;
        }
        .carousel-item img {
            object-fit: cover;
            height: 85vh; /* Adjust this value as needed */
        }
        .group {
              display: flex;
              line-height: 28px;
              align-items: center;
              position: relative;
              max-width: 190px;
            }

            .input {
              height: 40px;
              line-height: 28px;
              padding: 0 1rem;
              width: 100%;
              padding-left: 2.5rem;
              border: 2px solid transparent;
              border-radius: 8px;
              outline: none;
              background-color: #D9E8D8;
              color: #0d0c22;
              box-shadow: 0 0 5px #C1D9BF, 0 0 0 10px #f5f5f5eb;
              transition: .3s ease;
            }

            .input::placeholder {
              color: #777;
            }

            .icon {
              position: absolute;
              left: 1rem;
              fill: #777;
              width: 1rem;
              height: 1rem;
            }
    </style>
</head>
<body>

<!-- Navigation Bar -->
<nav class="navbar navbar-expand-lg navbar-white bg-white">
    <a class="c-header_logo" href="https://collegeboreal.ca">
        <img alt="Logo" data-src="https://collegeboreal.ca/wp-content/themes/boreal-theme/assets/src/images/logo.svg" class=" ls-is-cached lazyloaded" src="https://collegeboreal.ca/wp-content/themes/boreal-theme/assets/src/images/logo.svg"><noscript><img src="https://collegeboreal.ca/wp-content/themes/boreal-theme/assets/src/images/logo.svg" alt="Logo"></noscript>
    </a>
    <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarSupportedContent"
            aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
        <span class="navbar-toggler-icon"></span>
    </button>

    <div class="collapse navbar-collapse" id="navbarSupportedContent">
        <ul class="navbar-nav mr-auto">
            <!-- You can add additional navigation links here -->
        </ul>
        <form class="form-inline my-2 my-lg-0">
            <div class="group">
                <svg class="icon" aria-hidden="true" viewBox="0 0 24 24">
                    <g>
                        <path d="M21.53 20.47l-3.66-3.66C19.195 15.24 20 13.214 20 11c0-4.97-4.03-9-9-9s-9 4.03-9 9 4.03 9 9 9c2.215 0 4.24-.804 5.808-2.13l3.66 3.66c.147.146.34.22.53.22s.385-.073.53-.22c.295-.293.295-.767.002-1.06zM3.5 11c0-4.135 3.365-7.5 7.5-7.5s7.5 3.365 7.5 7.5-3.365 7.5-7.5 7.5-7.5-3.365-7.5-7.5z"></path>
                    </g>
                </svg>
                <input placeholder="Search" type="search" class="input">
            </div>
            </input>

            <a href="/login" class="btn btn-outline-success my-1 mx-2">Login</a>
            <a href="/registration" class="btn btn-outline-success my-1 mx-2">Register</a>
            <a href="/contact" class="btn btn-outline-danger my-1 mx-2">Contact Us</a>
        </form>
    </div>
</nav>

<!-- Carousel -->
<div id="carouselExampleIndicators" class="carousel slide" data-ride="carousel">
    <ol class="carousel-indicators">
        <li data-target="#carouselExampleIndicators" data-slide-to="0" class="active"></li>
        <li data-target="#carouselExampleIndicators" data-slide-to="1"></li>
        <li data-target="#carouselExampleIndicators" data-slide-to="2"></li>
        <!-- Add more indicators if needed -->
    </ol>
    <div class="carousel-inner">
        <div class="carousel-item active">
            <video class="c-page-header_img w-100" loop="" muted="" playsinline="" autoplay="">
                <source src="https://collegeboreal.ca/wp-content/uploads/2023/06/boreal-final-export.mp4" type="video/mp4">
            </video>
        </div>
        <div class="carousel-item">
            <img class="d-block w-100" src="{% static 'static/images/401-208_resultats_ir_tele_fr-1440x810.jpg' %}" alt="Second slide">
        </div>
        <div class="carousel-item">
            <img class="d-block w-100" src="{% static 'images/banner3.jpg' %}" alt="Third slide">
        </div>
        <!-- Add more carousel items if needed -->
    </div>
    <a class="carousel-control-prev" href="#carouselExampleIndicators" role="button" data-slide="prev">
        <span class="carousel-control-prev-icon" aria-hidden="true"></span>
        <span class="sr-only">Previous</span>
    </a>
    <a class="carousel-control-next" href="#carouselExampleIndicators" role="button" data-slide="next">
        <span class="carousel-control-next-icon" aria-hidden="true"></span>
        <span class="sr-only">Next</span>
    </a>
</div>

<!-- Bootstrap JS (jQuery is already included in Bootstrap) -->
<script src="https://maxcdn.bootstrapcdn.com/bootstrap/4.0.0/js/bootstrap.min.js"></script>

</body>
</html>
```
**Output:** 
![image](https://github.com/JPK2001/Learning-Django/assets/115308301/67b2dde9-b59a-45e9-ac17-7b72805cabf2)

Now create a registration.html page where students, staff, HOD can register themselves.
```html
{% load static %}
<html lang="en">
<head>
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Registration Page</title>

    <!-- Bootstrap CSS -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/twitter-bootstrap/4.1.3/css/bootstrap.min.css">

    <!-- Custom CSS -->
    <link rel="stylesheet" href="{% static 'assets/css/style.css' %}">
    <style>
        body {
    background-color: #4CAF50; /* Clear green */
}

.form {
    display: flex;
    flex-direction: column;
    gap: 10px;
    max-width: 350px;
    padding: 20px;
    border-radius: 20px;
    position: relative;
    background-color: #FFFFFF; /* White */
    color: #000000; /* Black */
    border: 1px solid #333;
}

.title {
    font-size: 28px;
    font-weight: 600;
    letter-spacing: -1px;
    position: relative;
    display: flex;
    align-items: center;
    padding-left: 30px;
    color: #4CAF50; /* Clear green */
}

.title::before {
    width: 18px;
    height: 18px;
}

.title::after {
    width: 18px;
    height: 18px;
    animation: pulse 1s linear infinite;
}

.title::before,
.title::after {
    position: absolute;
    content: "";
    height: 16px;
    width: 16px;
    border-radius: 50%;
    left: 0px;
    background-color: #4CAF50; /* Clear green */
}

.message,
.signin {
    font-size: 14.5px;
    color: rgba(0, 0, 0, 0.7); /* 70% opacity black */
}

.signin {
    text-align: center;
}

.signin a:hover {
    text-decoration: underline royalblue;
}

.signin a {
    color: #4CAF50; /* Clear green */
}

.flex {
    display: flex;
    width: 100%;
    gap: 6px;
}

.form label {
    position: relative;
}

.form label .input {
    background-color: #FFFFFF; /* White */
    color: #000000; /* Black */
    width: 100%;
    padding: 20px 05px 05px 10px;
    outline: 0;
    border: 1px solid rgba(105, 105, 105, 0.397);
    border-radius: 10px;
}

.form label .input + span {
    color: rgba(0, 0, 0, 0.5); /* 50% opacity black */
    position: absolute;
    left: 10px;
    top: 0px;
    font-size: 0.9em;
    cursor: text;
    transition: 0.3s ease;
}

.form label .input:placeholder-shown + span {
    top: 12.5px;
    font-size: 0.9em;
}

.form label .input:focus + span,
.form label .input:valid + span {
    color: #4CAF50; /* Clear green */
    top: 0px;
    font-size: 0.7em;
    font-weight: 600;
}

.input {
    font-size: medium;
}

.submit {
    border: none;
    outline: none;
    padding: 10px;
    border-radius: 10px;
    color: #FFFFFF; /* White */
    font-size: 16px;
    transform: .3s ease;
    background-color: #4CAF50; /* Clear green */
}
.login-dark {
    display: flex;
    justify-content: center;
    align-items: center;
    height: 100vh;
}
.submit:hover {
    background-color: #4CAF50A6; /* Clear green with 65% opacity */
}

@keyframes pulse {
    from {
        transform: scale(0.9);
        opacity: 1;
    }

    to {
        transform: scale(1.8);
        opacity: 0;
    }
}
button {
 appearance: none;
 background-color: transparent;
 border: 0.125em solid #1A1A1A;
 border-radius: 0.9375em;
 box-sizing: border-box;
 color: #3B3B3B;
 cursor: pointer;
 display: inline-block;
 font-family: Roobert,-apple-system,BlinkMacSystemFont,"Segoe UI",Helvetica,Arial,sans-serif,"Apple Color Emoji","Segoe UI Emoji","Segoe UI Symbol";
 font-size: 16px;
 font-weight: 600;
 line-height: normal;
 margin: 0;
 min-height: 3.75em;
 min-width: 0;
 outline: none;
 padding: 1em 2.3em;
 text-align: center;
 text-decoration: none;
 transition: all 300ms cubic-bezier(.23, 1, 0.32, 1);
 user-select: none;
 -webkit-user-select: none;
 touch-action: manipulation;
 will-change: transform;
}

button:disabled {
 pointer-events: none;
}

button:hover {
 color: #fff;
 background-color: #1A1A1A;
 box-shadow: rgba(0, 0, 0, 0.25) 0 8px 15px;
 transform: translateY(-2px);
}

button:active {
 box-shadow: none;
 transform: translateY(0);
}
    </style>
</head>
<body>

<!-- Navigation Bar -->
<nav class="navbar navbar-expand-lg navbar-white bg-white">
    <button><a class="navbar-brand" href="/">BACK TO HOME PAGE</a></button>
    <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarSupportedContent"
            aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
        <span class="navbar-toggler-icon"></span>
    </button>
    <div class="collapse navbar-collapse" id="navbarSupportedContent">
        <ul class="navbar-nav mr-auto">
        </ul>
        <form class="form-inline my-2 my-lg-0">
            <a href="/login" class="btn btn-outline-success my-1 mx-2">Login Here</a>
            <a href="/contact" class="btn btn-outline-danger my-1 mx-2">Contact Us</a>
        </form>
    </div>
</nav>

<!-- Registration Form -->
<div class="login-dark form-inline py-0 mx-4 my-4 pl-4 pr-4">
    <form class="form" action="{% url 'doRegistration' %}" method="get">
        {% csrf_token %}
        <p class="title">Register </p>
        <p class="message">Please Sign Up Here and Get Access to your Board. </p>
        <div class="flex">
            <label>
                <input class="input" type="text" placeholder="" required="">
                <span>Firstname</span>
            </label>
            <label>
                <input class="input" type="text" placeholder="" required="">
                <span>Lastname</span>
            </label>
        </div>
        <label>
            <input class="input" type="email" placeholder="" required="">
            <span>Email (Employee/Student)</span>
        </label>
        <label>
            <input class="input" type="password" placeholder="" required="">
            <span>Password</span>
        </label>
        <label>
            <input class="input" type="password" placeholder="" required="">
            <span>Confirm password</span>
        </label>
        <button class="submit">Submit</button>
        <p class="signin">Already have an account? <a href="/login">Login</a> </p>
    </form>
</div>

<!-- Bootstrap JS -->
<script src="https://cdnjs.cloudflare.com/ajax/libs/jquery/3.3.1/jquery.min.js"></script>
<script src="https://cdnjs.cloudflare.com/ajax/libs/twitter-bootstrap/4.1.3/js/bootstrap.bundle.min.js"></script>
</body>
</html>
```
**Output:** 
![image](https://github.com/JPK2001/Learning-Django/assets/115308301/caa4ec34-5772-4851-9ba4-83163cdb4b42)

Now create a login_page.html where students, staff, HOD can log in themselves.
```html
{% load static %}
<html lang="en">
<head>
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=0">
    <title>Login Page</title>

    <!-- Bootstrap CSS -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/twitter-bootstrap/4.1.3/css/bootstrap.min.css">

    <!-- Custom CSS -->
    <link rel="stylesheet" href="{% static 'assets/css/style.css' %}">
    <style>
    body {
    background-color: #4CAF50; /* Clear green */
}
        .form {
  display: flex;
  flex-direction: column;
  gap: 10px;
  padding-left: 2em;
  padding-right: 2em;
  padding-bottom: 0.4em;
  background-color: #FFFFFF;
  border-radius: 20px;
}

#heading {
  text-align: center;
  margin: 2em;
  color: rgb(0, 255, 200);
  font-size: 1.2em;
}

.field {
  display: flex;
  align-items: center;
  justify-content: center;
  gap: 0.5em;
  border-radius: 25px;
  padding: 0.6em;
  border: none;
  outline: none;
  color: white;
  background-color: #FFFFFF;
  box-shadow: inset 2px 5px 10px rgb(5, 5, 5);
}

.input-icon {
  height: 1.3em;
  width: 1.3em;
  fill: rgb(0, 255, 200);
}

.input-field {
  background: none;
  border: none;
  outline: none;
  width: 100%;
  color: r+#000000;
}

.form .btn {
  display: flex;
  justify-content: center;
  flex-direction: row;
  margin-top: 2.5em;
}

.button1 {
  padding: 0.5em;
  padding-left: 1.1em;
  padding-right: 1.1em;
  border-radius: 5px;
  margin-right: 0.5em;
  border: none;
  outline: none;
  transition: .4s ease-in-out;
  background-image: linear-gradient(163deg, #00ff75 0%, #3700ff 100%);
  color: rgb(0, 0, 0);
}

.button1:hover {
  background-image: linear-gradient(163deg, #00642f 0%, #4CAF50A6 100%);
  color: rgb(0, 255, 200);
}

.button2 {
  padding: 0.5em;
  padding-left: 2.3em;
  padding-right: 2.3em;
  border-radius: 5px;
  border: none;
  outline: none;
  transition: .4s ease-in-out;
  background-image: linear-gradient(163deg, #00ff75 0%, #3700ff 100%);
  color: rgb(0, 0, 0);
}

.button2:hover {
  background-image: linear-gradient(163deg, #00642f 0%, #4CAF50A6 100%);
  color: #4CAF50A6;
}

.button3 {
  margin-bottom: 3em;
  padding: 0.5em;
  border-radius: 5px;
  border: none;
  outline: none;
  transition: .4s ease-in-out;
  background-image: linear-gradient(163deg, #00ff75 0%, #3700ff 100%);
  color: rgb(0, 0, 0);
}

.button3:hover {
  background-image: linear-gradient(163deg, #a00000fa 0%, #4CAF50A6 100%);
  color: rgb(255, 255, 255);
}

.login-dark {
    display: flex;
    justify-content: center;
    align-items: center;
    height: 100vh;
}
button {
 appearance: none;
 background-color: transparent;
 border: 0.125em solid #1A1A1A;
 border-radius: 0.9375em;
 box-sizing: border-box;
 color: #3B3B3B;
 cursor: pointer;
 display: inline-block;
 font-family: Roobert,-apple-system,BlinkMacSystemFont,"Segoe UI",Helvetica,Arial,sans-serif,"Apple Color Emoji","Segoe UI Emoji","Segoe UI Symbol";
 font-size: 16px;
 font-weight: 600;
 line-height: normal;
 margin: 0;
 min-height: 3.75em;
 min-width: 0;
 outline: none;
 padding: 1em 2.3em;
 text-align: center;
 text-decoration: none;
 transition: all 300ms cubic-bezier(.23, 1, 0.32, 1);
 user-select: none;
 -webkit-user-select: none;
 touch-action: manipulation;
 will-change: transform;
}

button:disabled {
 pointer-events: none;
}

button:hover {
 color: #fff;
 background-color: #1A1A1A;
 box-shadow: rgba(0, 0, 0, 0.25) 0 8px 15px;
 transform: translateY(-2px);
}

button:active {
 box-shadow: none;
 transform: translateY(0);
}
    </style>
</head>
<body>

<!-- Navigation Bar -->
<nav class="navbar navbar-expand-lg navbar-white bg-white">
    <button><a class="navbar-brand" href="/">BACK TO HOME PAGE</a></button>
    <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarSupportedContent"
            aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
        <span class="navbar-toggler-icon"></span>
    </button>
    <div class="collapse navbar-collapse" id="navbarSupportedContent">
        <ul class="navbar-nav mr-auto">
        </ul>
        <form class="form-inline my-2 my-lg-0">
            <a href="{% url 'contact' %}" class="btn btn-outline-danger my-1 mx-2">Contact Us</a>
        </form>
    </div>
</nav>

<!-- Login Form -->
<div class="login-dark form-inline py-0 mx-4 my-4 pl-4 pr-4">
    <form class="form" action="{% url 'doLogin' %}" method="get">
        {% csrf_token %}
        <p id="heading">Login</p>
        <div class="field">
        <svg class="input-icon" xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" viewBox="0 0 16 16">
        <path d="M13.106 7.222c0-2.967-2.249-5.032-5.482-5.032-3.35 0-5.646 2.318-5.646 5.702 0 3.493 2.235 5.708 5.762 5.708.862 0 1.689-.123 2.304-.335v-.862c-.43.199-1.354.328-2.29.328-2.926 0-4.813-1.88-4.813-4.798 0-2.844 1.921-4.881 4.594-4.881 2.735 0 4.608 1.688 4.608 4.156 0 1.682-.554 2.769-1.416 2.769-.492 0-.772-.28-.772-.76V5.206H8.923v.834h-.11c-.266-.595-.881-.964-1.6-.964-1.4 0-2.378 1.162-2.378 2.823 0 1.737.957 2.906 2.379 2.906.8 0 1.415-.39 1.709-1.087h.11c.081.67.703 1.148 1.503 1.148 1.572 0 2.57-1.415 2.57-3.643zm-7.177.704c0-1.197.54-1.907 1.456-1.907.93 0 1.524.738 1.524 1.907S8.308 9.84 7.371 9.84c-.895 0-1.442-.725-1.442-1.914z"></path>
        </svg>
          <input autocomplete="off" placeholder="Username" class="input-field" type="text">
        </div>
        <div class="field">
        <svg class="input-icon" xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" viewBox="0 0 16 16">
        <path d="M8 1a2 2 0 0 1 2 2v4H6V3a2 2 0 0 1 2-2zm3 6V3a3 3 0 0 0-6 0v4a2 2 0 0 0-2 2v5a2 2 0 0 0 2 2h6a2 2 0 0 0 2-2V9a2 2 0 0 0-2-2z"></path>
        </svg>
          <input placeholder="Password" class="input-field" type="password">
        </div>
        <div class="btn">
        <button class="button1">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Login&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</button>
        <button class="button2"><a href="/registration" class="btn btn-outline-success my-1 mx-2">Sign Up</a></button>
        </div>
        <button class="button3">Forgot Password</button>
    </form>
</div>

<!-- Bootstrap JS -->
<script src="https://cdnjs.cloudflare.com/ajax/libs/jquery/3.2.1/jquery.min.js"></script>
<script src="https://cdnjs.cloudflare.com/ajax/libs/twitter-bootstrap/4.1.3/js/bootstrap.bundle.min.js"></script>
</body>
</html>
```
**Output:** 
![image](https://github.com/JPK2001/Learning-Django/assets/115308301/74119395-0b8b-438e-9a84-431852697d04)

Create contact.html 
```html
{% load static %}
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Contact Us</title>

    <!-- Bootstrap CSS -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/twitter-bootstrap/4.1.3/css/bootstrap.min.css">

    <!-- Custom CSS -->
    <link rel="stylesheet" href="{% static 'assets/css/style.css' %}">
    <style>
        .container {
    max-width: 600px;
    margin: 0 auto;
}

.jumbotron {
    background-color: #f8f9fa; /* Couleur de fond */
    padding: 40px;
    border-radius: 15px;
    box-shadow: 0 0 15px rgba(0, 0, 0, 0.1); /* Ombre douce */
}

.form-group {
    margin-bottom: 20px;
}

label {
    font-weight: bold;
}

.form-control {
    border-radius: 8px;
    border: 1px solid #ced4da; /* Bordure grise */
}

textarea.form-control {
    resize: vertical; /* Permettre le redimensionnement vertical */
}

.btn-primary {
    background-color: #007bff; /* Couleur de fond du bouton */
    border-color: #007bff; /* Couleur de la bordure du bouton */
}

.btn-primary:hover {
    background-color: #0056b3; /* Couleur de fond au survol */
    border-color: #0056b3; /* Couleur de la bordure au survol */
}
button {
 appearance: none;
 background-color: transparent;
 border: 0.125em solid #1A1A1A;
 border-radius: 0.9375em;
 box-sizing: border-box;
 color: #3B3B3B;
 cursor: pointer;
 display: inline-block;
 font-family: Roobert,-apple-system,BlinkMacSystemFont,"Segoe UI",Helvetica,Arial,sans-serif,"Apple Color Emoji","Segoe UI Emoji","Segoe UI Symbol";
 font-size: 16px;
 font-weight: 600;
 line-height: normal;
 margin: 0;
 min-height: 3.75em;
 min-width: 0;
 outline: none;
 padding: 1em 2.3em;
 text-align: center;
 text-decoration: none;
 transition: all 300ms cubic-bezier(.23, 1, 0.32, 1);
 user-select: none;
 -webkit-user-select: none;
 touch-action: manipulation;
 will-change: transform;
}

button:disabled {
 pointer-events: none;
}

button:hover {
 color: #fff;
 background-color: #1A1A1A;
 box-shadow: rgba(0, 0, 0, 0.25) 0 8px 15px;
 transform: translateY(-2px);
}

button:active {
 box-shadow: none;
 transform: translateY(0);
}
    </style>
</head>
<body>

<!-- Navigation Bar -->
<nav class="navbar navbar-expand-lg navbar-white bg-white">
    <button><a href="/" class="btn btn-outline-primary my-1 mx-2">Go Back To Home Page</a></button>
    <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarSupportedContent"
            aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
        <span class="navbar-toggler-icon"></span>
    </button>
    <div class="collapse navbar-collapse" id="navbarSupportedContent">
        <ul class="navbar-nav mr-auto">
        </ul>
        <form class="form-inline my-2 my-lg-0">
            <button><a class="form-control mr-sm-2" type="login" placeholder="Login" aria-label="Login" href="/login">Login</a></button>
            <button><a class="form-control mr-sm-2" type="Register" placeholder="Register" aria-label="Register" href="/registration">Register</a></button>
        </form>
    </div>
</nav>

<!-- Hero Image -->
<div class="container-fluid px-0">
    <img src="{% static 'dist/img/contact.jpg' %}" class="d-block w-100 mx-0" alt="Contact" height="450px">
</div>

<!-- Contact Form -->
<div class="container">
    <div class="jumbotron">
        <h1 class="text-center mb-4">Contact Us</h1>
        <form action="/contact" method="post">
            {% csrf_token %}
            <div class="form-group">
                <label for="name">Name</label>
                <input type="text" class="form-control" id="name" name="name" placeholder="Enter your Name">
            </div>
            <div class="form-group">
                <label for="email">Email</label>
                <input type="email" class="form-control" id="email" name="email" placeholder="Enter your Email">
            </div>
            <div class="form-group">
                <label for="phone">Phone number</label>
                <input type="number" class="form-control" id="phone" name="phone" placeholder="Enter your Phone number">
            </div>
            <div class="form-group">
                <label for="message">Message</label>
                <textarea class="form-control" id="message" rows="5" name="message" placeholder="How can we help you?"></textarea>
            </div>
            <button type="submit" class="btn btn-primary btn-lg btn-block">Submit</button>
        </form>
    </div>
</div>

<!-- Bootstrap JS -->
<script src="https://cdnjs.cloudflare.com/ajax/libs/jquery/3.2.1/jquery.min.js"></script>
<script src="https://cdnjs.cloudflare.com/ajax/libs/twitter-bootstrap/4.1.3/js/bootstrap.bundle.min.js"></script>

</body>
</html>
```
**Output:** 
![image](https://github.com/JPK2001/Learning-Django/assets/115308301/dfb95b9d-1e3a-4c04-9e66-33d46dd37f56)

# Run these commands to migrate your models into the database. When you successfully do all the steps you will get this type of output in CMD.
```
python manage.py makemigrations
```
![image](https://github.com/JPK2001/Learning-Django/assets/115308301/84545ac2-5458-4883-838d-06be069b6eec)

```
python manage.py migrate
```
![image](https://github.com/JPK2001/Learning-Django/assets/115308301/7c167c27-b715-424a-8643-ffcd70d694f2)

# Creating an admin user
First we’ll need to create a user who can login to the admin site. Run the following command:

$ python manage.py createsuperuser
Enter your desired username and press enter.

Username: admin
You will then be prompted for your desired email address:

Email address: admin@example.com
The final step is to enter your password. You will be asked to enter your password twice, the second time as a confirmation of the first.

Password: **********
Password (again): *********
Superuser created successfully.
![image](https://github.com/JPK2001/Learning-Django/assets/115308301/09b00dfe-7248-4c27-b19a-84f0e94fb31a)
![image](https://github.com/JPK2001/Learning-Django/assets/115308301/2f254575-0784-4b72-8def-ca207645fed6)
