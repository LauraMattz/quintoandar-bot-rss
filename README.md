# 🤖 QUINTOANDAR APARTMENT WATCHER BOT

Receba automaticamente os melhores apartamentos do QuintoAndar direto no seu Telegram com um fluxo simples e eficiente usando **RSS.app**, **n8n**, e **JavaScript**.

![Preview](assets/preview.png)

---

## 🚀 Visão Geral

Este projeto monitora imóveis para aluguel (ex: 2 quartos na Santa Cecília - SP) no site do [QuintoAndar](https://www.quintoandar.com.br) e envia os 5 melhores achados para o Telegram — tudo isso automaticamente!

> 💡 Ideal para quem quer estar sempre atualizado com os novos imóveis, sem precisar visitar o site todos os dias.

---

## 🛠️ Tecnologias Usadas

* [RSS.app](https://rss.app) – transforma páginas HTML em feeds RSS
* [n8n](https://n8n.io) – plataforma de automação low-code
* JavaScript – para extração e formatação de dados
* Telegram Bot API – envio automático das mensagens formatadas

---

## ⚙️ Como Funciona

1. **📰 RSS Feed**
   Criado com RSS.app a partir da URL de listagem do QuintoAndar.

2. **🌐 HTTP Request**
   Captura o HTML completo da página com um node do tipo `HTTP Request`.

3. **🧠 Código JavaScript**
   Usa `Code Nodes` para extrair os dados principais:
   `título`, `endereço`, `aluguel`, `metragem`, `quartos` e `vagas`.

4. **🎨 Formatação**
   Seleciona os 5 imóveis com mais informações completas e gera uma mensagem clara e atraente usando emojis.

5. **📤 Envio para o Telegram**
   A mensagem final é enviada automaticamente para seu bot ou grupo no Telegram.

---

## ✨ Exemplo de Saída

```markdown
📢 Achei 18 novos apartamentos!
🗕️ Atualizado em: 23/05/2025, 19:12:03

🔍 Veja os 5 destaques:

🏡 Rua Doutor Albuquerque Lins, Santa Cecilia · São Paulo  
📀 Tamanho: 140 m²  
✨ 🛌 Quartos: 3  
🚗 Vagas: 2  

🏢 Avenida General Olímpio da Silveira, Santa Cecília · São Paulo  
📀 Tamanho: 70 m²  
✨ 🛌 Quartos: 2  

🏠 Rua Rosa E Silva, Santa Cecília · São Paulo  
📀 Tamanho: 55 m²  
✨ 🛌 Quartos: 2  
🚗 Vagas: 1  
...
```

---

## 👩‍💼 Feito por Laura Mattos

Feito com ☕, automação e vontade de fugir de aluguel caro.

Contribuições são muito bem-vindas!
Abra uma issue, mande um PR ou compartilhe seu fork com outros fluxos criativos! 💡
