# Markdown

# Aprendendo Markdown
## Aprendendo Markdown

Aplicando **Negrito** em Markdown

Aplicando *Itálico* em Markdown

>Texto em caixa
>
>Exemplo

# Calculadora de Fatorial e Número Primo
``` HTML
<!DOCTYPE html>
<html lang="pt-BR">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Fatorial e Número Primo</title>
</head>

<body>
    <h2>Calculadora de Fatorial e Verificador de Número Primo</h2>
    <label for="numero">Digite um número:</label>
    <input type="number" id="numero">
    <button onclick="calcular()">Calcular</button>
    <p id="resultado"></p>
    <script>

        //Função para calcular o fatorial
        function calcularFatorial(n) {
            if (n === 0) {
                return 1;
            } else {

                return n * calcularFatorial(n - 1);
            }
        }

        //Função para verificar se o numero é primo
        function verificarNumeroPrimo(numero) {
            if (numero <= 1) {
                return false;
            }
            for (let i = 2; i < numero; i++) {
                if (numero % i === 0) {
                    return false;
                }
            }
            return true;
        }

        //Função calcular
        function calcular() {
            let numero = parseInt(document.getElementById("numero").value);
            let fatorial = calcularFatorial(numero);
            let primo = verificarNumeroPrimo(numero);
            document.getElementById("resultado").innerHTML =
                "O fatorial de " + numero + " é " + fatorial + "<br>" +
                "O número " + numero + (primo ? " é primo." : " não é primo.");
        }
    </script>
</body>

</html>

```
# Respostas
1. Após a formatação e a adição de comentários, o código se torna mais legível e compreensível.

2. A rastreabilidade permite a identificação do código desde o início até o desenvolvimento de cada parte do código, compreendendo as mudanças feitas ao longo do tempo.

3. Comentários claros: Explicar o que o código faz, especialmente em trechos complexos.
Estruturação adequada: Organizar o código de forma lógica e com nomes de variáveis e funções significativos.

4. O Markdown é uma linguagem de marcação simples e amplamente utilizada para documentação. Ele facilita a criação de documentos legíveis e bem formatados.

5. Garantem que todos os desenvolvedores sigam o mesmo estilo, tornando o código mais fácil de entender e modificar. A padronização também torna o código mais previsível e ajuda a identificar rapidamente problemas de lógica ou design.
