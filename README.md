# SL Veículos — Landing Page

## Como usar
Abra `index.html` em qualquer navegador. Não precisa de servidor, build ou instalação —
é um site estático em HTML/CSS/JS puro.

## Estrutura

```
sl-veiculos/
├── index.html        → página completa (estrutura, estilos e scripts)
└── hero-photo.jpg     → foto de fundo do Hero (PLACEHOLDER — ver abaixo)
```

## ⚠️ Antes de publicar o site

1. **Troque `hero-photo.jpg`**: a imagem atual é uma Ferrari usada apenas como
   referência visual temporária. Substitua por uma foto real da fachada/showroom
   da SL Veículos, mantendo o mesmo nome de arquivo (`hero-photo.jpg`) ou
   atualizando a referência dentro de `index.html` (busque por `hero-photo.jpg`).

2. **Fotos dos veículos**: dentro de `index.html`, procure o array `const vehicles`
   no `<script>` final. Cada veículo tem um campo `image: null` — troque por
   `image: 'nome-do-arquivo.jpg'` (e coloque o arquivo na mesma pasta) assim que
   tiver as fotos reais de cada carro. Enquanto `image` for `null`, o card mostra
   um ícone de placeholder.

3. **Preços e quilometragem**: nenhum valor foi inventado. Preencha o campo
   `price` de cada veículo no array `vehicles` conforme os dados reais chegarem.

4. **WhatsApp**: confira a constante `CONFIG.whatsappNumber` no `<script>` —
   está com o telefone fixo (15) 3226-1930. Troque por um número com WhatsApp
   Business ativo se for diferente.

## Dependências (via CDN, sem instalação)
- GSAP + ScrollTrigger (animações de scroll)
- hls.js (vídeo do Hero em streaming)
- Google Fonts: Inter + Instrument Serif

## Hospedagem
Como é um site 100% estático, pode subir direto em qualquer serviço simples de
hospedagem (Netlify, Vercel, GitHub Pages, cPanel, etc.) — basta enviar os dois
arquivos (`index.html` e `hero-photo.jpg`) para a mesma pasta.
