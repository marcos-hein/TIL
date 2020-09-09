# 📌️ Filtrar elemento de um array

O método `filter()`chama uma função callback para cada elemento do array e constrói um novo array com todos os valores que retornaram `true`.

Por exemplo:

~~~javascript
const array = [1, 2, 3, 4, 5]
const queroFiltrar = 3

const arrayFiltrado = array.filter(function(numero) {

  // retorna true se o número do array é diferente de queroFiltrar
  return queroFiltrar != numero
})

console.log(arrayFiltrado)

// resultado: [1, 2, 4, 5]
~~~