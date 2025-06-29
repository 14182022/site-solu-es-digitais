# Soluções Digitais Inteligentes

Bem‑vindo ao repositório **Soluções Digitais Inteligentes**!  
Aqui você encontra todo o código-fonte do site estático hospedado via **GitHub Pages**.

---

## 📄 Visão Geral

Este site apresenta nossos principais produtos de automação e tecnologia, incluindo o **Bot de Análise Binance**. Ele foi construído somente com **HTML5** e **CSS3**, sem dependências externas além de:

- Google Fonts (fonte Inter)  
- Um vídeo demonstrativo `bot-demo.mp4`  
- (Opcional) Imagem de pôster do vídeo `poster-bot.jpg`  

> **Demonstração online:** será exibida automaticamente após você habilitar o GitHub Pages nas configurações do repositório.

---

## 🌐 Publicação no GitHub Pages

1. Faça *push* de **todos** os arquivos para a branch `main` (ou `gh-pages`).  
2. Acesse **Settings ▸ Pages**.  
3. Em **Source**, escolha a branch que contém o site e clique em **Save**.  
4. Aguarde alguns segundos. Seu site ficará disponível em:<br>
   `https://<seu-usuario>.github.io/<nome-do-repo>/` *(ou apenas `<seu-usuario>.github.io` se o repositório se chamar assim).*

---

## 📂 Estrutura de Pastas

```
.
├── index.html          # Página principal
├── bot-demo.mp4        # Vídeo demonstrativo (até 100 MB)
├── poster-bot.jpg      # Miniatura opcional do vídeo
└── README.md           # Este arquivo
```

Se quiser organizar melhor:

```
.
├── index.html
├── assets/
│   ├── video/ bot-demo.mp4
│   └── img/   poster-bot.jpg
└── README.md
```

Lembre-se de ajustar o caminho no atributo `src` do `<video>` se mover o arquivo.

---

## 🔧 Customização Rápida

- **Título do site:** altere a tag `<title>` dentro do `<head>`.  
- **Meta description (SEO):**
  ```html
  <meta name="description" content="Bots, automação e tecnologia para resultados reais">
  ```
- **Contato e links:** edite as seções `WhatsApp`, `Hotmart`, etc.  
- **Cores:** todos os estilos estão embutidos no `<style>` do `index.html`; você pode migrar para um arquivo `style.css` se preferir.

---

## 🎥 Otimização do Vídeo

O GitHub impõe limite de **100 MB** por arquivo. Para arquivos grandes use:

```bash
ffmpeg -i bot-demo.mp4 -vcodec libx264 -crf 26 bot-demo-smaller.mp4
```

> Quanto maior o valor de **CRF** (0–51), menor o arquivo e ligeiramente menor a qualidade.

---

## 📜 Licença

Distribuído sob a licença **MIT** – veja o arquivo `LICENSE` para mais detalhes.

---

**Feito com 💙 por Maicko Massena**  
Para suporte, envie uma mensagem para [WhatsApp](https://wa.me/5548996184665).
