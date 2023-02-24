<html>
<head>
<title>JS01_Concatenacao.html</title>
<meta http-equiv="Content-Type" content="text/html; charset=iso-8859-1">
<meta http-equiv="Content-Type" content="text/html; charset=utf-8">
</head>

<body>

<h3> Programa de boas vindas com concatenacao de campos!</h3>

<!-- Definição de Formulario -->

<form name="FormConcatena" action="" method="post">

      Digite o nome......................: <input type="text" name="f_nome"/><p></p>
      Digite o sobrenome.........: <input type="text" name="f_sobrenome" /><p></p>
      <input type="button" name="btn_concatena" value="Concatenar" onclick="concatena()"/>
      <input type="reset" name="btn_cancela" value="Cancelar"/>

</form>

<!-- Definição do codigo JavaScript -->
<script language="JavaScript">
<!--
      /* Objetivo: Capturar nome e sobrenome do usuario, concatenar (juntar) os campos e apresentar uma saudação personalizada
Elemento de Entrada: Metodo Form do objeto do document
Elemento de Saida>  Metodo alert do objeto window */
/* Definição de variaveis */
var js_nome;
var js_sobrenome;
var js_nomecompleto;
/* Entrada de Dados */
function concatena() {
      js_nome = document.FormConcatena.f_nome.value;
      js_sobrenome = document.FormConcatena.f_sobrenome.value;
/* processamento de dados */
js_nomecompleto = js_nome + ' ' + js_sobrenome;
/* Saidade de Dados */
window.alert('Olá ' + js_nomecompleto);
}
//-->
</script>
</body>
</html>
