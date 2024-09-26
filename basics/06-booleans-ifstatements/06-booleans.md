# Notes of Booleans

## Truthy and Falsy Values
- É mais fácil destacar os flasy values, pois são somente alguns e os que não pertencem a essa lista de falsy values são truthy values.

- Lista de Falsy Values:
  - false
  - 0
  - ''
  - NaN
  - undefined
  - null

* Qualquer outro valor fora estes citados acima serão truthy values! 

### Para que se usam os false values:
  - Abreviar o código, ex:

    const cartQuantity = 5;

      if (cartQuantity > 0) {
        console.log('cart has products')
      }

      (cartQuantity > 0) é a mesma coisa que (cartQuantity)
      onde se cartQuantity for maior que 0 será verdade, e se não for será false.  

## Shortcuts for If-Statements:

### Tenary Operator ?:

   true     ? 'truthy' : 'falsy'
    |            |          |
  condition ?   if{}   :  else{}

Exemplo:

const result = true ? 'truthy' : 'falsy';
console.log(result); //will show truthy

const result = 0 ? 'truthy' : 'falsy';
console.log(result); //will show falsy


### Guard Operator &&

value1 && value2

- Caso o valor1 ja seja definido como false, automaticamente para o codigo e não avança nem para parte direita do operador. Ex:

  const message = false && 'hello';
  console.log(message); //system will print false

- Neste caso, message recebe false como seu valor e ira ignorar o valor a direita do operador.

- Porém se o value1, for um valor verdadeiro:

  const message = 5 && 'hello'
  console.log(message); //system will print 'hello'

- Basicamente o valor é dado como verdadeiro, assim o value2 será atribuido a variável 

- Isso serve como uma shortcut de: 
        if (condition){
          message = 'hello';
        }

### Default Operator ||

  value1 || value2

  const currency = 'EUR'|| 'USD';

  - Serve como uma shortcut para:
    let currency;

    if (!condition){
      currency = 'USD';
    }