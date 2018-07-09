<!DOCTYPE html>
<html lang="pt-br">
	<head>
		<meta charset="utf-8">
		<title>Curriculum</title>
		<script type="text/javascript">
			function validar_form_contato(){
				var nome = formcontato.nome.value;
				var endereço = formcontato.endereço.value;
				var idade = formcontato.idade.value;
				var objetivo = formcontato.objetivo.value;
				var formação = formcontato.formação.value;
				
				if(nome == ""){
					alert("Campo nome é obrigatorio");
					formcontato.nome.focus()
					return false;}
				if(endereço == ""){
					alert("Campo endereço é obrigatorio");
					formcontato.endereço.focus();
					return false;}
				if(idade == ""){
					alert("Campo Idade é obrigatorio");
					formcontato.idade.focus();
					return false;}
				if(objetivo == ""){
					alert("Campo objetivo é obrigatorio");
					formcontato.objetivo.focus();
					return false;}
				if(formação == ""){
					alert("Campo formação é obrigatorio");
					formcontato.formação.focus();
					return false;}
				 
				
			}
		</script>
	<head>
	<body>
		
			
        <fieldset>
             <h1>Gerador de Curriculum</h1>
    		<form name="formcontato" method="POST" action="curriculum1.php">
        		<label for="nome"></label><br>
        		Nome:<input type="text"name="nome" placeholder="digite seu nome"/><br>
            
                <label for="endereço"> </label><br>
        		Endereço:<input  type ="text" name="endereço" placeholder="digite seu endereço"/><br>

                
                <label for="idade"> </label><br>
        		Idade:<input name="idade" type ="text" placeholder="digite sua Idade"/><br>
                
                <label for="objetivo"> </label><br>
        		Objetivo:<input name="objetivo"  type ="text" placeholder="digite seu objetivo profissinal"/><br>
                
                <label for="formação"></label><br>
        		Formação:<input name="formação" type ="text" placeholder="digite sua Formação"/><br>
                
                <label for="Habilidades"></label><br>
        		Habilidades:<input name="habilidades"  type ="text" placeholder="digite suas Habilidades"/><br><br>

                
        		
    	         
          	   
                 <div class="pre-spoiler"><br />
                  Experiencias:<input id="xs" value="mais" style="margin-left: 10px; padding: 0px; width: 80px; " onclick="if (this.parentNode.parentNode.getElementsByTagName('div')[1].getElementsByTagName('div')[0].style.display != '') { this.parentNode.parentNode.getElementsByTagName('div')[1].getElementsByTagName('div')[0].style.display = '';this.innerText = ''; this.value = 'menos'; } else { this.parentNode.parentNode.getElementsByTagName('div')[1].getElementsByTagName('div')[0].style.display = 'none'; this.value = '+';}" type="button"> </div><br /> 
                 <div><br />
	                   <div class="spoiler" style="display: none;"><br />  <label for="Habilidades"></label><br>
	        		   Experiêcias Profissionais:<input name="habilidades"  type ="text" placeholder=""/><br><br>
	        		   </div><br />
	        		    <input type="submit"  value="enviar" onclick="return validar_form_contato()">
                       </div>
                       
	    	
	                   
	        </form>	
	       
        </fieldset>
             
	</body>
	</html>
