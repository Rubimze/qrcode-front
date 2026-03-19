# QR Code Generator - Web Interface

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![Vercel](https://img.shields.io/badge/Vercel-000000?style=for-the-badge&logo=vercel&logoColor=white)

Uma interface web simples e responsiva desenvolvida para consumir a **API REST de Geração de QR Codes**. 

Este projeto atua como o Front-end da aplicação, permitindo que os usuários insiram uma URL ou texto e recebam a imagem do QR Code gerada dinamicamente, que é hospedada em tempo real na nuvem (AWS S3).

🔗 **Acesse a aplicação online:** [https://qrcode-front-rust.vercel.app]

## ✨ Funcionalidades

* **Integração Assíncrona:** Consumo da API REST utilizando `fetch` no JavaScript (Vanilla JS).
* **Design Responsivo:** Interface *Mobile-First* que se adapta a telas de smartphones e desktops.
* **Feedback Visual:** Indicadores de carregamento ("Gerando...") e tratamento de erros na tela para uma melhor experiência do usuário.

## ⚙️ O Motor por trás da Tela (Back-end)

A inteligência de processamento, geração da matriz do QR Code e o upload automático para a nuvem não acontecem aqui. Todo esse fluxo é gerenciado por uma API construída em **Java 21, Spring Boot e AWS S3**.

👉 **[Clique aqui para ver o repositório do Back-end em Java](https://github.com/Rubimze/qr-code-generator)**

## 🚀 Como executar localmente

Como este projeto não utiliza frameworks complexos, rodá-lo localmente é extremamente simples:

1. Clone este repositório.
2. Abra a pasta do projeto.
3. Dê um duplo clique no arquivo `index.html` para abri-lo no seu navegador padrão.

> **⚠️ Nota:** Para que a geração funcione localmente, certifique-se de que a URL da API no arquivo `index.html` esteja apontando para o seu servidor na nuvem (Render) ou para o seu `http://localhost:8080` (caso o Back-end Java esteja rodando na sua máquina).
