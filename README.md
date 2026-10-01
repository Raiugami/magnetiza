# Magnetiza | Ímãs personalizados e impressão 3D

Site institucional da **Magnetiza**, marca de **Alessandra Brassal** que faz ímãs de geladeira personalizados de 50 mm e peças de decoração em impressão 3D, para festas, empresas e eventos, com envio para todo o Brasil.

- **Cliente:** Alessandra Brassal
- **Site publicado:** https://magnetiza.imaguiar.com.br/
- **Instagram:** [@wagnetiza.oficial](https://www.instagram.com/wagnetiza.oficial/)
- **Loja:** [Shopee](https://s.shopee.com.br/gPQTmjNee)

## Sobre o projeto

Página única (one-page), responsiva, para apresentar os produtos e levar o visitante ao pedido de orçamento. O botão de orçamento fica fixo na tela e leva ao direct do Instagram; para usar WhatsApp, basta preencher o número no script do final do `index.html`.

Seções: apresentação, o que fazemos (ímãs, impressão 3D, festas, empresas e eventos), detalhes, galeria de trabalhos, feedbacks de clientes, passo a passo do pedido, dúvidas frequentes e chamada final com link para a Shopee.

## Tecnologias

- HTML5, CSS3 e JavaScript puros, em um único arquivo, sem build e sem dependências
- Google Fonts: Manrope
- Dados estruturados (schema.org) e meta tags para busca e compartilhamento
- Hospedagem: GitHub Pages, com domínio próprio (`CNAME`)

## Estrutura de pastas

```
.
├── index.html   # página única do site (estilos e scripts embutidos)
├── img/         # imagens do portfólio e logo oficial da Magnetiza
├── CNAME        # subdomínio magnetiza.imaguiar.com.br
└── README.md
```

## Como personalizar

O logo original enviado pela cliente está preservado em `img/logo-magnetiza.png`. O símbolo separado, com transparência real, está em `img/icone-magnetiza.png` e aparece no cabeçalho, no rodapé e no ícone da aba. O nome e a assinatura da marca são textos no site, com exibição responsiva. A paleta usa azul-marinho (`#082754`), azul (`#315684`), cinza e branco. A extração do símbolo foi feita com a ferramenta integrada de edição de imagem; o prompt está em `img/README.md`.

No `<script>` do final do `index.html`:

- `WHATSAPP`: número com DDI+DDD, só dígitos (ex.: `"5511999999999"`). Vazio, os botões levam ao direct do Instagram.
- `INSTAGRAM`: usuário do Instagram.
- `MENSAGEM`: texto pronto do WhatsApp.

Na seção `#galeria`, cada `.portfolio-card` contém uma imagem local, título, descrição e link para a publicação original no Instagram. As seis imagens em `img/` foram selecionadas do perfil `@wagnetiza.oficial` em 01/10/2026; incluem fotos e artes de divulgação já publicadas pela marca. As imagens aparecem inteiras e podem ser abertas em tamanho maior. Para trocar um trabalho, atualize a imagem, o texto alternativo, as dimensões e o link da publicação no respectivo card.

A seção `#feedbacks` apresenta as cinco capturas enviadas pela cliente, preservadas em `img/feedbacks/`. O enquadramento uniforme em 9:16 usa `object-fit: contain`, mantendo todo o conteúdo visível. O carrossel permite navegação por botões, rolagem e teclado, com imagens ampliáveis; as frases das legendas foram transcritas dos próprios relatos. Para incluir outro registro, adicione um `.feedback-card` e atualize o total no texto e no rótulo da região.

## Como rodar localmente

```bash
python -m http.server 8000
```

Depois acesse http://localhost:8000.

## Publicação

Publicado pelo GitHub Pages a partir da branch `main`, pasta raiz. Qualquer push na `main` atualiza o site em poucos minutos.
