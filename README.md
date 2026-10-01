# Magnetiza | Ímãs personalizados e impressão 3D

Site institucional da **Magnetiza**, marca de **Alessandra Brassal** que faz ímãs de geladeira personalizados de 50 mm e peças de decoração em impressão 3D, para festas, empresas e eventos, com envio para todo o Brasil.

- **Cliente:** Alessandra Brassal
- **Site publicado:** https://magnetiza.imaguiar.com.br/
- **Instagram:** [@wagnetiza.oficial](https://www.instagram.com/wagnetiza.oficial/)
- **Loja:** [Shopee](https://s.shopee.com.br/gPQTmjNee)

## Sobre o projeto

Página única (one-page), responsiva, para apresentar os produtos e levar o visitante ao pedido de orçamento. O botão de orçamento fica fixo na tela e leva ao direct do Instagram; para usar WhatsApp, basta preencher o número no script do final do `index.html`.

Seções: apresentação, o que fazemos (ímãs, impressão 3D, festas, empresas e eventos), detalhes, galeria de trabalhos, passo a passo do pedido, dúvidas frequentes e chamada final com link para a Shopee.

## Tecnologias

- HTML5, CSS3 e JavaScript puros, em um único arquivo, sem build e sem dependências
- Google Fonts: Fredoka e Nunito
- Dados estruturados (schema.org) e meta tags para busca e compartilhamento
- Hospedagem: GitHub Pages, com domínio próprio (`CNAME`)

## Estrutura de pastas

```
.
├── index.html   # página única do site (estilos e scripts embutidos)
├── CNAME        # subdomínio magnetiza.imaguiar.com.br
└── README.md
```

## Como personalizar

No `<script>` do final do `index.html`:

- `WHATSAPP`: número com DDI+DDD, só dígitos (ex.: `"5511999999999"`). Vazio, os botões levam ao direct do Instagram.
- `INSTAGRAM`: usuário do Instagram.
- `MENSAGEM`: texto pronto do WhatsApp.

Na seção `#galeria`, cada `.slot` é um espaço reservado; para usar foto real, coloque a imagem em `img/` e troque o conteúdo do slot por `<img src="img/arquivo.jpg" alt="descrição">`.

## Como rodar localmente

```bash
python -m http.server 8000
```

Depois acesse http://localhost:8000.

## Publicação

Publicado pelo GitHub Pages a partir da branch `main`, pasta raiz. Qualquer push na `main` atualiza o site em poucos minutos.
