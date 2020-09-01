# 📅️ Formatando datas para formulários

Já precisou devolver uma data para um formulário HTML?

É necessário enviar a data no seguinte formato: aaaa/mm/dd.

Como faz? Abaixo o código em JavaScript.


~~~javascript
function(timestamp){
    const date = new Date(timestamp)

    const year = date.getFullYear()
    const month = `0${date.getMonth() + 1}`.slice(-2)
    const day = `0${date.getDate() + 1}`.slice(-2)

    return `${year}-${month}-${day}`
}
~~~