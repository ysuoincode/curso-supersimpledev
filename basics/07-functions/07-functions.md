# Notes - Functions

## Definição de Functions
- Um recurso para reutilizarmos nosso código;

## Estrutura de uma function
<code>
function "nome da function"(){
  bloco de código
}
  
## Executando/chamando uma função 
'nome da fução'();

## Escopo
- Limita onde uma variável atua/existe;
- Define tbm se uma variável pode ser global ou local

### Variável global/pública
- pode ser utilizada por toda o código

## Return Statement
Nos permite retornar um valor para fora da function
Podemos retornar desde:
  - calculos :    return 2+2;
  - variáveis:    return variable1;
  - funções tbm:  return Math.random();
  - undefined:    return;

## Parametros
Pode-se dizer que são o oposto da Return Statement, pois coloca um valor de fora da função para dentro da função.

  function calculateTax(cost){

    console.log(cost * 0.1)
  }

  calculateTax(2000);

* Uma Função tbm pode passar mais de um parêmetro:

  function calculateTax(cost,taxPercent){
    console.log(cost * taxPercent)
  }

  calculateTax(2000,0.2)

* Também é possivél deixar valores setados por padrão

  function calculateTax(cost,taxPercent = 0.1){
      console.log(cost * taxPercent)
    }

    calculateTax(2000,0.2)
