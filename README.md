# 🐾 ATIVIDADE PRÁTICA — Landing Page EducaCão (HTML5 e CSS3)

> **Você é o(a) desenvolvedor(a) contratado(a) pela EducaCão**, uma empresa fictícia de educação canina. O cliente entregou o arquivo **`modelo.pdf`**, que deve ser reproduzido visualmente no projeto final. Sua missão é montar os textos no HTML e reconstruir o visual com as alternativas do CSS.

## 🎯 Objetivo e resultado esperado

A página final deverá apresentar a **mesma organização e a mesma identidade visual do PDF**: marca em verde com destaque laranja, menu horizontal, banner com foto, três cartões de serviços, seção Sobre, faixa verde-clara de diferenciais, três depoimentos fictícios, contato com formulário e rodapé verde-escuro. **Não é uma atividade de criar cores novas**: neste desafio, a fidelidade ao modelo do cliente será avaliada.

Em `css/style.css`, **uma das três opções de cada questão corresponde ao estilo do modelo**. Os valores precisam ser descobertos observando o PDF, testando e comparando. A resposta correta **não está marcada**.

## 📁 Estrutura obrigatória

```text
EducaCao_Atividade_CSS_Visual/
├── index.html                ← complete os ___ do HTML
├── modelo.pdf                ← referência visual do cliente
├── README.md                 ← instruções e regras
├── css/
│   ├── base.css              ← base neutra para a visualização (NÃO EDITAR)
│   └── style.css             ← SEU EXERCÍCIO: preencher alternativas
└── img/
    ├── golden.avif
    ├── adestrador1.avif
    ├── adestrador2.avif
    ├── adestrador 3.avif
    └── sobre.jpg
```

**Atenção às imagens:** as quatro fotos `*.avif` neste pacote são recortes da referência entregue pelo professor e servem ao exercício. A foto `sobre.jpg` é apenas um espaço reservado: substitua-a por uma foto apropriada, se disponibilizada pelo professor. Preserve os nomes exatos ou atualize os `src` no HTML. Não use uma pasta `img` vazia.

## 🚀 Como abrir no VS Code e ver tudo acontecendo

1. No GitHub, clique em **Code → Download ZIP** (ou baixe o ZIP fornecido pelo professor).
2. Extraia **toda a pasta**. Não abra somente o `index.html` sem as pastas `css` e `img`.
3. No **VS Code**, use **Arquivo → Abrir Pasta** e escolha o diretório completo.
4. Instale a extensão **Live Server**, se ainda não estiver instalada.
5. Abra `index.html` e clique com o botão direito em **Open with Live Server**.
6. Deixe o navegador ao lado do VS Code. Preencha uma propriedade, aperte **Ctrl + S** e observe imediatamente a mudança. Use **Ctrl + F** para encontrar o seletor no CSS.
7. Compare o navegador com a página correspondente do `modelo.pdf`, revise e só então avance.

> **A página já aparece no início com um visual neutro**, graças ao arquivo `base.css`. Isso é proposital: o design final só surgirá à medida que o aluno preencher `style.css`.

## 🧩 Regras obrigatórias da atividade

1. **Não edite o `css/base.css`**. Ele existe apenas para você enxergar a evolução do trabalho.
2. **Preencha o `css/style.css` de cima para baixo**. Comece pelas variáveis em `:root` (cores e tamanhos), depois `body`, cabeçalho, logo, menu, botões, banner, serviços e demais seções.
3. Em cada propriedade do CSS, **leia as opções A, B e C** e digite **o valor completo escolhido** depois dos `:`. Ex.: `display: flex;`. **Não escreva `display: A;`**.
4. **Não remova o ponto e vírgula (`;`), as chaves `{ }`, os seletores, os comentários explicativos e os blocos `@media`.**
5. **Não adicione regras no final do CSS para esconder erros** e não substitua `style.css` por um CSS pronto. A atividade exige experimentar, corrigir e compreender os comandos.
6. No `index.html`, **substitua todos os `___` por textos coerentes com o PDF**, preservando tags, classes, IDs e caminhos das imagens. Não mude o `href` dos links de navegação.
7. Respeite a ordem de importação: no `<head>`, **`base.css` antes de `style.css`**. Não inverta e não apague as duas linhas.
8. **Preserve a paleta de cores e o layout final do PDF**; versões com cores diferentes não reproduzem a solicitação do cliente.
9. **Teste a página no computador e no celular** (F12 → alternar dispositivo). Ajuste as opções dentro dos blocos `@media` para caber corretamente.
10. Os depoimentos são **fictícios**; mantenha essa identificação. O formulário é **apenas demonstrativo**, sem PHP/banco de dados nesta etapa.

### Exemplo de preenchimento

```css
/* display: controla como o elemento se organiza.
   A) block
   B) flex
   C) grid
*/
display: ;          /* ANTES: ainda sem resposta */
```

Escolhendo `flex`, o aluno deverá deixar exatamente:

```css
display: flex;      /* DEPOIS: um valor CSS, não a letra B */
```

**Observação importante sobre as variáveis:** preencher `background: var(--green);` só mostrará a cor esperada depois que `--green` tiver um valor válido em `:root`. Por isso, comece pela paleta; não significa que a ligação do CSS esteja quebrada.

## 🗺️ Ordem de trabalho recomendada

| Etapa | Seção no HTML / CSS | Observe no navegador |
| --- | --- | --- |
| 1 | `:root`, `body`, `img`, `a`, `ul` | Cores, fonte, margens e imagens |
| 2 | `.site-header`, `.logo`, `.main-nav` | Cabeçalho e menu distribuídos |
| 3 | `.button`, `.button-primary`, `.button-secondary` | Botões laranja e verde |
| 4 | `.hero`, `.hero-content`, `.hero-image` | Banner com texto e foto lado a lado |
| 5 | `.section`, `.services`, `.service-grid`, `.service-card` | Três cartões em linha em tela grande |
| 6 | `.about`, `.benefits`, `.benefit-grid` | História e faixa verde-clara |
| 7 | `.testimonial-grid`, `.contact`, `.contact-form` | Depoimentos e formulário |
| 8 | `.site-footer`, `.social-links` | Rodapé verde-escuro |
| 9 | `@media` de 980px e 700px | Versão responsiva |

## 🔧 Se você preencher e não aparecer

- Confira se **salvou com Ctrl+S** e se o Live Server está aberto.
- Verifique o arquivo certo: edite **`css/style.css`**, não `css/base.css`.
- Confirme se o HTML contém **duas** referências a CSS e se a ordem está correta.
- Ao usar `var(--nome)`, confira se a variável do `:root` já foi preenchida corretamente.
- Confira se a propriedade tem `:` e `;` e se as chaves `}` dos blocos estão equilibradas.
- No navegador, use **F12 → Network** e verifique se CSS e imagens não apresentam erro **404**.
- O comando correto pode produzir uma mudança pequena ou só ser visível ao passar o mouse (`:hover`) ou em tela pequena (`@media`).
- Use **Ctrl + Shift + R** para atualizar sem cache, se necessário.

## ✅ Entrega e critérios de avaliação

Entregue a pasta ou publique o trabalho no **seu repositório do GitHub** com:

- [ ] `index.html` com todos os textos e atributos `alt` preenchidos;
- [ ] `css/style.css` com as alternativas resolvidas, sem `: ;` nas declarações;
- [ ] `css/base.css` preservado, sem mudanças;
- [ ] imagens da pasta `img/` carregando corretamente;
- [ ] cores, tamanhos e composição coerentes com as duas páginas de `modelo.pdf`;
- [ ] alinhamento correto de menu, três serviços, diferenciais, depoimentos, formulário e rodapé;
- [ ] versão responsiva testada no celular;
- [ ] imagem da página pronta (captura de tela) comparada ao PDF.

**Sugestão de critérios (100 pontos):** HTML e textos 20; preenchimento correto das propriedades CSS 30; fidelidade visual e cores 25; responsividade 15; organização, arquivos e publicação 10.

Para entregar no GitHub: crie um repositório próprio, envie **toda** a pasta do projeto e mantenha os nomes dos arquivos. Na descrição da atividade, mencione o professor no formato `@eduardo97mendes` (marcação em texto) e adicione uma captura de tela da página pronta.

---

**Próximas etapas:** em aulas futuras poderão ser acrescentados JavaScript, PHP e PostgreSQL, mas **não fazem parte desta entrega de HTML/CSS**.
