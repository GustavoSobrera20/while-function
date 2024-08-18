(1) - Imprima a tabuada do 5 (5 x 1 até 5 x 10) utilizando um laço de repetição

    function tabuada_5 (contador){
    contador =1

    while (contador <= 10 ){
 
    console.log ( '5 x ' + contador + '=' + contador * 5)
    contador++
    }
    } 
    tabuada_5()

(2) - Calcule a soma de todos os números de 1 a 100 utilizando um laço de repetição

    function soma_ate_100(contador, soma){
    contador = 1 
    soma = 0 
   
    while (contador <= 100){
          soma += contador
     contador++
    }
    return soma
    }
    console.log (soma_ate_100())


(3) - Calcule a soma dos dígitos de um número fornecido pelo usuário utilizando um laço de repetição.

    function somaDigitosUsuario() {
    let resultado = 0;

    while (true) {
        let numero_usuario = prompt("Digite um número (ou 'soma' para resultado): ");
        if (numero_usuario === "soma") {
            break;
        }
        let numero = parseInt(numero_usuario, 10);
        
        if (!isNaN(numero)) {
           
            resultado += numero;
        } else {
           
            alert("Entrada inválida. Por favor, digite um número.");
        }
    }

    
    
    alert("A soma dos números digitados é: " + resultado);
    }

    somaDigitosUsuario();

## o porque do ===

O operador === é conhecido como o operador de igualdade estrita em JavaScript. Ele é usado para comparar dois valores, garantindo que ambos sejam do mesmo tipo e tenham o mesmo valor.
Resumo
Use === para garantir uma comparação exata onde o tipo e o valor devem corresponder exatamente

-------------------------------------------------------------------------------------------------------------------------------------------------
(4) - Imprima os primeiros 10 números da sequência de Fibonacci utilizando um laço de repetição.


    function Fibonacci(n) {
    let a = 0, b = 1;
    
    while (n-- > 0) {
        console.log(a); 
        [a, b] = [b, a + b]; 
    }
    }

    Fibonacci(11);

-------------------------------------------------------------------------------------------------------------------------------------------------
## explicando o porque do [a, b] = [b, a + b]

[b, a + b]: Cria um array temporário com dois elementos:

O primeiro elemento é o valor atual de b.
O segundo elemento é a soma de a e b.
[a, b]: A desestruturação faz com que os valores no array temporário sejam atribuídos às variáveis a e b, respectivamente.

a recebe o valor que estava em b.
b recebe o valor da soma de a e b (ou seja, o próximo número na sequência de Fibonacci).

-------------------------------------------------------------------------------------------------------------------------------------------------
