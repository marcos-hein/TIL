# 📃️ Como espalhar dados de um objeto JavaScript

Com `...pessoa` é feito um espalhamento dos dados contidos dentro do objeto `pessoa`. Passando uma chave específica, é possível atualizar o valor, como no exemplo abaixo.  

~~~javascript
let pessoa = {
  "nome": "João",
  "idade": 26,
  "altura": 178
}

pessoa = {
  ...pessoa,
  idade: 21,
}

console.log(pessoa)

/*
Resultado:
{
  altura: 178,
  idade: 21,
  nome: "João"
}
*/
~~~