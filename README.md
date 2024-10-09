# Calculadora IMC (Índice de Massa Corporal)

## Sobre o Projeto

Este projeto é uma calculadora simples de IMC (Índice de Massa Corporal) desenvolvida com HTML, CSS e JavaScript. A calculadora permite que o usuário insira seu nome, altura e peso para calcular seu IMC e exibir o resultado em tempo real. Além de ser uma ferramenta útil para medir o IMC, este projeto também demonstra minha capacidade de criar interfaces de usuário simples e eficazes, integrando lógica de programação para fornecer uma experiência funcional e amigável.

## Funcionalidades

- **Entrada de dados**: O usuário pode inserir seu nome, altura e peso.
- **Cálculo automático**: Ao clicar no botão "Calcular", o IMC é calculado e exibido na página.
- **Responsividade**: A interface foi projetada para ser amigável em diferentes tamanhos de tela, sendo utilizável tanto em dispositivos móveis quanto em desktops.

## Tecnologias Utilizadas

Este projeto foi desenvolvido utilizando as seguintes tecnologias:

- **HTML5**: Para a estruturação do conteúdo.
- **CSS3**: Para estilização e layout responsivo.
- **JavaScript**: Para a lógica do cálculo de IMC e manipulação do DOM.
- **Next.js**: (caso aplicável) Para gerenciamento de estados e reatividade na interface.
  
## Código de Destaque

O projeto utiliza JavaScript para manipular os valores inseridos e calcular o IMC, conforme o código abaixo:

```javascript
document.getElementById('calcular').addEventListener('click', function() {
    const altura = document.getElementById('altura').value;
    const peso = document.getElementById('peso').value;
    const imc = (peso / (altura * altura)).toFixed(2);
    document.getElementById('resultado').textContent = `Seu IMC é: ${imc}`;
});
