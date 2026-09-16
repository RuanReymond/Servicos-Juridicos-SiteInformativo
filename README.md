# Jean Bruno Advogados Associados — Site Institucional

Site institucional simples e responsivo para o escritório Jean Bruno Advogados Associados. Não usa banco de dados nem back-end: é HTML, CSS e JavaScript puros, prontos para hospedar em qualquer serviço.

## Arquivos

```
jean-bruno-site/
├── index.html   -> estrutura e conteúdo da página
├── styles.css   -> todo o visual (cores, layout, responsividade)
└── script.js    -> efeito de revelar o conteúdo ao rolar a página
```

Os três arquivos precisam ficar **na mesma pasta** e com esses nomes, pois o `index.html` referencia os outros dois:

```html
<link rel="stylesheet" href="styles.css">
...
<script src="script.js"></script>
```

## Como visualizar localmente

Basta abrir o arquivo `index.html` duas vezes no navegador (duplo clique), ou clicar com o botão direito → "Abrir com" → navegador de sua preferência. Não é necessário instalar nada.

## Seções do site

- **Cabeçalho** — logo, menu de navegação e botão de WhatsApp fixo
- **Início (hero)** — chamada principal com botões "Agendar atendimento" e "Falar pelo WhatsApp"
- **Sobre** — apresentação do escritório e diferenciais em destaque
- **Diferenciais** — grade com os 6 pontos fortes do escritório
- **Avaliações** — nota do Google e depoimentos de clientes
- **Localização** — endereço, botão "Como chegar" e mapa incorporado (Google Maps)
- **Horário** — banner "Aberto 24 horas"
- **Contato** — atalhos para WhatsApp, rota no mapa, e-mail e agendamento
- **Rodapé** — resumo de contato e endereço
- Botão flutuante de WhatsApp visível em todas as páginas/seções

## O que personalizar

| O que mudar | Onde está | Como encontrar |
|---|---|---|
| Número de WhatsApp | `index.html` | busque por `5592981329379` (aparece em vários links `wa.me`) |
| E-mail de contato | `index.html` | busque por `reymondruan4@gmail.com` |
| Endereço e mapa | `index.html`, seção `id="localizacao"` e rodapé | troque o texto do endereço e o parâmetro do link do Google Maps |
| Textos e depoimentos | `index.html` | edite diretamente o texto dentro das tags `<p>`, `<h1>`, `<h2>`, etc. |
| Cores | `styles.css`, bloco `:root` no topo do arquivo | variáveis `--navy`, `--gold`, `--cream`, etc. |
| Fontes | `index.html` (link do Google Fonts) e `styles.css` (`font-family`) | atualmente usa Playfair Display + Inter |

> Dica: para trocar o número de WhatsApp, atualize **todas** as ocorrências de `5592981329379` no `index.html` (são vários botões: cabeçalho, hero, contato, rodapé e o botão flutuante).

## Como publicar o site online

Qualquer opção abaixo funciona, já que o site é 100% estático:

1. **Hospedagem gratuita e simples**: Netlify, Vercel ou GitHub Pages — basta arrastar a pasta com os 3 arquivos.
2. **Hospedagem tradicional (cPanel/Hostinger/etc.)**: envie os 3 arquivos por FTP para a pasta `public_html` (ou equivalente).
3. **Domínio próprio**: após hospedar, aponte o domínio do escritório para o serviço escolhido.

## Requisitos

- Nenhum. Não precisa de servidor, banco de dados ou instalação de dependências.
- Funciona em qualquer navegador moderno (Chrome, Firefox, Edge, Safari) e é responsivo para celular, tablet e desktop.
