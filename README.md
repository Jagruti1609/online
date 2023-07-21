<html>
<head>
<title>First Login Page</title>
<meta name="viewport" content="width=device-width, initial-scale=1">
<link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/4.1.3/css/bootstrap.min.css">
  <script src="https://ajax.googleapis.com/ajax/libs/jquery/3.3.1/jquery.min.js"></script>
  <script src="https://cdnjs.cloudflare.com/ajax/libs/popper.js/1.14.3/umd/popper.min.js"></script>
  <script src="https://maxcdn.bootstrapcdn.com/bootstrap/4.1.3/js/bootstrap.min.js"></script>
<style>
body {
  margin: 0;
  font-family: Arial, Helvetica, sans-serif;
}
form {
	border:3px solid #f1f1f1  ;}


.hero-image {
  background-image: url("http://www.hdnicewallpapers.com/Walls/Big/Flowers/Beautiful_Nice_Purple_Flower_Wallpapers.jpg");
  background-color: #cccccc;
  height:800px;
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;
  position: relative;
}

 .hero-text {
  text-align: center;
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  color: white;
}

input[type=text], input[type=password] {
  width: 100%;
  padding: 12px 20px;
  margin: 8px 0;
  display: inline-block;
  border: 1px solid #ccc;
  box-sizing: border-box;
}

button {
  background-color: #4CAF50;
  color: white;
  padding: 14px 20px;
  margin: 8px 0;
  border: none;
  cursor: pointer;
  width: 100%;
}


button:hover {
  opacity: 0.8;
}

.cancelbtn {
  width: auto;
  padding: 10px 18px;
  background-color: #f44336;
}


.imgcontainer {

  text-align: center;
  margin: 12px 0 8px 0;
}

img.avatar {
	
  width:40%;
  border-radius: 50%;
}

.container {

  text-align:left;
  padding:20px;
}

span.psw {
  float: right;
  padding-top:16px;
}


@media screen and (max-width: 90px) {
  span.psw {
     display: block;
     float: none;
  }
  .cancelbtn {
	
     width:60%;
  }
}
</style>
</head>
<body>


<div class="hero-image">
<div class="hero-text">
<h2></h2>
<h3 align=center>Login Form</h3>
<form>
<div class="imgcontainer">
<img src="https://www.findmecure.com/Content/Images/recommended/girl-min.png" alt="Avatar" class="avatar">
</div>
<div class="container">

<b align=left>Username</b>
<input type="text" placeholder="Enter Username" name="uname" 
value="<?php if(isset($_GET['uname'])) echo $_GET['uname']?>">

<b>Password</b>
<input type="password" placeholder="Enter Password" name="psw" 
value="<?php if(isset($_GET['psw'])) echo $_GET['psw']?>">
        
<button type="submit" name="sub">Login</button>

<button type="submit" name="reg">Create New User</button>


<input type="checkbox" checked="checked" name="remember"> Remember me
</label>
</div>

<div class="container">
<button type="button" class="cancelbtn">Cancel</button>
<span class="psw"><a href="forgotpwd.php">Forgot password?</a></span>
</div>
</form>
</div>
</div>
</body>
</html>


