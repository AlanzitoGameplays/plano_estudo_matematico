# Arquitetura Técnica HTML/CSS
## Plano de Estudo Matemático — Versão 1.0

**Documento 03 da Consolidação Pós-Tópico 1.1**  
**Escopo:** especificação técnica da infraestrutura mínima, estável e herdável das apostilas HTML/CSS do Plano de Estudo Matemático.

Este documento materializa tecnicamente os princípios definidos pela **Arquitetura e Taxonomia Canônica do Sistema de Apostilas — V1.0** e pelas **Regras Gerais HTML/CSS — V3.0**. Sua função é responder:

> **Qual é a infraestrutura técnica que uma apostila normal do Plano Matemático deve herdar antes de sabermos qual será seu conteúdo particular?**

Ele não é o HTML Base definitivo, não é o CSS Base definitivo e não é um catálogo de componentes opcionais. É a especificação a partir da qual esses artefatos poderão ser construídos sem que novas apostilas precisem reaprender a infraestrutura examinando os Blocos III, IV e V.

Em caso de conflito, a ordem de precedência permanece:

1. conteúdo mestre aprovado;
2. Regras Gerais vigentes;
3. esta Arquitetura Técnica;
4. Catálogo de Componentes aplicável;
5. precedente específico, quando necessário;
6. instrução local da tarefa.

---

# 1. Finalidade e escopo

A Arquitetura Técnica descreve o **chassi documental** do Plano Matemático. Ela contém apenas aquilo que uma apostila precisa para existir corretamente antes da introdução de soluções próprias do conteúdo.

Pertencem ao seu escopo:

- tema e tokens canônicos;
- documento e página A4;
- capa;
- cabeçalho, área de conteúdo e rodapé;
- fonte semântica do conteúdo;
- geração de páginas físicas;
- hierarquia editorial estrutural;
- primitivas tipográficas e matemáticas fundamentais;
- infraestrutura genérica de tabelas;
- outline e bookmarks;
- paginação, atomicidade e diagnóstico de overflow;
- comportamento em tela e impressão;
- contrato técnico para extensões futuras.

Não pertencem ao seu escopo:

- componentes semânticos opcionais específicos;
- tabelas especializadas;
- painéis de quantificadores;
- estruturas de argumento ou demonstração;
- recursos geométricos particulares;
- ajustes de uma página específica;
- fluxo operacional completo de produção;
- instruções de agentes;
- Git;
- o template final já preenchido.

Princípio de escopo:

> **A infraestrutura contém aquilo que toda apostila precisa antes de sabermos qual será seu conteúdo.**

---

# 2. Princípios técnicos

## 2.1 Base estável; extensão local

Uma nova apostila deve herdar a infraestrutura comum e acrescentar apenas as extensões exigidas pelo conteúdo.

> **BASE ESTÁVEL + EXTENSÃO LOCAL**

é preferível a:

> **BASE MODIFICADA PARA CADA NOVO CONTEÚDO.**

## 2.2 Herança técnica deve ser intencional

Copiar um arquivo anterior não autoriza transportar todo o seu CSS. Classes de quantificadores, argumentos, demonstrações, exercícios específicos ou correções históricas não pertencem à nova apostila apenas porque estavam presentes no precedente usado como ponto de partida.

## 2.3 Fonte semântica e página física são camadas distintas

O conteúdo é organizado semanticamente antes de ser distribuído fisicamente em folhas A4. Quebras concretas de página não devem comandar a estrutura conceitual do conteúdo.

## 2.4 O paginador organiza; não reescreve

O mecanismo de paginação move unidades de conteúdo entre páginas. Não deve resumir, duplicar, reordenar semanticamente ou alterar o texto mestre para fazê-lo caber.

## 2.5 O resultado renderizado possui precedência prática

Código aparentemente elegante que produz PDF pior não é solução superior. A arquitetura deve ser validada pelo resultado real em:

- paginação;
- legibilidade;
- outline;
- ausência de clipping e overflow;
- fidelidade semântica;
- manutenção razoável.

## 2.6 Componentes devem ser transparentes ao núcleo

O paginador não deve precisar conhecer a semântica de `definition-box`, `argument-stack`, painéis de quantificadores ou qualquer outro componente opcional. Um componente correto respeita o contrato de fluxo da arquitetura e se encaixa sem contaminar o núcleo.

---

# 3. Modelo geral do documento

A arquitetura adota:

```text
CONTEÚDO-FONTE SEMÂNTICO
        ↓
PAGINADOR
        ↓
PÁGINAS A4 RENDERIZADAS
        ↓
PDF OFICIAL
```

O HTML contém duas representações complementares.

### A. Representação semântica

Organiza o conteúdo em seções conceituais, títulos, parágrafos, matemática, tabelas, visuais e componentes. Essa camada existe em `.source-content` e em suas `.source-section`.

### B. Representação física

Organiza o mesmo conteúdo em páginas concretas `.page`, com cabeçalho, `.page-content` e rodapé.

O paginador **move os nós reais** da fonte semântica para as páginas geradas. Não é necessário manter uma segunda cópia visível do conteúdo.

---

# 4. Camadas da arquitetura

| Camada | Função | Elementos centrais | Status |
|---|---|---|---|
| **1 — Tokens e identidade** | fornecer valores comuns e pontos de extensão | `.theme--math`, variáveis CSS | consolidado |
| **2 — Documento e página** | representar o artefato e a folha física | `.document`, `.page`, `.page-content` | consolidado |
| **3 — Navegação documental** | localizar leitor e gerar navegação | header, footer, headings, `.outline-root` | consolidado |
| **4 — Hierarquia editorial** | representar Partes, seções e níveis internos | openings, labels, titles | consolidado |
| **5 — Prosa e matemática fundamental** | fornecer primitivas de leitura e notação | prosa, `.math-inline`, `.math-line`, `.math-structural` | consolidado |
| **6 — Infraestrutura tabular** | fornecer base visual e física às tabelas | `.table-wrap`, `table`, `thead`, `th`, `td` | consolidado |
| **7 — Paginação** | distribuir unidades pela área útil | `.source-section`, paginador, helpers atômicos | consolidado |
| **8 — Tela e impressão** | separar preview de produto impresso | `@media screen`, `@media print`, `@page` | consolidado |
| **9 — Pontos de extensão** | receber componentes sem modificar o núcleo | contrato de componente/visual | consolidado como princípio |

---

# 5. Tokens e identidade técnica

## 5.1 Escopo de `.theme--math`

A classe `.theme--math` é o contêiner de identidade do Plano Matemático. Os tokens globais devem ser declarados nesse escopo ou em mecanismo semanticamente equivalente, evitando valores cromáticos e tipográficos repetidos por todo o CSS.

## 5.2 Paleta canônica

| Token | Valor | Função geral |
|---|---:|---|
| `--primary` | `#252B5E` | índigo; títulos, identidade principal e matemática |
| `--secondary` | `#3657A7` | cobalto; hierarquia secundária, tabelas e linhas |
| `--accent` | `#6558A6` | violeta; acentos editoriais e níveis menores |
| `--support` | `#7396C8` | azul técnico; suporte, linhas e contraste auxiliar |
| `--soft` | `#EEF2F8` | fundo leve funcional |
| `--border` | `#C5CEDD` | linhas e divisórias discretas |
| `--text` | `#252A33` | grafite do corpo |
| `--muted` | `#6F7583` | metadados e hierarquia subordinada |
| `--paper` | `#FBFCFE` | papel editorial |
| `--white` | `#FBFCFE` | branco editorial da identidade |
| `--screen` | `#EEF2F8` | fundo externo do preview |

Os valores fazem parte da identidade matemática e não devem ser alterados isoladamente por um bloco.

## 5.3 Tokens de página

Os precedentes maduros III–V convergem para:

```css
--page-width: 210mm;
--page-height: 297mm;
--page-top: 12mm;
--page-right: 17mm;
--page-bottom: 7mm;
--page-left: 20mm;
```

Esses valores são a geometria-base da implementação atual. Uma alteração deve ser tratada como mudança de arquitetura, e não como ajuste casual de conteúdo.

## 5.4 Tokens tipográficos

```css
--font-heading: Arial, "Liberation Sans", "DejaVu Sans", sans-serif;
--font-body: Georgia, "Times New Roman", "Liberation Serif", serif;
--font-math: "Cambria Math", "STIX Two Math", "DejaVu Math TeX Gyre", serif;
```

Escala consolidada de referência:

```css
--text-size: 9.55pt;
--text-line: 1.39;
--text-small: 8.2pt;
--text-micro: 7.25pt;

--title-cover: 27.5pt;
--title-part: 19.5pt;
--title-section: 13.2pt;
--title-subsection: 10.2pt;
--title-minor: 8.5pt;
```

### Observação sobre `--title-section`

Nos precedentes III–V, `--title-section` é declarado, mas `.section-title` conserva historicamente um valor direto de `19pt`. Isso é uma inconsistência de implementação, não razão para manter duas fontes de verdade.

O futuro CSS Base deverá **utilizar efetivamente o token para o nível que ele representa ou remover/renomear o token após decisão explícita**. Esta arquitetura não congela a duplicidade histórica como requisito.

## 5.5 Linhas e raio

```css
--line-thin: 0.24mm;
--line-regular: 0.34mm;
--line-medium: 0.78mm;
--line-strong: 1.3mm;
--radius-small: 1.2mm;
```

Os tokens de linha são parte da linguagem gráfica recorrente. `--radius-small` permanece disponível como token de extensão para componentes que justificarem raio discreto; sua existência não obriga o uso de caixas arredondadas.

## 5.6 Espaçamento

Os precedentes utilizam valores estáveis de espaçamento, mas ainda não existe uma escala abstrata de spacing tokens suficientemente consolidada.

A V1.0 **não inventa** uma escala nova apenas para completar o sistema.

---

# 6. Primitivas globais

A infraestrutura deve estabelecer um pequeno conjunto de garantias globais.

## 6.1 Box model

```css
*, *::before, *::after {
    box-sizing: border-box;
}
```

Essa regra é fundamental para a previsibilidade das dimensões físicas.

## 6.2 Documento

O `body` utiliza por padrão:

- margem externa zero;
- fonte discursiva;
- cor de texto canônica;
- tamanho e entrelinha-base;
- fundo de preview;
- largura real das páginas preservada.

## 6.3 Elementos de fluxo

Elementos estruturais usados dentro de grid/flex devem aceitar redução de largura:

```css
main, section, article, header, footer, div {
    min-width: 0;
}
```

## 6.4 Prosa e listas

Parágrafos e listas possuem ritmo moderado. Controles de `orphans` e `widows` podem reduzir quebras tipográficas ruins, mas não substituem a paginação conceitual.

## 6.5 Mídia

Imagens devem respeitar a área disponível:

```css
img {
    display: block;
    max-width: 100%;
}
```

SVG e outros visuais devem obedecer ao mesmo contrato de largura.

---

# 7. Geometria A4

## 7.1 Página física

A página final é A4:

```css
@page {
    size: A4;
    margin: 0;
}
```

A margem física do navegador fica em zero porque a área útil é controlada pela própria `.page`.

## 7.2 `.page` como folha física

A folha é representada por um contêiner com:

- largura de `210mm`;
- altura de `297mm`;
- `box-sizing: border-box`;
- padding interno;
- três faixas estruturais: cabeçalho, conteúdo flexível e rodapé.

Modelo:

```css
.page {
    display: grid;
    grid-template-rows: auto minmax(0, 1fr) auto;
    width: var(--page-width);
    height: var(--page-height);
    padding:
        var(--page-top)
        var(--page-right)
        var(--page-bottom)
        var(--page-left);
}
```

O uso de `border-box` impede que o padding faça a folha ultrapassar `210 × 297mm`.

## 7.3 Área interna

Nos precedentes maduros:

```css
.page-content {
    min-width: 0;
    min-height: 0;
    padding-top: 4mm;
    padding-bottom: 3.6mm;
}
```

`min-height: 0` permite que a faixa central do grid possua altura mensurável corretamente.

## 7.4 Prevenção de overflow horizontal

Nenhum elemento interno deve assumir `210mm` como largura disponível.

> **Componentes dimensionam-se em relação à área útil, nunca à folha física inteira.**

---

# 8. Estrutura DOM canônica

O seguinte skeleton representa a arquitetura, não o futuro arquivo Base definitivo:

```html
<!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <meta name="description" content="...">
  <title>...</title>
  <link rel="stylesheet" href="...css">
</head>

<body class="theme--math">
  <main class="document" id="document">

    <section
      class="page page--cover"
      id="capa"
      aria-label="Capa"
    >
      <div class="cover-top">
        <div class="cover-collection">
          PLANO DE ESTUDO MATEMÁTICO
        </div>
      </div>

      <div class="cover-bottom">
        <div class="cover-kicker">...</div>
        <div class="cover-title">...</div>

        <div class="cover-rule" aria-hidden="true">
          <span></span>
          <span></span>
        </div>

        <div class="cover-version">...</div>
      </div>
    </section>

    <div class="source-content" id="source-content">

      <section
        class="source-section"
        data-context="..."
      >
        ...conteúdo semântico...
      </section>

    </div>

  </main>

  <script>
    /* paginador */
  </script>
</body>
</html>
```

### Contratos essenciais

| Elemento | Função | Obrigatório? | Pode variar? |
|---|---|---:|---|
| `body.theme--math` | ativa identidade matemática | sim | nome só muda em nova arquitetura de tema |
| `main#document.document` | raiz das páginas e da fonte | sim | conteúdo interno varia |
| `.page.page--cover` | primeira folha física | sim nas apostilas padrão | conteúdo e quebras variam |
| `#source-content.source-content` | fonte semântica ainda não paginada | sim | não deve virar paginação manual |
| `.source-section` | fronteira contextual e início de nova sequência | sim | quantidade varia |
| `data-context` | contexto das páginas geradas | sim | valor varia |
| `.page--generated` | página criada em runtime | gerada | não é conteúdo autoral |
| `.page-header` | localização interna | gerada | texto varia |
| `.page-content` | área de encaixe e medição | gerada | estrutura fixa |
| `.page-footer` | identidade e número | gerada | identidade varia |

---

# 9. Fonte semântica e páginas renderizadas

## 9.1 `.source-content`

`.source-content` contém a versão semântica contínua do conteúdo interno.

```css
.source-content {
    display: none;
}
```

A ocultação não impede que o JavaScript acesse e mova seus nós internos.

## 9.2 `.source-section`

Cada `.source-section` representa uma **unidade contextual maior**.

Nos precedentes ela corresponde a:

- Parte do Texto Teórico;
- Exemplos Resolvidos;
- Quiz;
- Exercícios;
- Gabarito Comentado.

O paginador cria uma nova página no início de cada `.source-section`. Portanto, ela funciona simultaneamente como:

- fronteira de contexto;
- fronteira de running header;
- início deliberado de sequência paginada.

Não se deve criar uma `.source-section` para cada subseção pequena apenas para forçar quebra.

## 9.3 `data-context`

```html
<section
  class="source-section"
  data-context="TEXTO TEÓRICO • PARTE I"
>
```

O atributo fornece o texto utilizado por `.header-context`.

| Atributo | Função | Escopo | Consumidor |
|---|---|---|---|
| `data-context` | contexto do running header | `.source-section` | `makePage()` |
| `data-keep-count` | une o nó atual a N−1 irmãos seguintes | filho direto de `.source-section` | paginador |

Atributos como `data-visual`, presentes em precedentes específicos, não são consumidos pelo núcleo atual e não pertencem automaticamente à infraestrutura.

## 9.4 Ciclo de vida

1. navegador carrega capa e fonte semântica;
2. paginador identifica as `.source-section`;
3. cria páginas físicas;
4. move os filhos das seções para `.page-content`;
5. remove a fonte semântica ao final.

Mover, em vez de clonar, reduz duplicação e risco de IDs repetidos.

---

# 10. Contrato de `.document`

`.document` é a raiz visual de todas as folhas.

### Em tela

Deve:

- empilhar páginas verticalmente;
- centralizar folhas quando houver espaço;
- manter separação visual;
- preservar a largura física A4;
- permitir inspeção de overflow.

Referência:

```css
.document {
    display: flex;
    flex-direction: column;
    align-items: center;
    gap: 18px;
    width: 100%;
    padding: 24px 0;
}
```

`18px` e `24px` pertencem ao **preview**, não à geometria do PDF.

### Em impressão

```css
.document {
    display: block;
    gap: 0;
    padding: 0;
}
```

---

# 11. Contrato de `.page`

`.page` é a unidade física da impressão.

Deve:

- possuir dimensão A4 fixa;
- usar grid de três linhas;
- conter header, área central e footer nas páginas internas;
- terminar com quebra de página;
- preservar geometria entre screen e print;
- não esconder overflow real.

A sombra observada em tela é apenas recurso de preview.

`.page--generated` identifica páginas produzidas pelo paginador e não necessita de identidade visual própria.

---

# 12. Capa

A capa utiliza a mesma folha A4, mas substitui o grid header/conteúdo/footer por duas zonas editoriais.

```html
<section
  class="page page--cover"
  id="capa"
  aria-label="Capa"
>
  <div class="cover-top">
    <div class="cover-collection">
      PLANO DE ESTUDO MATEMÁTICO
    </div>
  </div>

  <div class="cover-bottom">
    <div class="cover-kicker">...</div>
    <div class="cover-title">...</div>

    <div class="cover-rule" aria-hidden="true">
      <span></span>
      <span></span>
    </div>

    <div class="cover-version">...</div>
  </div>
</section>
```

Configuração consolidada:

- `.page--cover`: `101mm` na região superior + espaço restante;
- `.cover-top`: zona institucional índigo;
- faixa cromática inferior na zona escura;
- `.cover-bottom`: região de identificação;
- `.cover-title`: título principal;
- `.cover-rule`: elemento decorativo `aria-hidden`;
- `.cover-version`: identificação editorial.

A capa não recebe header/footer internos.

Quebras manuais de linha do título são adaptações da capa, não invariantes técnicos.

---

# 13. Cabeçalho

Estrutura:

```html
<header class="page-header">
  <span>PLANO DE ESTUDO — MATEMÁTICA</span>
  <span class="header-context">...</span>
</header>
```

Contrato:

- esquerda: identidade constante;
- direita: contexto da `.source-section`;
- fonte editorial;
- escala pequena;
- linha inferior discreta;
- não competir com títulos internos.

`.header-context` deve tolerar contexto relativamente longo sem romper a página. Os precedentes usam:

- largura máxima próxima de `92mm`;
- linha única;
- `overflow: hidden`;
- `text-overflow: ellipsis`.

O truncamento é proteção técnica, não licença para criar rótulos excessivamente longos.

> **Header = localização interna.**

---

# 14. Rodapé

```html
<footer class="page-footer">
  <span>IDENTIDADE DA APOSTILA</span>
  <span class="page-number">2</span>
</footer>
```

Contrato:

- esquerda: identidade documental;
- direita: número físico;
- linha superior discreta;
- mesma linguagem do cabeçalho;
- números tabulares.

Nos precedentes, a capa corresponde à primeira folha e a primeira página interna começa em `2`.

> **Footer = identidade documental + paginação.**

O texto específico da apostila é dado variável; o mecanismo não deve ser reimplementado por bloco.

---

# 15. Área de conteúdo e fluxo principal

A prosa normal ocupa uma única coluna da área útil.

A infraestrutura não cria colunas gerais para compactação. Grids e múltiplas colunas pertencem a componentes cuja função exige simultaneidade ou comparação.

Elementos estruturais devem aceitar redução de largura:

```css
main,
section,
article,
header,
footer,
div {
    min-width: 0;
}
```

Imagens devem, no mínimo:

```css
img {
    display: block;
    max-width: 100%;
}
```

---

# 16. Hierarquia editorial estrutural

| Classe | Função | Outline por si só? | Status |
|---|---|---:|---|
| `.section-opening` | abertura de grande seção | não; contém heading | infraestrutura |
| `.part-opening` | abertura de Parte real | não; contém heading | infraestrutura |
| `.section-label` | rótulo da seção | somente se for heading | infraestrutura |
| `.part-label` | rótulo de Parte | não necessariamente | infraestrutura |
| `.section-title` | título principal de seção | quando usado como heading | infraestrutura |
| `.part-title` | título de Parte | quando usado como heading | infraestrutura |
| `.item-title` | título visual de unidade interna | não por padrão | infraestrutura |
| `.minor-title` | subtítulo subordinado | não por padrão | infraestrutura |
| `.gabarito-subtitle` | título visual interno de gabarito | não por padrão | infraestrutura recorrente |

## 16.1 Abertura de Parte

Exemplo:

```html
<header class="part-opening" data-keep-count="3">

  <div class="part-label">
    <h1 class="outline-root">
      Texto Teórico
    </h1>
    · Parte I
  </div>

  <h2 class="part-title">
    Parte I — ...
  </h2>

</header>
```

O `h1` da raiz aparece onde a raiz de navegação é inaugurada. Partes seguintes não repetem desnecessariamente outro `h1` “Texto Teórico”.

## 16.2 Títulos visuais não precisam entrar no outline

`.item-title` e `.minor-title` fornecem hierarquia visual sem poluir bookmarks.

## 16.3 Modificadores de comprimento

Classes históricas como `.part-title--long` são microajustes, não infraestrutura obrigatória.

---

# 17. Tipografia

A arquitetura separa três papéis.

### Editorial

Arial ou fallback equivalente:

- títulos;
- labels;
- cabeçalho;
- rodapé;
- números;
- cabeçalhos de tabela;
- metadados.

### Discursiva

Georgia ou fallback serifado:

- parágrafos;
- explicações;
- listas discursivas;
- interpretação.

### Matemática

Cambria Math, STIX ou equivalente:

- notação;
- fórmulas;
- relações simbólicas.

O sistema não deve depender de fontes raras ou não confiáveis no ambiente oficial.

---

# 18. Matemática fundamental

A arquitetura fornece três primitivas e um helper textual.

## 18.1 `.math-inline`

Função: matemática integrada à frase.

Contrato:

- forma padrão;
- fonte matemática;
- cor primária;
- `white-space: nowrap` para expressões curtas.

```html
<p>
  Se <span class="math-inline">p→q</span> é verdadeira...
</p>
```

Expressão longa que produz overflow deve ser reclassificada editorialmente, e não corrigida desligando globalmente a proteção de quebra.

## 18.2 `.math-line`

Função: expressão simples em linha própria.

Configuração madura:

```css
.math-line {
    margin: .45mm 0 .9mm 4mm;
    text-align: left;
    font-family: var(--font-math);
    font-size: 9.9pt;
    line-height: 1.34;
}
```

Características:

- alinhada à esquerda;
- recuo discreto;
- sem caixa;
- sem fundo;
- sem centralização automática.

## 18.3 `.math-structural`

Função: disposição espacial relevante.

```css
.math-structural {
    width: fit-content;
    max-width: 100%;
    margin: 2.2mm auto 2.6mm;
    font-family: var(--font-math);
    font-size: 11.2pt;
    line-height: 1.35;
    text-align: center;
    break-inside: avoid;
}
```

A centralização ocorre porque a estrutura espacial justifica, não porque a expressão é matemática.

## 18.4 `.math-text`

Permite prosa dentro de estrutura cuja fonte externa é matemática:

```css
.math-text {
    font-family: var(--font-body);
    white-space: normal;
}
```

É helper técnico, não componente editorial.

## 18.5 Fora da base

Não entram automaticamente:

- `argument-stack`;
- `proof-schema`;
- `math-sequence`;
- formas de inferência;
- frações customizadas específicas;
- esquemas de quantificadores;
- cadeias semânticas especializadas.

---

# 19. Infraestrutura tabular

A arquitetura distingue mecanismo genérico de tabela de tipo semântico.

## 19.1 `.table-wrap`

Responsabilidades:

- respeitar a área disponível;
- fornecer ritmo vertical;
- expor, e não esconder, problemas de largura.

III–V preservam historicamente uma declaração de `overflow-x: auto`, mas IV e V a anulam depois com `overflow: visible`.

Para o futuro Base:

> **scroll horizontal não pode mascarar uma tabela larga que falhará no PDF.**

## 19.2 HTML tabular real

Dados tabulares devem usar:

- `<table>`;
- `<thead>`;
- `<tbody>`;
- `<tr>`;
- `<th>`;
- `<td>`;
- `scope`, quando apropriado.

## 19.3 Comportamento-base

- largura `100%`;
- `table-layout: fixed` como padrão;
- `border-collapse: collapse`;
- `thead` repetível como `table-header-group`;
- fonte editorial nos cabeçalhos;
- bordas discretas;
- alinhamento superior;
- alternância suave de linhas quando não houver semântica conflitante.

## 19.4 Tipos especializados ficam fora

Não pertencem à infraestrutura:

- `truth-table`;
- `translation-table`;
- `comparison-table`;
- `analysis-table`;
- `worksheet-table`;
- `counterexample-table`;
- tabelas específicas de quantificadores;
- larguras de coluna próprias de um exercício.

## 19.5 Tabelas longas

A arquitetura atual cobre tabelas compatíveis com uma página.

A V1.0 não congela estratégia para tabelas verdadeiramente multipágina. Esse problema só deve ser resolvido quando houver caso real.

---

# 20. Outline e bookmarks

## 20.1 Outline é semântico

Modelo geral:

```text
Texto Teórico
├── Parte I
├── Parte II
└── Parte III

Texto Prático
├── Exemplos Resolvidos
├── Quiz
├── Exercícios
└── Gabarito Comentado
```

A quantidade real varia com o conteúdo.

## 20.2 `.outline-root`

Permite heading semanticamente real sem impor aparência própria:

```css
.outline-root {
    margin: 0;
    padding: 0;
    color: inherit;
    font: inherit;
    font-weight: inherit;
    letter-spacing: inherit;
    line-height: inherit;
    text-transform: none;
}
```

O `display` pode depender do contexto em que o heading está inserido.

## 20.3 Texto contínuo

Invariante:

> **Heading destinado a bookmark deve, sempre que possível, possuir um único fluxo textual contínuo.**

Não fragmentar heading em spans apenas para controlar wrapping visual.

## 20.4 Heading visual não é bookmark

`.item-title`, `.minor-title` e equivalentes não viram headings apenas para reproduzir aparência.

---

# 21. Arquitetura de paginação

O mesmo algoritmo-base permanece nos Blocos III, IV e V. Isso constitui evidência forte de estabilidade.

## 21.1 Responsabilidades

O paginador deve:

1. localizar raiz documental;
2. localizar fonte semântica;
3. iniciar numeração após a capa;
4. percorrer `.source-section` de primeiro nível;
5. criar nova página para cada início de seção;
6. gerar header/footer;
7. aplicar contexto;
8. mover unidades para `.page-content`;
9. respeitar atomicidade;
10. medir overflow;
11. transportar o grupo para nova página;
12. marcar overflow persistente;
13. remover a fonte semântica ao terminar.

## 21.2 `makePage(context)`

Responsável por:

- criar `.page.page--generated`;
- inserir header;
- criar `.page-content`;
- inserir footer;
- aplicar contexto;
- aplicar número;
- inserir a folha antes de `source-content`.

A identidade específica do bloco é um dado da instância, não motivo para duplicar o algoritmo.

## 21.3 `overflows(content)`

Padrão comprovado:

```js
content.scrollHeight > content.clientHeight + 1
```

A tolerância de `1px` reduz falso positivo provocado por arredondamento.

## 21.4 `appendAtomic(content, nodes)`

Move os nós do grupo para a página preservando ordem.

## 21.5 `removeAtomic(content, nodes)`

Retira o grupo quando a tentativa de encaixe produz overflow e preserva as referências para a página seguinte.

## 21.6 Pseudocódigo

```text
source ← #source-content
pageNumber ← 2

para cada source-section filha direta de source:

    context ← section.data-context
    page ← criarPágina(context)
    content ← page.page-content
    nodes ← filhos diretos de section

    para cada node:

        count ← 1

        se node possui data-keep-count:
            count ← valor positivo de data-keep-count

        senão se node possui keep-with-next:
            count ← 2

        count ← limitar aos irmãos restantes

        atomic ←
            node atual
            + próximos (count - 1)

        mover atomic para content

        se content excede altura disponível:

            retirar atomic

            page ← criarPágina(context)
            content ← page.page-content

            mover atomic para content

            se ainda excede:
                marcar overflow-warning

        avançar pelo número de nós consumidos

remover source
```

## 21.7 Snippet representativo

```js
const sections = Array.from(
  source.querySelectorAll(':scope > .source-section')
);

for (const section of sections) {

  const context = section.dataset.context || '';

  let page = makePage(context);
  let content = page.querySelector('.page-content');

  const nodes = Array.from(section.children);

  for (let i = 0; i < nodes.length; i++) {

    const node = nodes[i];

    let count = 1;

    if (node.dataset?.keepCount) {

      count = Math.max(
        1,
        parseInt(node.dataset.keepCount, 10) || 1
      );

    } else if (
      node.classList?.contains('keep-with-next')
      && i + 1 < nodes.length
    ) {

      count = 2;
    }

    count = Math.min(
      count,
      nodes.length - i
    );

    const atomic = nodes.slice(
      i,
      i + count
    );

    appendAtomic(content, atomic);

    if (overflows(content)) {

      removeAtomic(content, atomic);

      page = makePage(context);
      content = page.querySelector('.page-content');

      appendAtomic(content, atomic);

      if (overflows(content)) {
        page.classList.add(
          'page--overflow-warning'
        );
      }
    }

    i += count - 1;
  }
}
```

## 21.8 Paginador content-agnostic

É inadequado introduzir lógica como:

```text
se for argument-stack → faça X
se for quantifier-panel → faça Y
se for proof-schema → faça Z
```

Componentes devem obedecer ao contrato comum de fluxo.

---

# 22. Atomicidade e dependências pedagógicas

## 22.1 `.keep-with-next`

Relaciona o nó atual ao irmão seguinte.

```html
<div class="item-title keep-with-next">
  ...
</div>

<p>
  ...
</p>
```

Sem `data-keep-count`, o paginador considera os dois nós um grupo.

## 22.2 `data-keep-count`

Agrupa uma cadeia curta de irmãos.

```html
<div
  class="item-title keep-with-next"
  data-keep-count="3"
>
  ...
</div>

<p>...</p>
<div class="math-line">...</div>
```

`3` significa:

> nó atual + dois irmãos seguintes.

Não usar para obter visualmente uma página mais cheia ou bonita.

## 22.3 `.atomic-group`

IV–V consolidam um padrão genérico útil: envolver pequena unidade composta em um único filho direto.

```html
<div class="atomic-group">

  <div class="minor-title">
    ...
  </div>

  <p>...</p>

  <div class="math-line">
    ...
  </div>

</div>
```

Por possuir função puramente estrutural e reutilizável, `.atomic-group` é classificada como **helper técnico opcional da arquitetura**.

Contrato:

- deve caber numa página nova;
- não deve envolver exercícios longos;
- não deve envolver demonstrações longas;
- não deve envolver tabela maior que a área disponível;
- pode utilizar `break-inside: avoid`.

## 22.4 Princípio

> **Proteja dependências pequenas; deixe unidades longas quebrarem naturalmente.**

---

# 23. Overflow e diagnóstico

## 23.1 Overflow vertical

É medido em `.page-content`, não no `body`.

Quando a unidade não cabe:

1. retira-se o grupo;
2. cria-se página seguinte;
3. reinsere-se o grupo;
4. se ainda não couber, sinaliza-se o defeito.

## 23.2 `.page--overflow-warning`

É diagnóstico exclusivo de tela:

```css
@media screen {

  .page--overflow-warning {
      outline: 2px solid var(--accent);
  }

}
```

Não deve aparecer no PDF.

## 23.3 Overflow horizontal

O paginador histórico não possui medição JavaScript canônica de largura.

Por isso:

- CSS deve impedir larguras incompatíveis;
- tabelas e mídias respeitam área útil;
- preflight verifica largura;
- um futuro warning horizontal pode ser criado caso demonstre utilidade.

`overflow-x: auto` não transforma conteúdo largo em conteúdo válido para PDF.

## 23.4 Não esconder defeitos

Não utilizar como correção geral:

- `overflow: hidden` em conteúdo;
- redução global de fonte;
- compressão indiscriminada de margens;
- remoção de conteúdo.

---

# 24. Comportamento em tela

O preview serve à inspeção.

Padrão:

- fundo `--screen`;
- páginas A4 reais;
- sombra discreta;
- gap;
- centralização em monitor largo;
- alinhamento à esquerda em viewport estreita;
- warnings visíveis.

Referência:

```css
@media screen and (max-width: 900px) {

    .document {
        align-items: flex-start;
        padding: 12px;
    }

    .page {
        transform-origin: top left;
    }

}
```

Não aplicar uma escala automática que faça overflow parecer resolvido.

---

# 25. Comportamento em impressão

```css
@media print {

    html,
    body {
        width: var(--page-width);
        margin: 0;
        padding: 0;
        background: var(--paper);
    }

    .document {
        display: block;
        gap: 0;
        padding: 0;
    }

    .page {
        margin: 0;
        box-shadow: none;
        break-after: page;
        page-break-after: always;
    }

    .page:last-of-type {
        break-after: auto;
        page-break-after: auto;
    }

}
```

Também são estruturais:

```css
-webkit-print-color-adjust: exact;
print-color-adjust: exact;
```

### Screen ≠ print

Existem apenas no preview:

- sombra;
- fundo externo;
- gap externo;
- warning visual.

Não deve haver diferença semântica entre screen e print.

---

# 26. Nomenclatura e identificadores

## 26.1 Classes

- `kebab-case`;
- nomes por função;
- modificadores com `--` quando representam variante real.

Adequado:

```text
page--cover
page--generated
math-structural
```

Inadequado:

```text
exercise-9-blue-box
page-37-fix
quantifier-purple-panel-final
```

## 26.2 IDs

Consolidados:

```text
#document
#source-content
#capa
```

`#document` e `#source-content` são contratos do paginador atual.

`#capa` possui função de identificação semântica/documental, mas não deve tornar-se dependência arbitrária de estilo.

## 26.3 Atributos `data-*`

Metadados de paginação e contexto usam `data-*`, em vez de codificar informação de runtime no nome da classe.

---

# 27. Semântica e acessibilidade

## 27.1 Documento

A base deve possuir:

```html
<html lang="pt-BR">
```

e:

```html
<meta charset="utf-8">
```

Além de:

- `<title>` coerente;
- viewport;
- descrição documental quando pertinente.

## 27.2 Headings

Headings reais representam unidades de navegação.

Não são criados apenas para obter tamanho tipográfico.

## 27.3 Tabelas

Dados tabulares usam tabela HTML real.

Cabeçalhos usam `<th>` e `scope` quando apropriado.

## 27.4 Elementos decorativos

Elementos puramente decorativos podem utilizar:

```html
aria-hidden="true"
```

## 27.5 `aria-label`

Utilizar quando acrescenta identificação útil.

Não usar ARIA para:

- fabricar bookmark;
- substituir heading correto;
- corrigir artificialmente semântica HTML inadequada.

## 27.6 Limite atual

A V1.0 não declara ainda uma política completa para:

- descrição de diagramas;
- leitura matemática avançada;
- gráficos;
- mapas;
- figuras complexas.

Esses temas devem ser consolidados a partir de uso real.

---

# 28. Pontos de extensão

Uma `.source-section` pode receber:

- prosa;
- listas;
- matemática;
- tabela;
- visual;
- componente semântico;
- exercício;
- abertura editorial.

O núcleo do paginador precisa saber apenas:

1. ordem;
2. dependência/atomicidade;
3. tamanho físico.

Ele não precisa conhecer a categoria pedagógica particular do componente.

---

# 29. Contrato técnico de componente futuro

Todo componente opcional deverá:

1. caber na largura útil;
2. herdar `box-sizing: border-box`;
3. não produzir overflow horizontal;
4. declarar comportamento de quebra coerente;
5. usar tokens canônicos;
6. não alterar infraestrutura global para resolver problema local;
7. manter HTML semanticamente adequado;
8. funcionar em screen e print;
9. não depender de hack global;
10. não alterar o paginador apenas por possuir semântica própria;
11. não esconder conteúdo para caber;
12. não antecipar resposta pedagógica por aparência.

Se um componente exige exceção de paginação, deve-se verificar primeiro se:

- foi marcado atomicamente em excesso;
- pode quebrar internamente;
- o problema é local;
- existe função realmente geral que justifique nova versão da arquitetura.

---

# 30. Limite entre infraestrutura e componentes

| Elemento | Destino | Justificativa |
|---|---|---|
| `.theme--math` | Arquitetura | identidade global |
| `.document` | Arquitetura | raiz física/preview |
| `.page` / `.page-content` | Arquitetura | modelo da folha |
| header/footer | Arquitetura | navegação e identidade |
| `.source-content` / `.source-section` | Arquitetura | modelo semântico/paginação |
| `.outline-root` | Arquitetura | contrato de navegação |
| `.math-inline` / `.math-line` / `.math-structural` | Arquitetura | primitivas matemáticas |
| `.math-text` | Arquitetura | helper tipográfico |
| `.table-wrap` + tabela-base | Arquitetura | infraestrutura tabular |
| `.keep-with-next` / `data-keep-count` | Arquitetura | paginação genérica |
| `.atomic-group` | Arquitetura auxiliar | agrupamento curto |
| `.visual` | ponto de extensão | contrato genérico de visual |
| `.definition-box` | Catálogo | componente semântico |
| `.answer-box` | Catálogo | componente de resposta |
| `.student-quote` | Catálogo | função pedagógica específica |
| `.key-statement` | Catálogo/revisão | destaque semântico |
| `truth-table` | Catálogo | tipo funcional de tabela |
| `analysis-table` | Catálogo | tipo funcional de tabela |
| `worksheet-table` | Catálogo | estado de exercício |
| `argument-stack` | Catálogo | estrutura inferencial |
| `proof-schema` | Catálogo | estrutura de demonstração |
| `attempt-block` | Catálogo | estrutura pedagógica |
| painéis de quantificadores | local/Catálogo após promoção | função específica |
| `.part-title--long` | microajuste | comprimento local |
| larguras específicas via `nth-child()` | local | dependência do conteúdo |
| `data-visual` | local/auditoria | não consumido pelo núcleo |

---

# 31. O que não pertence à base

Não incluir automaticamente:

- `definition-box`;
- `statement-example`;
- `student-quote`;
- `answer-box`;
- `key-statement`;
- `truth-table` e variantes;
- `analysis-table`;
- `worksheet-table`;
- `argument-stack`;
- `argument-premises`;
- `argument-conclusion`;
- `proof-schema`;
- `proof-step`;
- `attempt-block`;
- `inference-pair`;
- painéis de domínio;
- grids de quantificadores;
- `blank-line`;
- formas geométricas específicas;
- larguras locais de colunas;
- `focus-row` dependente da tabela;
- correções de página;
- classes ligadas a apenas um bloco.

A presença de uma classe em III, IV ou V não constitui prova de que ela pertence à infraestrutura.

---

# 32. CSS morto e herança acidental

A evolução III → IV → V demonstra que copiar CSS completo do precedente pode transportar resíduos sem uso.

Princípio:

> **Seletor específico sem consumidor real não acompanha a nova apostila.**

A montagem futura deve tender a:

```text
CSS Base
+
componentes necessários
+
extensão local mínima
```

e não:

```text
copiar CSS do bloco anterior
+
apagar parcialmente o que não for necessário
```

---

# 33. Extensão sem contaminação

Componente específico não deve redefinir indiscriminadamente:

- `.page`;
- `.page-content`;
- `.document`;
- header/footer;
- tokens globais;
- paginador;
- headings globais;
- todas as tabelas;
- comportamento global de print.

Se isso for necessário, avaliar se:

1. existe bug na arquitetura;
2. a função se tornou sistêmica;
3. o componente está excessivamente acoplado.

---

# 34. Ordem recomendada do futuro CSS Base

```text
01. Tokens e tema
02. Reset e primitivas globais
03. Documento e página
04. Cabeçalho e rodapé
05. Capa
06. Hierarquia editorial
07. Prosa e elementos básicos
08. Matemática fundamental
09. Infraestrutura tabular
10. Fonte semântica e helpers de paginação
11. Outline
12. Diagnóstico de tela
13. Media queries de screen
14. Media print
15. Ponto de extensão documentado
```

Componentes opcionais não pertencem ao núcleo.

---

# 35. Ordem recomendada do futuro HTML Base

```text
01. DOCTYPE

02. html lang

03. head
    ├── charset
    ├── viewport
    ├── description
    ├── title
    └── link CSS

04. body.theme--math

05. main#document.document
    ├── cover
    └── source-content
        └── source-section(s)

06. script do paginador
```

O Base deve utilizar placeholders mínimos, e não conteúdo fictício extenso.

---

# 36. Compatibilidade com Chromium

A arquitetura V1.0 assume:

> **Windows + Chrome**

como ambiente oficial.

Devem permanecer comportamentos comprovados:

- `@page` A4;
- `print-color-adjust`;
- folhas em dimensões físicas;
- quebras explícitas;
- outline por headings reais;
- heading de bookmark com texto contínuo;
- screen e print separados.

Não pertencem à arquitetura:

- hacks experimentais de bookmark;
- `aria-label` usado para substituir título de bookmark;
- JavaScript que tente fabricar árvore paralela de bookmarks;
- solução escolhida apenas porque funciona em outro renderer.

---

# 37. Invariantes técnicas

| Invariante | Classificação | Motivo | Exceção possível? |
|---|---|---|---|
| PDF A4 | **OBRIGATÓRIO** | formato físico | somente decisão sistêmica |
| `box-sizing: border-box` global | **OBRIGATÓRIO** | previsibilidade dimensional | arquitetura equivalente |
| ausência de clipping/overflow | **OBRIGATÓRIO** | integridade | não |
| HTML/CSS separados | **OBRIGATÓRIO** | manutenção | exceção normativa documentada |
| fonte semântica separada da paginação | **OBRIGATÓRIO na V1.0** | independência conteúdo/página | nova arquitetura aprovada |
| `.source-section` com contexto | **OBRIGATÓRIO** | header e paginação | valor varia |
| header nas páginas internas | **OBRIGATÓRIO** | localização | texto varia |
| footer + número | **OBRIGATÓRIO** | identidade | texto varia |
| capa canônica | **OBRIGATÓRIO** | identidade | composição adapta-se |
| prosa em uma coluna | **ADAPTÁVEL COM JUSTIFICATIVA** | continuidade | simultaneidade real |
| tokens cromáticos | **OBRIGATÓRIO** | identidade | mudança sistêmica |
| famílias tipográficas | **OBRIGATÓRIO** | identidade | fallback equivalente |
| matemática funcional | **OBRIGATÓRIO** | coerência | componente especializado |
| outline econômico | **OBRIGATÓRIO** | navegação | árvore varia |
| texto contínuo em bookmarks | **OBRIGATÓRIO POR PADRÃO** | Chromium | necessidade comprovada |
| paginador content-agnostic | **OBRIGATÓRIO** | extensibilidade | nova arquitetura |
| atomicidade proporcional | **OBRIGATÓRIO** | paginação pedagógica | não |
| screen/print separados | **OBRIGATÓRIO** | preview ≠ produto | não |
| warnings ausentes no print | **OBRIGATÓRIO** | limpeza do PDF | não |
| geometria 12/17/7/20 mm | **BASE CANÔNICA** | convergência III–V | alteração sistêmica justificada |
| espaçamento de preview | **ADAPTÁVEL** | não afeta produto | sim |

---

# 38. Checklist de conformidade arquitetônica

- [ ] `lang="pt-BR"`, charset UTF-8 e metadados básicos presentes;
- [ ] HTML referencia CSS externo;
- [ ] `body` utiliza tema matemático;
- [ ] existe uma única raiz `.document`;
- [ ] capa ocupa folha própria;
- [ ] `.page` mede A4 sob `border-box`;
- [ ] `@page` usa A4 e margem zero;
- [ ] área útil é produzida pelo padding da folha;
- [ ] páginas internas possuem header, conteúdo e footer;
- [ ] `.source-content` é separada das páginas físicas;
- [ ] cada `.source-section` possui `data-context`;
- [ ] paginador percorre apenas seções de primeiro nível;
- [ ] paginador move, não duplica, conteúdo;
- [ ] `data-keep-count` e `.keep-with-next` protegem apenas dependências curtas;
- [ ] grupos atômicos cabem em folha nova;
- [ ] overflow vertical é detectável;
- [ ] overflow horizontal é auditado;
- [ ] warning não aparece no print;
- [ ] prosa normal permanece em uma coluna;
- [ ] `math-inline`, `math-line` e `math-structural` possuem funções distintas;
- [ ] linha própria não implica centralização;
- [ ] tabelas usam HTML tabular;
- [ ] tipos especializados não foram incorporados acidentalmente ao núcleo;
- [ ] headings correspondem ao outline real;
- [ ] bookmarks não utilizam fragmentação artificial;
- [ ] CSS específico de precedentes não foi herdado sem uso;
- [ ] componentes não redefinem infraestrutura;
- [ ] screen preserva geometria real;
- [ ] print remove sombras, gaps e diagnóstico;
- [ ] PDF é validado em Windows + Chrome.

---

# 39. Questões técnicas abertas

## 39.1 Tokenização de espaçamento

Ainda não há necessidade demonstrada de converter todo spacing recorrente em tokens abstratos.

## 39.2 `--title-section`

O token histórico e o valor real de `.section-title` não coincidem. A futura Base deve eliminar a duplicidade conscientemente.

## 39.3 Tabelas multipágina

A estratégia atual serve para tabelas que cabem numa folha. Tabelas realmente longas exigirão solução própria quando aparecer caso real.

## 39.4 Overflow horizontal automatizado

A detecção vertical está consolidada; warning horizontal pode ser incorporado se demonstrar utilidade.

## 39.5 Paginador inline ou separado

III–V usam script inline curto. A extração futura para `.js` separado deve ser decidida na implementação da Base, e não por preferência abstrata.

## 39.6 Primitivas matemáticas adicionais

Frações, sistemas, matrizes, radicais e notações futuras não devem ser canonizados antes de uso suficiente.

## 39.7 Imagens, gráficos e Geometria

O contrato geral de largura está definido; arquiteturas específicas ainda dependem de casos reais.

## 39.8 Acessibilidade ampliada

A semântica básica está consolidada. Descrições de diagramas e matemática avançada ainda precisam de experiência real.

## 39.9 Compatibilidade além do Chrome

A V1.0 não promete paginação idêntica entre engines.

---

# 40. Relação com o futuro Catálogo de Componentes

A Arquitetura fornece ao Catálogo:

- tokens;
- área física;
- tipografia;
- fluxo;
- matemática fundamental;
- infraestrutura tabular;
- paginação;
- atomicidade;
- screen/print;
- contrato de extensão.

O Catálogo fornecerá:

- nome canônico;
- status;
- nível;
- função;
- quando usar;
- quando não usar;
- HTML;
- seletores;
- variantes;
- comportamento de quebra;
- precedentes.

O Catálogo não redefine o chassi.

---

# 41. Relação com o futuro HTML/CSS Base

Este documento é **especificação**.

Os futuros:

```text
Plano_Matematico_Base.html
Plano_Matematico_Base.css
```

serão a **implementação**.

A Base deverá:

- materializar apenas o núcleo descrito;
- eliminar duplicidades históricas evidentes sem alterar função;
- não transportar CSS morto;
- oferecer pontos de extensão limpos;
- manter placeholders mínimos;
- preservar o paginador content-agnostic;
- ser testada em Windows + Chrome.

A Base não deve ser construída copiando integralmente o Bloco V e apagando conteúdo.

Deve ser construída **a partir desta Arquitetura**, usando precedentes para validação.

---

# 42. Teste de economia — novo Bloco VI

Depois da aprovação desta Arquitetura, um agente não deve precisar abrir III, IV e V apenas para descobrir:

- como funciona uma página;
- quais são as margens;
- como funcionam header/footer;
- como o conteúdo vira páginas;
- como funciona o outline;
- como uma fórmula comum é apresentada;
- como overflow é medido.

O conjunto normal deverá progressivamente tornar-se:

```text
Regras Gerais 3.0
+
Arquitetura Técnica V1.0
+
HTML/CSS Base
+
conteúdo mestre
+
componentes específicos necessários
```

Precedentes passam a ser consultados somente para funções especiais.

---

# 43. Base empírica

A Arquitetura Técnica V1.0 foi consolidada a partir de:

### Documentos de autoridade

- **Arquitetura e Taxonomia Canônica do Sistema de Apostilas — Plano de Estudo Matemático — V1.0**;
- **Regras Gerais para Criação de HTML/CSS — Plano de Estudo Matemático — V3.0**;
- relatórios de classificação e consolidação associados.

### Precedentes técnicos

- **Bloco III — Condicional, Bicondicional e Condições Matemáticas**;
- **Bloco IV — Sentenças Abertas e Quantificadores**;
- **Bloco V — Argumentos, Validade e Demonstração Elementar**.

A convergência III → IV → V sustenta especialmente:

- tokens;
- A4;
- `.document`;
- `.page`;
- `.page-content`;
- capa;
- header/footer;
- fonte semântica;
- `data-context`;
- paginador;
- `keep-with-next`;
- `data-keep-count`;
- outline;
- matemática fundamental;
- infraestrutura tabular;
- screen/print.

Extensões específicas foram deliberadamente excluídas do núcleo quando dependiam do conteúdo particular.

---

# 44. Síntese arquitetônica

A infraestrutura técnica do Plano Matemático pode ser resumida por:

> **CONTEÚDO SEMÂNTICO + CHASSI A4 + PAGINADOR CONTENT-AGNOSTIC + PRIMITIVAS EDITORIAIS = APOSTILA TECNICAMENTE MATERIALIZÁVEL**

O núcleo deve permanecer pequeno porque sua estabilidade é mais valiosa que sua abrangência.

Uma nova necessidade deve seguir:

> **usar a base → usar componente existente → criar extensão local → promover somente se a função se provar geral.**

O objetivo desta arquitetura não é antecipar todos os conteúdos futuros. É fazer com que conteúdos futuros possam nascer sobre uma infraestrutura que já não precisa ser reinventada.

> **Uma apostila herda antes de criar.**

> **Base estável; extensão local.**

> **Herança técnica deve ser intencional.**

> **O passado deve ser condensado em sistema, não reaprendido indefinidamente.**