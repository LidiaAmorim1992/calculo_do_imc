<meta charset="UTF-8">

<script>

    function pulaLinha() {

        document.write("<br>");
        document.write("<br>");
}

    function mostra(frase) {

        document.write(frase);
        pulaLinha();
}

    function calculaImc(altura, peso) {

        return peso / (altura * altura);
}


var nome = prompt("Qual é o seu nome?")
var alturaInformada = prompt(nome + ", por favor informe sua altura");
var pesoInformado = prompt(nome + ", agora informe seu peso");

var Imc = calculaImc(alturaInformada, pesoInformado);

mostra(nome + ", o seu Imc é " + Imc);


if(Imc < 18.5){
mostra("O seu Imc está abaixo do recomendado.");
}
if(Imc >35){
mostra("O seu Imc está acima do recomendado.");
}
if(Imc <=35){
mostra("O seu Imc está excelente!");
}


</script>
