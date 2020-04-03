<html>
<head>

	<meta http-equiv="Content-Type" content="text/html; charset=utf-8">
	<title>Formularz</title>
		<style>
		body
		{
		background-color: aqua;
		}
		</style>
		<script>
		<script>
        function sprawdz(){
            var fullName = document.getElementById("imie").value;
            if (fullName.match(/^[A-Z][a-z]+ [A-Z][a-z]+$/)){
                document.getElementById("imie").style.backgroundColor='red';
            }	
			var fullName = document.getElementById("nazwisko").value;
            if (fullName.match(/^[A-Z][a-z]+ [A-Z][a-z]+$/)){
                document.getElementById("nazwisko").style.backgroundColor='red';
            }	
			var kod = document.getElementById("kod").value;
			if (kod.match(/[0-9]{2}-[0-9]{3}/)){
                document.getElementById("kod").style.backgroundColor='red';
				}
			var city= document.getElementById("Miasto").value;
            if (city.match(/^([A-Z][a-z]+[A-Z][a-z])|( [A-Z][a-z])+$/)){
                document.getElementById("Miasto").style.backgroundColor='red';
			}
			var mail = document.getElementById("email").value;
            if (mail.match(/^([a-z]+@[a-z]+\.pl)|([a-z]+@[a-z]+\.[a-z]+.pl)/)){
                document.getElementById("email").style.backgroundColor='red';
			}
			var phone = document.getElementById("telefon").value;
            if (phone.match(/[0-9]{3}-[0-9]{3}-[0-9]{3}/)){
                document.getElementById("telefon").style.backgroundColor='red';
			}
			
			
				
        }
    </script>
		

		
		
		
		
		
		</script> 
</head>
<body>
<div id="body">
</div>

<form action="" method="post">

  <div>
				<br><br><br>
  <center> Imię:<br />

	<center><input name="imie" value="" /><br />
	
	<center> Nazwisko:<br />

	<center><input name="nazwisko" value="" /><br />

	<center>  Miasto:<br />

	<input name="Miasto" value="" /><br />
	
	 Kod-Pocztowy:<br />

	<input name="kod" value="" /><br />
	
	
	<center> Adres e-mail:<br />

	<center> <input name="email" value="" /><br /> 
	
	 Telefon:<br />

	<input name="telefon" value="" /><br />

  
  
	<button onclick="sprawdz()">sprawdz</button>
  
</body>


</html>
