# Step 3: Building the Web page for the App.
Now create a base.html page.
```html
{% load static %} 

<!DOCTYPE html> 
<html> 
<head> 
<meta charset="utf-8"> 
<meta http-equiv="X-UA-Compatible" content="IE=edge"> 
<title>College Management System | Dashboard</title> 
<!-- Tell the browser to be responsive to screen width -->
<meta name="viewport" content="width=device-width, initial-scale=1"> 
<meta name="viewport" content="width=device-width, initial-scale=1"> 
<!-- Font Awesome -->
<link rel="stylesheet" href="{% static "fontawesome-free/css/all.min.css" %}"> 
<!-- Ionicons -->
	
<!-- Bootstrap CSS -->
<link href="https://cdn.jsdelivr.net/npm/bootstrap@5.0.0-beta3/dist/css/bootstrap.min.css" rel="stylesheet" integrity="sha384-eOJMYsd53ii+scO/bJGFsiCZc+5NDVN2yr8+0RDqr0Ql0h+rP48ckxlpbzKgwra6" crossorigin="anonymous"> 

<link rel="stylesheet" href="https://code.ionicframework.com/ionicons/2.0.1/css/ionicons.min.css"> 
<!-- Tempusdominus Bbootstrap 4 -->
<link rel="stylesheet" href="{% static 'tempusdominus-bootstrap-4/css/tempusdominus-bootstrap-4.min.css' %}"> 
<!-- iCheck -->
<link rel="stylesheet" href="{% static "icheck-bootstrap/icheck-bootstrap.min.css" %}"> 
<!-- JQVMap -->
<link rel="stylesheet" href="{% static "jqvmap/jqvmap.min.css" %}"> 
<!-- Theme style -->
<link rel="stylesheet" href="{% static 'dist/css/adminlte.min.css' %}"> 
<!-- overlayScrollbars -->
<link rel="stylesheet" href="{% static "overlayScrollbars/css/OverlayScrollbars.min.css" %}"> 
<!-- Daterange picker -->
<link rel="stylesheet" href="{% static "daterangepicker/daterangepicker.css" %}"> 
<!-- summernote -->
<link rel="stylesheet" href="{% static "summernote/summernote-bs4.css" %}"> 
<!-- Google Font: Source Sans Pro -->
<link href="https://fonts.googleapis.com/css?family=Source+Sans+Pro:300,400,400i,700" rel="stylesheet"> 

</head> 



{% block content %} 


{% endblock content %} 

<!-- jQuery -->
	<!-- Optional JavaScript -->
	<!-- jQuery first, then Popper.js, then Bootstrap JS -->
	<script src="https://code.jquery.com/jquery-3.4.1.slim.min.js" integrity="sha384-J6qa4849blE2+poT4WnyKhv5vZF5SrPo0iEjwBvKU7imGFAV0wwj1yYfoRSJoZ+n" crossorigin="anonymous"></script> 
	<script src="https://cdn.jsdelivr.net/npm/popper.js@1.16.0/dist/umd/popper.min.js" integrity="sha384-Q6E9RHvbIyZFJoft+2mJbHaEWldlvI9IOYy5n3zV9zzTtmI3UksdQRVvoxMfooAo" crossorigin="anonymous"></script> 
	<script src="https://stackpath.bootstrapcdn.com/bootstrap/4.4.1/js/bootstrap.min.js" integrity="sha384-wfSDF2E50Y2D1uUdj0O3uMBJnjuUD4Ih7YwaYd1iqfktj0Uod8GCExl3Og8ifwB6" crossorigin="anonymous"></script> 

<script src="{% static "jquery/jquery.min.js" %}"></script> 
<!-- jQuery UI 1.11.4 -->
<script src="{% static "jquery-ui/jquery-ui.min.js" %}"></script> 
<!-- Resolve conflict in jQuery UI tooltip with Bootstrap tooltip -->
<script> 
$.widget.bridge('uibutton', $.ui.button) 
</script> 
<!-- Bootstrap 4 -->
<script src="{% static "bootstrap/js/bootstrap.bundle.min.js" %}"></script> 
<!-- ChartJS -->
<script src="{% static "chart.js/Chart.min.js" %}"></script> 
<!-- Sparkline -->
<script src="{% static "sparklines/sparkline.js" %}"></script> 
<!-- JQVMap -->
<script src="{% static "jqvmap/jquery.vmap.min.js" %}"></script> 
<script src="{% static "jqvmap/maps/jquery.vmap.usa.js" %}"></script> 
<!-- jQuery Knob Chart -->
<script src="{% static "jquery-knob/jquery.knob.min.js" %}"></script> 
<!-- daterangepicker -->
<script src="{% static "moment/moment.min.js" %}"></script> 
<script src="{% static "daterangepicker/daterangepicker.js" %}"></script> 
<!-- Tempusdominus Bootstrap 4 -->
<script src="{% static "tempusdominus-bootstrap-4/js/tempusdominus-bootstrap-4.min.js" %}"></script> 
<!-- Summernote -->
<script src="{% static "summernote/summernote-bs4.min.js" %}"></script> 
<!-- overlayScrollbars -->
<script src="{% static "overlayScrollbars/js/jquery.overlayScrollbars.min.js" %}"></script> 
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
{% extends 'base.html' %} 
{% load static %} 
{% block title %}Home{% endblock title %} 

{% block content %} 
<html> 
<head> 

<style> 
img { 
background-size: cover; 
} 
body {background-color: coral;} 

</style> 

<link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/4.0.0-alpha.6/css/bootstrap.min.css" integrity="sha384-rwoIResjU2yc3z8GV/NPeZWAv56rSmLldC3R/AZzGRnGxQQKnKkoFVhFQhNUwEyJ" crossorigin="anonymous"> 
<script src="https://code.jquery.com/jquery-3.1.1.slim.min.js" integrity="sha384-A7FZj7v+d/sdmMqp/nOQwliLvUsJfDHW+k9Omg/a/EheAdgtzNs3hpfag6Ed950n" crossorigin="anonymous"></script> 
<script src="https://maxcdn.bootstrapcdn.com/bootstrap/4.0.0-alpha.6/js/bootstrap.min.js" integrity="sha384-vBWWzlZJ8ea9aCX4pEW3rVHjgjt7zpkNpZk+02D9phzyeVkE+jo0ieGizqPLForn" crossorigin="anonymous"></script> 

<link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/4.0.0/css/bootstrap.min.css" integrity="sha384-Gn5384xqQ1aoWXA+058RXPxPg6fy4IWvTNh0E263XmFcJlSAwiGgFAW/dAiS6JXm" crossorigin="anonymous"> 
<script src="https://maxcdn.bootstrapcdn.com/bootstrap/4.0.0/js/bootstrap.min.js" integrity="sha384-JZR6Spejh4U02d8jOt6vLEHfe/JQGiRRSQQxSfFWpi1MquVdAyjUar5+76PVCmYl" crossorigin="anonymous"></script> 
<script src="https://code.jquery.com/jquery-3.2.1.slim.min.js" integrity="sha384-KJ3o2DKtIkvYIK3UENzmM7KCkRr/rE9/Qpg6aAZGJwFDMVNA/GpGFF93hXpG5KkN" crossorigin="anonymous"></script> 
<script src="https://cdnjs.cloudflare.com/ajax/libs/popper.js/1.12.9/umd/popper.min.js" integrity="sha384-ApNbgh9B+Y1QKtv3Rn7W3mgPxhU9K/ScQsAP7hUibX39j7fakFPskvXusvfa0b4Q" crossorigin="anonymous"></script> 

</head> 

<nav class="navbar navbar-expand-lg navbar-dark bg-dark"> 
	<a class="navbar-brand" href=""><h3>WELCOME TO CMS</h3></a> 
<button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation"> 
	<span class="navbar-toggler-icon"></span> 
</button> 

<div class="collapse navbar-collapse" id="navbarSupportedContent"> 
	<ul class="navbar-nav mr-auto"> 
	</ul> 
	<form class="form-inline my-2 my-lg-0"> 
	<!--<input class="form-control mr-sm-2" type="search" placeholder="Search" aria-label="Search">-->
<a href="/logi" class="btn btn-outline-success my-1 mx-2">Login</a> 

	<!--<input class="form-control mr-sm-2" type="Register" placeholder="Register" aria-label="Register">-->
	<a href="/registration" class="btn btn-outline-success my-1 mx-2">Register</a> 
		<a href="/contact" class="btn btn-outline-danger my-1 mx-2">Contact Us</a> 
	</form> 
</div> 
</nav> 

<div id="carouselExampleIndicators" class="carousel slide" data-ride="carousel"> 
<ol class="carousel-indicators"> 

</ol> 
<div class="carousel-inner"> 
	<div class="carousel-item active"> 
	{% comment %} <img class="d-block w-100" src="https://images.unsplash.com/20/cambridge.JPG?ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&ixlib=rb-1.2.1&auto=format&fit=crop&w=1030&q=80" alt="First slide"> {% endcomment %} 
	<img src="{% static 'dist/img/111.png' %}" class="d-block w-100 h-100 size-cover" alt="..."> 
	</div> 
		<div class="carousel-item"> 
	{% comment %} <img class="d-block w-100" src="https://images.unsplash.com/photo-1541339907198-e08756dedf3f?ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&ixlib=rb-1.2.1&auto=format&fit=crop&w=1050&q=80" alt="Second slide"> {% endcomment %} 
	<img src="{% static 'dist/img/re.png' %}" class="d-block w-100 h-100 size-cover " alt="..."> 
	</div> 
		<div class="carousel-item"> 
	{% comment %} <img class="d-block w-100" src="https://images.unsplash.com/photo-1541339907198-e08756dedf3f?ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&ixlib=rb-1.2.1&auto=format&fit=crop&w=1050&q=80" alt="Second slide"> {% endcomment %} 
	<img src="{% static 'dist/img/e.png' %}" class="d-block w-100 h-100 size-cover " alt="..."> 
	</div> 
	<div class="carousel-item"> 
	{% comment %} <img class="d-block w-100" src="https://images.unsplash.com/photo-1541339907198-e08756dedf3f?ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&ixlib=rb-1.2.1&auto=format&fit=crop&w=1050&q=80" alt="Second slide"> {% endcomment %} 
	<img src="{% static 'dist/img/22.png' %}" class="d-block w-100 h-100 size-cover " alt="..."> 
	</div> 
	<div class="carousel-item"> 
	{% comment %} <img class="d-block w-100" src="https://images.unsplash.com/photo-1503676260728-1c00da094a0b?ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&ixlib=rb-1.2.1&auto=format&fit=crop&w=1009&q=80" alt="Third slide"> {% endcomment %} 
	<img src="{% static 'dist/img/33.png' %}" class="d-block w-100 h-100 size-cover" alt="..."> 
	</div> 
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

</html> 

{% endblock content %}
```
Now create a registration.html page where students, staff, HOD can register themselves.
```html
{% extends 'base.html' %} 
{% load static %} 
{% block content %} 
<head> 
<meta charset="utf-8"> 
<meta name="viewport" content="width=device-width, initial-scale=1.0"> 
<title>Untitled</title> 
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/twitter-bootstrap/4.1.3/css/bootstrap.min.css"> 
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/ionicons/2.0.1/css/ionicons.min.css"> 
<link rel="stylesheet" href="assets/css/style.css"> 
<style> 
	body{ 
	height:1000px;		 
	background:#475d62; 
	background-color: cover; 
	font-family: sans-seriff; 
	} 
	.login-dark { 
	max-width:320px; 
	width:90%; 
	background-color: #1e2833; 
	padding:40px; 
	border-radius:4px; 
	transform: translate(-50%,-50%); 
	position: absolute; 
	top: 50%; 
	left: 50%; 
	color:#fff; 
	box-shadow:3px 3px 4px rgba(0,0,0,0.2); 
	} 
	.login-dark form { 
	max-width:320px; 
	width:90%; 
	background-color:#1e2833; 
	padding:40px; 
	border-radius:4px; 
	transform:translate(-50%, -50%); 
	position:absolute; 
	top:50%; 
	left:50%; 
	color:#fff; 
	box-shadow:3px 3px 4px rgba(0,0,0,0.2); 
	} 
	.login-dark .illustration { 
	text-align:center; 
	padding:15px 0 20px; 
	font-size:100px; 
	color:#2980ef; 
	} 
	.login-dark form .form-control { 
	background:none; 
	border:none; 
	border-bottom:1px solid #434a52; 
	border-radius:0; 
	box-shadow:none; 
	outline:none; 
	color:inherit; 
	} 
	.login-dark form .btn-primary { 
	background:#214a80; 
	border:none; 
	border-radius:4px; 
	padding:11px; 
	box-shadow:none; 
	margin-top:26px; 
	text-shadow:none; 
	outline:none; 
	} 
	.login-dark form .btn-primary:hover, .login-dark form .btn-primary:active { 
	background:#214a80; 
	outline:none; 
	} 
	.login-dark form .forgot { 
	display:block; 
	text-align:center; 
	font-size:12px; 
	color:#6f7a85; 
	opacity:0.9; 
	text-decoration:none; 
	} 
	.login-dark form .forgot:hover, .login-dark form .forgot:active { 
	opacity:1; 
	text-decoration:none; 
	} 
	.login-dark form .btn-primary:active { 
	transform:translateY(1px); 
	} 
</style> 
</head> 
<nav class="navbar navbar-expand-lg navbar-dark bg-dark"> 
<a class="navbar-brand" href="/ "> 
	<h4>BACK TO HOME</h4> 
</a> 
<button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation"> 
<span class="navbar-toggler-icon"></span> 
</button> 
<div class="collapse navbar-collapse" id="navbarSupportedContent"> 
	<ul class="navbar-nav mr-auto"> 
	</ul> 
	<form class="form-inline my-2 my-lg-0"> 
		<!-- <input class="form-control mr-sm-2" type="login" placeholder="login" aria-label="login">-->
		<!--<input class="form-control mr-sm-2" type="Register" placeholder="Register" aria-label="Register">-->
		<a href="/logi" class="btn btn-outline-success my-1 mx-2">Login Here</a> 
		<a href="/contact" class="btn btn-outline-danger my-1 mx-2">Contact Us</a> 
		<!--<input class="form-control mr-sm-2" type="register" placeholder="register" aria-label="register">-->
	</form> 
</div> 
</nav> 
<div class="login-dark form-inline py-0 mx-4 my-4 pl-4 pr-4"> 
<form action="{% url 'doRegistration' %}" method="get"> 
{% csrf_token %} 
<h1 class="text-center">Signup</h1> 
<div class="illustration"><i class="icon ion-ios-locked-outline"></i></div> 
<div class="form-group"><input class="form-control mb-2" type="text" name="first_name" placeholder="First Name"></div> 
<div class="form-group"><input class="form-control mb-2" type="text" name="last_name" placeholder="Last Name"></div> 
<div class="form-group"><input class="form-control mb-2" type="email" name="email" placeholder="Email"></div> 
<div class="form-group"><input class="form-control mb-2" type="password" name="password" placeholder="Password"></div> 
<div class="form-group"><input class="form-control mb-2" type="password" name="confirmPassword" placeholder="Confirm Password"></div> 
<div class="form-group"><button class="btn btn-primary btn-block mt-2 ml-2" type="submit">Register</button></div> 
{% comment %} Display Messages {% endcomment %} 
{% if messages %} 
<div class="col-12"> 
{% for message in messages %} 
{% if message.tags == "error" %} 
<div class="alert alert-danger alert-dismissible fade show" role="alert" style="margin-top: 10px;"> 
	<b>{{ message }}</b> 
	<button type="button" class="btn-close" data-bs-dismiss="alert" aria-label="Close"></button> 
</div> 
{% endif %} 
{% endfor %} 
</div> 
{% endif %} 
<script src="https://cdnjs.cloudflare.com/ajax/libs/jquery/3.2.1/jquery.min.js"></script> 
<script src="https://cdnjs.cloudflare.com/ajax/libs/twitter-bootstrap/4.1.3/js/bootstrap.bundle.min.js"></script> 
{% endblock content %}
```
Now create a login_page.html where students, staff, HOD can log in themselves.
```html
{% extends 'base.html' %} 
{% load static %} 
{% block content %} 
<head> 
<meta charset="utf-8"> 
<meta name="viewport" content="width=device-width, initial-scale=1; maximum-scale=1.0; user-scalable=0;"> 
<title>Untitled</title> 
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/twitter-bootstrap/4.1.3/css/bootstrap.min.css"> 
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/ionicons/2.0.1/css/ionicons.min.css"> 
<link rel="stylesheet" href="assets/css/style.css"> 
<style> 
	body{ 
	height:1000px; 
	background:#475d62; 
	background-color: cover; 
	font-family: sans-seriff; 
	} 
	.login-dark { 
	max-width:320px; 
	width:90%; 
	background-color: #1e2833; 
	padding:40px; 
	border-radius:4px; 
	transform: translate(-50%,-50%); 
	position: absolute; 
	top: 50%; 
	left: 50%; 
	color:#fff; 
	box-shadow:3px 3px 4px rgba(0,0,0,0.2); 
	} 
	.login-dark form { 
	max-width:320px; 
	width:90%; 
	background-color:#1e2833; 
	padding:40px; 
	border-radius:4px; 
	transform:translate(-50%, -50%); 
	position:absolute; 
	top:50%; 
	left:50%; 
	color:#fff; 
	box-shadow:3px 3px 4px rgba(0,0,0,0.2); 
	} 
	.login-dark .illustration { 
	text-align:center; 
	padding:15px 0 20px; 
	font-size:100px; 
	color:#2980ef; 
	} 
	.login-dark form .form-control { 
	background:none; 
	border:none; 
	border-bottom:1px solid #434a52; 
	border-radius:0; 
	box-shadow:none; 
	outline:none; 
	color:inherit; 
	} 
	.login-dark form .btn-primary { 
	background:#214a80; 
	border:none; 
	border-radius:4px; 
	padding:11px; 
	box-shadow:none; 
	margin-top:26px; 
	text-shadow:none; 
	outline:none; 
	} 
	.login-dark form .btn-primary:hover, .login-dark form .btn-primary:active { 
	background:#214a80; 
	outline:none; 
	} 
	.login-dark form .forgot { 
	display:block; 
	text-align:center; 
	font-size:12px; 
	color:#6f7a85; 
	opacity:0.9; 
	text-decoration:none; 
	} 
	.login-dark form .forgot:hover, .login-dark form .forgot:active { 
	opacity:1; 
	text-decoration:none; 
	} 
	.login-dark form .btn-primary:active { 
	transform:translateY(1px); 
	} 
</style> 
</head> 
<nav class="navbar navbar-expand-lg navbar-dark bg-dark"> 
<a class="navbar-brand" href="/ ">BACK TO HOME</a> 
<button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation"> 
<span class="navbar-toggler-icon"></span> 
</button> 
<div class="collapse navbar-collapse" id="navbarSupportedContent"> 
	<ul class="navbar-nav mr-auto"> 
	</ul> 
	<form class="form-inline my-2 my-lg-0"> 
		<a href="{% url 'contact' %}" class="btn btn-outline-danger my-1 mx-2">Contact Us</a> 
	</form> 
	<!--	 <form class="form-inline my-2 my-lg-0">-->
</div> 
</nav> 
<div class="login-dark form-inline py-0 mx-4 my-4 pl-4 pr-4"> 
<form action="{% url 'doLogin' %}" method="get"> 
	{% csrf_token %} 
	<h1 class="text-center">Login</h1> 
	<div class="illustration"><i class="icon ion-ios-locked-outline"></i></div> 
	<div class="form-group"><input class="form-control mb-2" type="email" name="email" placeholder="Email"></div> 
	<div class="form-group"><input class="form-control mb-2" type="password" name="password" placeholder="Password"></div> 
	<div class="form-group"><button class="btn btn-primary btn-block mb-2 ml-2" type="submit">Log In</button></div> 
	<a href="/registration" class="forgot">Not Registered Yet? Register Now</a> 
</form> 
</div> 
{% comment %} Display Messages {% endcomment %} 
{% if messages %} 
<div class="col-12"> 
{% for message in messages %} 
{% if message.tags == "error" %} 
{% comment %} 
<div class="alert alert-danger alert-dismissible fade show" role="alert" style="margin-top: 10px;"> 
	<b>{{ message }}</b> 
	<button type="button" class="btn-close" data-bs-dismiss="alert" aria-label="Close"></button> 
</div> 
{% endcomment %} 
<div class="alert alert-danger alert-dismissible fade show" role="alert"> 
	<strong>Invalid Login Credentials!</strong> 
	<button type="button" class="close" data-dismiss="alert" aria-label="Close"> 
	<span aria-hidden="true">×</span> 
	</button> 
</div> 
{% endif %} 
{% endfor %} 
</div> 
{% endif %} 
<script src="https://cdnjs.cloudflare.com/ajax/libs/jquery/3.2.1/jquery.min.js"></script> 
<script src="https://cdnjs.cloudflare.com/ajax/libs/twitter-bootstrap/4.1.3/js/bootstrap.bundle.min.js"></script> 
{% endblock content %}
```
Create contact.html 
```html
{% extends 'base.html' %} 
{% load static %} 

{% block content %} 


<nav class="navbar navbar-expand-lg navbar-dark bg-dark"> 
				<a href="/ " class="btn btn-outline-primary my-1 mx-2">Go Back To Home </a> 
					<button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation"> 
					<span class="navbar-toggler-icon"></span> 
					</button> 
					
					<div class="collapse navbar-collapse" id="navbarSupportedContent"> 
					<ul class="navbar-nav mr-auto"> 
						
						
					</ul> 
					<form class="form-inline my-2 my-lg-0"> 
					<!-- <input class="form-control mr-sm-2" type="login" placeholder="login" aria-label="login">-->
						
	<!--<input class="form-control mr-sm-2" type="Register" placeholder="Register" aria-label="Register">-->
	
						<!--<input class="form-control mr-sm-2" type="register" placeholder="register" aria-label="register">-->
						
					</form> 
					<form class="form-inline my-2 my-lg-0"> 
					</div> 
				</nav> 
<div class="container-fluid px-0"> 

	<img src="{% static 'dist/img/contact.jpg' %}" class="d-block w-100 mx-0" alt="..." height=450px width=10px> 
</div> 
<div class="container"> 
	<h1 class="text-center my-3 display-2"> 
		<b>Contact Us</b> 
	</h1> 
<form action="/contact" method="post"> 
{% csrf_token %} 
	<div class="mb-3 py-2"> 
<label for="exampleFormControlInput1" class="form-label"><b>Name</b></label> 
<input type="name" class="form-control" id="exampleFormControlInput1" name = "name" placeholder="Enter your Name"> 
</div> 
		<div class="mb-3 py-2"> 
			<label for="exampleFormControlInput1" class="form-label"><b>Email id</b></label> 
<input type="email" class="form-control" id="exampleFormControlInpu2"name = "email" placeholder="Enter your Email"> 
</div> 
		<div class="mb-3 py-2"> 
			<label for="exampleFormControlInput1" class="form-label"><b>Phone number</b></label> 
<input type="number" class="form-control" id="exampleFormControlInput3" name = "phone" placeholder="Enter your Phone number"> 
</div> 
<div class="mb-3 py-2"> 
	<label for="exampleFormControlTextarea1" class="form-label"><b>How can we help you ??</b></label> 
<textarea class="form-control" id="exampleFormControlTextarea1" rows="7" name = "desc"></textarea> 
</div> 

	<button type="submit" class="btn btn-primary btn-lg ">Submit</button> 
		</form> 
</div> 



{% endblock content%}
```
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
