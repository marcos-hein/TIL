# 📃️ Como espalhar dados de um objeto JavaScript


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
~~~