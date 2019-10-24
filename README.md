<!DOCTYPE html>
<html>
	<head>
		<title>demonstrating of flyers</title>
		<link rel="stylesheet" href="https://www.w3schools.com/w3css/4/w3.css">
	<script type="text/javascript"  src="https://ajax.googleapis.com/ajax/libs/angularjs/1.6.9/angular.min.js"> ></script>
		<link rel="stylesheet" type="text/css" href="cardindex.css">
		<script type="text/javascript" src="jquery.js"></script>
		<script src="https://files.codepedia.info/files/uploads/iScripts/html2canvas.js"></script>
		<script type="text/javascript" src="cardindex.js"></script>
		<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.7.0/css/font-awesome.min.css">
	</head>

			<style type="text/css">
				#bb1{
					position: absolute;
					top: 10%;
					left: 0.1%;

					display: none;
				}
				
				 #f1:hover #bb1{display: block;}
				 #f2:hover #bb1{display: block}
			  #f3:hover #bb1{display: block}
			   #f4:hover #bb1{display: block}
			  #f5:hover #bb1{display: block}
			   #f6:hover #bb1{display: block}
			    #f7:hover #bb1{display: block} 
			     #f8:hover #bb1{display: block}
			      #f9:hover #bb1{display: block} 

			      /* pagination */
			      #pagination{
			      	position: absolute;
			      	top: 280%;
			      	left: 38%;
			      }
			      /* navigation */
			      #navigation{

			      	position: absolute;
			      	top: 3%;
			      	left: 1%;

			      }
			      #cart{
			      	position: absolute;
			      left: 80%;
			      top: 1%;
			      }
			      #model{
			      	position: absolute;
			      	top: 25%;
			      	left: 33%;
			      	width: 600px;
			      	display: none;
			      }
			      #signin{
			      	position: absolute;
			      	left: 33%;
			      }
			      	#myul{
			      		position: absolute;
			      		left: 20%;
			      		top: 8%;
			      		z-index: 2;
			      		display: none;
			      	}
			      	a{text-decoration: none;}
			      	/* form image */
			      			/* timer */
			      			#date{
			      				position: absolute;
			      				top:-1%;
			      				left: 60%; 
			      				color: blue;

			      				font-family: sans-serif;


			      			}


			</style>
	<body>
		<!-- navigation -->
		
		<div class="w3-bar w3-container w3-mobile" id="navigation" style="width: 100% ;">
			<a href="https://pnvsoft.com/digitalking/index.html#" class="w3-bar-item w3-button w3-green" id="home"><i class="fa  fa-2x fa-home"></i></a>
			<a href="#" class="w3-bar-item w3-button w3-teal tablink w3-red" id="home"><i class="fa fa-2x fa-envelope "></i></a>
			<a href="#" class="w3-bar-item w3-button w3-teal tablink w3-red" id="globe"><i class="fa fa-2x fa-globe"></i></a>
			<span class="w3-bar-item w3-button w3-teal tablink w3-red" id="sign"><i class="fa fa-2x fa-sign-in"  onclick="openmodel()"></i></span>
			<input type="text" name="input" placeholder="enter something" class="w3-input w3-bar-item" style="width: 30%;" id="myinput" onkeyup="search()" onclick="list1()">
			<a href="#" class="w3-bar-item w3-button w3-teal" id="search"><i class="fa fa-2x fa-search"></i></a>

		</div>
	
		<!-- search button element -->
				<ul class="w3-ul w3-bar-block w3-margin-top w3-container w3-light-gray w3-round w3-s3 " id="myul" style="width: 30%">
					<a href="cardindex.html"><li class="w3-hover-teal">Bussiness card</li></a>
					<a href="cardindex.html"><li class="w3-hover-teal">Smart Bussiness card</li></a>
					<a href="flyercards.html"><li class="w3-hover-teal">Flyers</li></a>
					 <li class="w3-hover-teal">Flex</li>
					<li class="w3-hover-teal">Banners</li>
					<a href="cardindex.html"><li class="w3-hover-teal">Delux bussiness card</li></a>
					<li class="w3-hover-teal">other</li>
					<li class="w3-hover-teal" onclick="hidelist()">close &times</li>
				</ul>

				<!-- javascript code for searching button -->
                <script type="text/javascript">
                	function search()
                	{
                		 var input, filter, ul, li, a, i;
							  input = document.getElementById("myinput");
							  filter = input.value.toUpperCase();
							  ul = document.getElementById("myul");
							  li = ul.getElementsByTagName("li");
							  for (i = 0; i < li.length; i++) {
							    txtValue = li[i].textContent || li[i].innerText;
							    if (txtValue.toUpperCase().indexOf(filter) > -1) {
							      li[i].style.display = "";
							    } else {
							      li[i].style.display = "none";
							    }
							  }
                		
                	}
                	function list1()
                	{
                		document.getElementById("myul").style = "display:block";
                	}
                	function hidelist()
                	{
                		document.getElementById("myul").style = "display:none"
                	}
                </script>

		<div class="w3-bar w3-container" id="cart">
			<a href="#" class="w3-bar-item w3-mobile " id="home"><i class="fa fa-3x fa-heart-o w3-icon" style="color: red" title="wishlist"></i><span class="w3-badge w3-mobile " id="wishlist">0</span></a>
			<a href="#" class="w3-bar-item w3-mobile " id="home"><i class="fa fa-3x fa-shopping-cart" style="color: blue" title="cart"></i><span class="w3-badge w3-mobile"></span>0</a>
		</div>
	<div class="w3-container w3-teal w3-border w3-center w-card-4" style="width: 100%" id="flyer"><h1 class="w3-animate-zoom" style="font-size: 2.5vw">LOOKING FOR FLYERS </h1></div>
	<div class="w3-container w3-row ">
		<!-- flyer1 -->
		<div class="w3-container w3-card-4 w3-teal" style="width: 30%;" id="f1">
			<img src="PROGRAMEGUIDE1.jpg" style="width: 100%; " id="img1" class="w3-animate-zoom">
			<img src="blackbox.jpeg" style="width: 100% ;" id="bb1" class="w3-container w3-opacity w3-animate-zoom" >
			 <div class="w3-container w3-yellow w3-border w3-circle w3-quarter w3-margin-6" style="width: 5px; height: 30px ;margin: 5px;" onclick="pguide()"> </div>
			 <div class="w3-container w3-red w3-border w3-circle w3-quarter w3-margin-6" style="width: 5px; height: 30px ;margin: 5px;" onclick="pguide1()"> </div>
			 <div class="w3-container w3-orange w3-border w3-circle w3-quarter w3-margin-6" style="width: 5px; height: 30px ;margin: 5px;" onclick="pguide2()"> </div>
               
		</div>
	</div>
	<!-- for flyer2 -->
	<div class="w3-container w3-card-4 w3-teal" style="width: 28.5%;" id="f2">
			<img src="HAIRCUT.jpg" style="width: 100%; " id="img2" class="w3-animate-zoom ">
			<img src="blackbox.jpeg" style="width: 100% ;" id="bb1" class="w3-container w3-opacity w3-animate-zoom" >
			 <div class="w3-container w3-blue w3-border w3-circle w3-quarter w3-margin-6" style="width: 5px; height: 30px ;margin: 5px;" onclick="hair()"> </div>
			 <div class="w3-container w3-red w3-border w3-circle w3-quarter w3-margin-6" style="width: 5px; height: 30px ;margin: 5px;" onclick="hair1()"> </div>
			 <div class="w3-container w3-pale-red w3-border w3-circle w3-quarter w3-margin-6" style="width: 5px; height: 30px ;margin: 5px;" onclick="hair2()"> </div>

		</div>
		<!-- for flyer 3 -->
		<div class="w3-container w3-card-4 w3-teal" style="width: 30%;" id="f3">
			<img src="CHIRSTMAS1.jpg" style="width: 100%; " id="img3" class="w3-animate-zoom">
			<img src="blackbox.jpeg" style="width: 100% ;" id="bb1" class="w3-container w3-opacity w3-animate-zoom" >
			 <div class="w3-container w3-red w3-border w3-circle w3-quarter w3-margin-6" style="width: 5px; height: 30px ;margin: 5px;" onclick="christmas()"> </div>
			 <div class="w3-container w3-green w3-border w3-circle w3-quarter w3-margin-6" style="width: 5px; height: 30px ;margin: 5px;" onclick="christmas1()"> </div>
			 <div class="w3-container w3-pink w3-border w3-circle w3-quarter w3-margin-6" style="width: 5px; height: 30px ;margin: 5px;" onclick="christmas2()"> </div>

		</div>
		<!-- for flyer 4 -->
		<div class="w3-container w3-card-4 w3-teal" style="width: 30%;" id="f4">
			<img src="candy1.jpg" style="width: 100%; " id="img4" class="w3-animate-zoom">
			<img src="blackbox.jpeg" style="width: 100% ;" id="bb1" class="w3-container w3-opacity w3-animate-zoom" >
			 <div class="w3-container w3-green w3-border w3-circle w3-quarter w3-margin-6" style="width: 5px; height: 30px ;margin: 5px;" onclick="candy()"> </div>
			 <div class="w3-container w3-red w3-border w3-circle w3-quarter w3-margin-6" style="width: 5px; height: 30px ;margin: 5px;" onclick="candy1()"> </div>
			 <div class="w3-container w3-pink w3-border w3-circle w3-quarter w3-margin-6" style="width: 5px; height: 30px ;margin: 5px;" onclick="candy2()"> </div>

		</div>
		<!-- for flyer 5 -->
		<div class="w3-container w3-card-4 w3-teal" style="width: 21%;" id="f5">
			<img src="aibmflyer.jpg" style="width: 100%; " id="img5" class="w3-animate-zoom">
			<img src="blackbox.jpeg" style="width: 100% ;" id="bb1" class="w3-container w3-opacity w3-animate-zoom" >
			 <div class="w3-container w3-light-blue w3-border w3-circle w3-quarter w3-margin-6" style="width: 5px; height: 30px ;margin: 5px;" onclick="abim()"> </div>
			 <div class="w3-container w3-blue w3-border w3-circle w3-quarter w3-margin-6" style="width: 5px; height: 30px ;margin: 5px;" onclick="abim1()"> </div>
			 <div class="w3-container w3-green w3-border w3-circle w3-quarter w3-margin-6" style="width: 5px; height: 30px ;margin: 5px;" onclick="abim2()"> </div>

		</div>
		<!-- for flyer 6 -->
		<div class="w3-container w3-card-4 w3-teal" style="width: 30%;" id="f6">
			<img src="FOOD1.jpg" style="width: 100%; " id="img6" class="w3-animate-zoom">
			<img src="blackbox.jpeg" style="width: 100% ;" id="bb1" class="w3-container w3-opacity w3-animate-zoom" >
			 <div class="w3-container w3-blue w3-border w3-circle w3-quarter w3-margin-6" style="width: 5px; height: 30px ;margin: 5px;" onclick="food()"> </div>
			 <div class="w3-container w3-pink w3-border w3-circle w3-quarter w3-margin-6" style="width: 5px; height: 30px ;margin: 5px;" onclick="food1()"> </div>
			 <div class="w3-container w3-green w3-border w3-circle w3-quarter w3-margin-6" style="width: 5px; height: 30px ;margin: 5px;" onclick="food2()"> </div>

		</div>
		<!-- for flyer 7 -->
		<div class="w3-container w3-card-4 w3-teal " style="width: 28%;" id="f7">
			<img src="LOREM.jpg" style="width: 100%; " id="img7" class="w3-animate-zoom">
				<img src="blackbox.jpeg" style="width: 100% ;" id="bb1" class="w3-container w3-opacity w3-animate-zoom" >
			 <div class="w3-container w3-light-blue w3-border w3-circle w3-quarter w3-margin-6" style="width: 5px; height: 30px ;margin: 5px;" onclick="lorem()"> </div>
			 <div class="w3-container w3-blue w3-border w3-circle w3-quarter w3-margin-6" style="width: 5px; height: 30px ;margin: 5px;" onclick="lorem1()"> </div>
			 <div class="w3-container w3-red w3-border w3-circle w3-quarter w3-margin-6" style="width: 5px; height: 30px ;margin: 5px;" onclick="lorem2()"> </div>

		</div>
		<!-- for flyer 8 -->
		<div class="w3-container w3-card-4 w3-teal " style="width: 28%;" id="f8">
			<img src="mbe1.jpg" style="width: 100%; " id="img8" class="w3-animate-zoom">
				<img src="blackbox.jpeg" style="width: 100% ;" id="bb1" class="w3-container w3-opacity w3-animate-zoom" >
			 <div class="w3-container w3-red w3-border w3-circle w3-quarter w3-margin-6" style="width: 5px; height: 30px ;margin: 5px;" onclick="mbe()"> </div>
			 <div class="w3-container w3-blue w3-border w3-circle w3-quarter w3-margin-6" style="width: 5px; height: 30px ;margin: 5px;" onclick="mbe1()"> </div>
			 <div class="w3-container w3-pink w3-border w3-circle w3-quarter w3-margin-6" style="width: 5px; height: 30px ;margin: 5px;" onclick="mbe2()"> </div>

		</div>
		<!-- for flyer 9 -->
		<div class="w3-container w3-card-4 w3-teal " style="width: 28%;" id="f9">
			<img src="jansena1.jpg" style="width: 100%; " id="img9" class="w3-animate-zoom" >
				<img src="blackbox.jpeg" style="width: 100% ;" id="bb1" class="w3-container w3-opacity w3-animate-zoom" >
			 <div class="w3-container w3-pink w3-border w3-circle w3-quarter w3-margin-6" style="width: 5px; height: 30px ;margin: 5px;" onclick="jansena()"> </div>
			 <div class="w3-container w3-blue w3-border w3-circle w3-quarter w3-margin-6" style="width: 5px; height: 30px ;margin: 5px;" onclick="jansena1()"> </div>
			 <div class="w3-container w3-red w3-border w3-circle w3-quarter w3-margin-6" style="width: 5px; height: 30px ;margin: 5px;" onclick="jansena2()"> </div>

		</div>
		<!-- sidebar --> 
		<div class="w3-sidebar w3-bar-block w3-display-top-right w3-animate-left " style="height: 30% ; width: 13% ; display: none;" id="sidebarmenu">
			<button class="w3-button w3-bar-item w3-border w3-card-4 w3-teal" style="width: 100% ;font-size:1.5vw" onclick="hidemenu()">CLOSE &times</button>
			<a href="https://pnvsoft.com/digitalking/index.html#" class="w3-bar-item w3-button w3-border w3-card-4 w3-teal " style="width: 100% ;font-size:1.5vw">HOME</a>
			<a href="#" class="w3-bar-item w3-button w3-border w3-card-4 w3-teal" style="width: 100% ;font-size:1.5vw">NEXT</a>
			<a href="#" class="w3-bar-item w3-button w3-border w3-card-4 w3-teal" style="width: 100% ; font-size:1.5vw">BACK</a>
			<a href="cardindex.html" class="w3-bar-item w3-button w3-border w3-card-4 w3-teal" style="width: 100% ; font-size:1.5vw">Bussiness card</a>
		</div>
		<button class="w3-teal w3-card-4 w3-button w3-xlarge" id="sidebar" style="font-size: 1.5vw" onclick="showmenu()">☰</button>
		<div class="w3-bar w3-container  " id="pagination">
			<a href="#" class="w3-bar-item w3-button w3-blue " style="font-size: 1vw">&laquo</a>
			<a href="#" class="w3-bar-item w3-button w3-teal" style="font-size: 1vw">1</a>
			<a href="#" class="w3-bar-item w3-button w3-teal" style="font-size: 1vw">2</a>
			<a href="#" class="w3-bar-item w3-button w3-teal" style="font-size: 1vw">3</a>
			<a href="#" class="w3-bar-item w3-button w3-teal" style="font-size: 1vw">4</a>
		    <a href="#" class="w3-bar-item w3-button w3-teal" style="font-size: 1vw">5</a>
		    <a href="#" class="w3-bar-item w3-button w3-teal" style="font-size: 1vw">6</a>
			<a href="#" class="w3-bar-item w3-button w3-blue" style="font-size: 1vw">&raquo</a>
		</div>
         <!-- login form -->
         <script type="text/javascript">
         	function openmodel()
         	{
         		document.getElementById('model').style = "display:block";
         	}
         	function closemodel(){
         		document.getElementById('model').style = "display:none";
         	}
         </script>

         <!-- log in form -->
		<div class="w3-model w3-blue w3-mobile w3-responsive" id="model" style="width: 100%; z-index: 11">
			<div class="w3-model-content w3-card-4 w3-animate-zoom">
			<span class="w3-button w3-card-4 w3-red w3-display-topright w3-red" id="close" onclick="closemodel()" >&times</span>
			<img src="img_avatar4.png" alt="Avatar" style="width:30%" class="w3-circle w3-margin-top" id="formimg">
			 <form class=" w3-container">
			 	 <div class="w3-section w3-margin-top">
			 	 	<label><b>username</b></label>
			 	 	<input type="text" name="uname" class="w3-input w3-border w3-margin-top w3-card-4" placeholder="enter user name" required="">
			 	 	<label><b>password</b></label>
			 	 	<input type="text" name="upass" class="w3-input w3-border w3-margin-top w-card-4" placeholder="enter password" required="">
			 	 	<input type="submit" name="submit" class="w3-button w3-card-4 w3-green w3-border w3-margin-top" value="Log In" style="width: 100%" >
			 	 	<input type="checkbox" name="check" class="w3-check  w3-margin-top" checked="checked">Remember Me
			 	 </div>
			 	 <div class=" w3-margin-top w3-container w3-model-content w3-light-gray w3-padding-16" style="height: 15%">
			 	 	<span onclick="closemodel()" class="w3-button w3-card-4  w3-red">Cancel</span>
			 	 	<span onclick="signin()" class="w3-button w3-card-4  w3-green w3-center w3-middle" id="signin">New To Digi talking</span>
			 	 	<a href="#" class="w3-button w3-teal w3-border w3-card-4 w3-right">Forgot password</a>
			 	 	
			 	 </div>

			 </form>
		</div>
		</div>
		  <p id="date" class="w3-container w3-teal" style="font-size: 2vw"></p>
		    <script type="text/javascript">
		    	
		    	
		      function myfun()
		      {
		      	var d = new Date();
		    	var timer = d.toLocaleTimeString();
		    	document.getElementById("date").innerHTML = timer ; 
		    }
		      var clock = setInterval(myfun
		    		,1000);
		   
		    	
		    	
		    </script>
	</body>
</html>
