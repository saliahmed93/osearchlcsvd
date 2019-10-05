<!DOCTYPE html>
<html>
	<head>
		<title></title>
		<meta name="viewport" content="width=device-width, initial-scale=1">
		<link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/4.3.1/css/bootstrap.min.css">
		<script src="https://ajax.googleapis.com/ajax/libs/jquery/3.4.1/jquery.min.js"></script>
		<script src="https://cdnjs.cloudflare.com/ajax/libs/popper.js/1.14.7/umd/popper.min.js"></script>
		<script src="https://maxcdn.bootstrapcdn.com/bootstrap/4.3.1/js/bootstrap.min.js"></script>
		<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.7.0/css/font-awesome.min.css">
		<link rel="stylesheet" type="text/css" href="css/style.css">
		<style type="text/css">
			
		</style>
		
	</head>
	<body>
		<div class="container-fluid" >
			<div class="row mytoprow" >
				<div class="col-sm-12">
					<nav class="navbar navbar-expand-sm bg-white
						justify-content-end">
						
						<button class="navbar-toggler this" type="button" data-toggle="collapse" data-target="#collapsibleNavbar">
						<span class="fa fa-bars"></span>
						</button>
						<ul  class="navbar-nav collapse navbar-collapse justify-content-end" id="collapsibleNavbar" style="">
							
							<li class="nav-item" >
								<a class="nav-link" href="#" title="">HomePage</a>
							</li>
							<li class="nav-item" >
								<a class="nav-link" href="#" title="">Page</a>
							</li>
							<li class="nav-item" >
								<a class="nav-link" href="#" title="">Page</a>
							</li>
							<li class="nav-item" >
								<a class="nav-link" href="#" title="">Page</a>
							</li>
							<li class="nav-item" >
								<a class="nav-link" href="#" title="">Page</a>
							</li>
							<li class="nav-item" >
								<a class="nav-link" href="#" title="">Page</a>
							</li>
						</ul>
						
					</nav>
				</div>
			</div>
			<div class="container">
				<div class="card">
					<img src="img/logo.png">

					<div class="input-group">
							<input type="text" class="" id="textInput" placeholder="Search for car ratings">
							<div class="input-group-append" style="">
								<button type="button" id="submitBtn" class="btn btn-primary">
									<span class="fa fa-search"></span>
								</button>
							</div>
						</div>
				</div>


				
			</div>
			<div class="end">
				<h5>Copyright © 2019. All Rights Reserved.</h5>
				</div>
		<!--	<div class="last_row">
				<h6>Made in Swizterland-Search Project all right reserved sample text</h6>
			</div>-->

			
			
			<script type="text/javascript">
			
			// Get input element
			const textInput = document.getElementById('textInput');
			// Array containing values form which we want to search
			// insert lowecase letters here in this array
			// YOu can edit your list here.
			const arr = [
			'hbrehman',
			'adnan',
			'walid',
			'wosno.com'
			];
			// get Btn
			const btn = document.getElementById('submitBtn');
			// Event listener...
			btn.addEventListener('click', () => {
			const textValue = textInput.value.toLowerCase();
			var indicator = false;
			for (let c of arr) {
			if (c == textValue) {
			//alert('Domain is valid');
			
			indicator = true;
			window.location.assign("#");
			break;
			}
			}
			if (!indicator)
			//alert('Not exists');
			window.location.assign("#");
			});
			</script>


			<script>

    
    var h = window.innerHeight;
    $(".container").css({"height":h});

    $('#submitBtn').click(function () {
       let search = $('#textInput').val();
       if(search != '') {
           window.location.href = "search_result?search="+search;
       }
    });

</script>
			
			
		</div>
	</body>
</html>