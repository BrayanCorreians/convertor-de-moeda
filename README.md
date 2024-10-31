## 𝑪𝒐𝒏𝒗𝒆𝒓𝒔𝒐𝒓 𝒅𝒆 𝒎𝒐𝒆𝒅𝒂𝒔


# License
>![](https://img.shields.io/badge/license-%20Escola%20Marista%20Ir.%20Ac%C3%A1cio-black) ![](https://img.shields.io/badge/version-0.3-white)
 
## Descrição do Projeto
Este projeto foi desenvolvido na aula de PWI (Programação Web 1), ministrada pelo professor [Leonardo Rocha](https://github.com/leonardossrocha). O objetivo do projeto é aprender a converter valores de moedas, ainda de forma simples, porém logo esse projeto terá uma continuação mais aprimorada juntamente com o consumo de API.
 
![tela do sistema](projeto.png)
 
## Funcionalidades do website
 
✔️ Verificação de Campos Obrigatórios;
 
✔️ Resetar o formulário;
 
✔️ Preencher Formulário;
 
✔️ Converter moeda;
 
✔️ Inserir valor;
 
✔️ Resultado do valor inserido;
 
✔️ Definir Taxas de câmbio;

✔️ Definir taxas de câmbio manualmente
 
 
# Funcionalidades JS utilizadas🔧
1- Recuperação de valores de entrada: Recupera os valores inseridos pelo usuário nos campos do formulário
 
2- Definição de taxas de câmbio: Define um objeto de taxas de câmbio fixas exchangeRates que contém as taxas de conversão entre diferentes moedas (USD, BRL e EUR).
 
3- Conversão de moeda: converte a moeda, deMoeda, paraMoeda.
 
4- Exibição do resultado: Atualiza o conteúdo de texto do elemento com o id "result" para exibir o valor convertido, arredondado para duas casas decimais usando toFixed(2), juntamente com o símbolo da moeda convertida.
 
# Inserir valor de taxa de câmbio
~~~ Javascript
document.getElementById ('currency-converter').addEventListener('submit', function(event){
    event.preventDefault();
 
    // Obter valores de entrada informados pelo usuário
    const valor = parseFloat(document.getElementById('amount').value);
    const daMoeda = document.getElementById('daMoeda').value;
    const paraMoeda = document.getElementById('paraMoeda').value;
~~~
 
# Definição de taxas de câmbio
~~~ Javascript
const exchangeRates = {
        USD: { BRL: 5.70, EUR: 0.93 },
        BRL: { USD: 0.18, EUR: 0.16 },
        EUR: { USD: 1.08, EUR: 6.16 }
 
    };
~~~
 
~~~ Javascript
// Conversão simples de moeda
    let valorConvertido;
    if(daMoeda === paraMoeda){
        valorConvertido = valor;
    }else{
        valorConvertido = valor * exchangeRates[daMoeda][paraMoeda];
    } 
~~~

## COMO USAR
1. Selecione a moeda de origem e destino BRL, EUR, USD E EUR.
2. Insira o valor que deseja converter e tera o valor convertido.

 
 
 
## Tecnlogias utilizadas 🔧
![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)
![Visual Studio Code](https://img.shields.io/badge/Visual_Studio_Code-0078d7?style=for-the-badge&logo=visual-studio-code&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=black)