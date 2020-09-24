#  Interrompendo o submit de um formulário

Para perguntar ao usuário se quer continuar com a submissão do formulário, podemos usar a seguinte lógica.



~~~javascript
const form = document.querySelector("#form")

// escuta o evento submit
form.addEventListener("submit", function(event) {
    // o método confirm exibe uma janela com os botões 'OK' e 'Cancelar'
    const confirmation = confirm('Deseja submeter o formulário?')

    if (!confirmation) {
        // o preventDefault cancela o evento, nesse caso o submit
        event.preventDefault()
    }
})
~~~