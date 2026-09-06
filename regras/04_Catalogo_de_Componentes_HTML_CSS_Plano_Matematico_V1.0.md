# Catálogo de Componentes HTML/CSS
## Plano de Estudo Matemático — Versão 1.0

**Documento 04 da Consolidação Pós-Tópico 1.1**  
**Escopo:** biblioteca semântica de componentes opcionais e padrões reutilizáveis aprovados para as apostilas HTML/CSS do Plano de Estudo Matemático.

> **Canônico não significa obrigatório.**
>
> **Um componente existe para resolver uma função editorial identificável; não para preencher uma página.**

---

## 1. Finalidade e escopo

Este Catálogo define quais soluções editoriais reutilizáveis já existem no Plano de Estudo Matemático, qual função cada uma exerce, quando devem ser utilizadas e quando devem ser evitadas.

O documento não substitui:

- a **Arquitetura e Taxonomia Canônica — V1.0**, que define níveis A/B/C/D e critérios de promoção;
- as **Regras Gerais HTML/CSS — V3.0**, que estabelecem conformidade normativa;
- a **Arquitetura Técnica HTML/CSS — V1.0**, que define o chassi herdável de toda apostila.

Este Catálogo concentra principalmente elementos de **Nível B — Canônico Opcional**. Elementos de **Nível C — Específico** aparecem apenas quando vale a pena preservar um precedente sem promovê-lo. Elementos de **Nível A** pertencem à Arquitetura Técnica. Elementos de **Nível D** não são catalogados.

A existência de um componente no Catálogo significa:

> **Quando esta função existir, há uma solução aprovada ou provisoriamente aprovada que deve ser considerada antes da criação de uma nova.**

Não significa:

> **Toda apostila deve utilizar este componente.**

---

## 2. Como utilizar este Catálogo

A consulta normal deve ser curta:

1. identificar a função editorial que precisa ser representada;
2. procurar essa função no **Mapa Geral de Componentes**;
3. abrir somente a ficha relevante;
4. verificar **Usar quando** e **Não usar quando**;
5. reutilizar a estrutura mínima se o componente for adequado;
6. consultar um precedente completo apenas se a implementação concreta exigir contexto adicional.

Se nenhuma ficha resolver a função:

> **criar extensão local primeiro; promover depois, somente se a função se mostrar geral.**

O Catálogo não deve ser lido como galeria estética nem como lista de elementos para “variar” a página.

---

## 3. Relação com os Documentos 01–03

A separação documental é:

```text
DOCUMENTO 01 — ARQUITETURA E TAXONOMIA
“Que tipo de solução é esta e em que nível ela pertence?”

DOCUMENTO 02 — REGRAS GERAIS
“O que deve ser respeitado?”

DOCUMENTO 03 — ARQUITETURA TÉCNICA
“O que toda apostila herda antes de conhecermos seu conteúdo?”

DOCUMENTO 04 — CATÁLOGO DE COMPONENTES
“Quando uma necessidade específica aparece, que solução reutilizável já existe?”
```

Não recebem ficha própria neste Catálogo:

- `.theme--math`;
- `.document`;
- `.page`;
- `.page-content`;
- `.source-content`;
- `.source-section`;
- `.page-header`;
- `.page-footer`;
- `.page--cover`;
- `.section-opening`;
- `.part-opening`;
- `.math-inline`;
- `.math-line`;
- `.math-structural`;
- `.math-text`;
- `.table-wrap`;
- `.outline-root`;
- `.keep-with-next`;
- `data-keep-count`;
- `.atomic-group`;
- paginator;
- comportamento screen/print.

Esses elementos são dependências técnicas da biblioteca, não componentes opcionais.

---

## 4. Critérios de entrada no Catálogo

Uma solução é candidata ao Catálogo quando, em conjunto, satisfaz os seguintes critérios:

1. sua função pode ser descrita sem depender do conteúdo particular que a originou;
2. a mesma função pode reaparecer em outro tópico;
3. a reutilização da solução reduz improvisação;
4. a solução acrescenta compreensão, comparação, investigação, verificação ou organização real;
5. existe implementação HTML/CSS concreta ou padrão editorial suficientemente definido;
6. a solução foi testada em apostila real e, quando aplicável, em PDF final;
7. existem critérios claros para seu uso;
8. existem critérios claros para seu não uso.

Repetição de aparência, por si só, não basta.

> **O Catálogo canoniza funções, não coincidências visuais.**

---

## 5. Status e níveis de maturidade

### CONSOLIDADO

Função estável, reutilização segura, critérios de uso e não uso conhecidos e precedente suficiente em produto real.

### PROVISORIAMENTE CANÔNICO

Função clara e implementação aprovada, mas ainda com evidência limitada a poucos tópicos ou a um único bloco maduro. Pode ser reutilizado com prudência.

### LOCAL / PRECEDENTE

Solução útil que permanece ligada a uma necessidade particular. Deve ser consultada apenas quando uma necessidade futura for realmente comparável.

### DEPRECIADO

Solução que não deve ser utilizada em novas apostilas e que possui substituição declarada.

**Nenhum componente é formalmente depreciado nesta V1.0.**

---

## 6. Anatomia das fichas

Cada componente canônico ou provisório é descrito por:

- **Nome canônico**;
- **Seletor / identificador**;
- **Status**;
- **Nível**;
- **Função**;
- **Usar quando**;
- **Não usar quando**;
- **Conteúdo adequado**;
- **Conteúdo inadequado**, quando necessário;
- **Relação com a prosa**;
- **Estrutura HTML mínima**;
- **Dependências da arquitetura**;
- **Comportamento de paginação**;
- **Outline**;
- **Acessibilidade / semântica**;
- **Variantes**, apenas quando comprovadas;
- **Precedentes**;
- **Observações**.

Os snippets são ilustrativos e mínimos. O CSS detalhado pertence à futura implementação da biblioteca de componentes.

---

## 7. Mapa geral de componentes

| Componente | Seletor principal | Família | Status | Nível | Função curta | Precedente principal |
|---|---|---|---|---|---|---|
| **Definição Formal** | `.definition-box` | Definição | **Consolidado** | B | destacar conteúdo definicional real | Blocos II–V |
| **Enunciado como Objeto de Análise** | `.statement-example` | Objeto de análise | **Consolidado** | B | isolar frase/proposição que será examinada | Blocos I–III |
| **Resposta Curta Destacada** | `.answer-box` | Resposta | **Consolidado** | B | tornar localizável uma resposta breve | Blocos II–V |
| **Tabela de Tradução** | `.translation-table` | Tabela | **Consolidado** | B | relacionar duas representações do mesmo conteúdo | Bloco II |
| **Tabela-Verdade** | `.truth-table` | Tabela matemática | **Consolidado** | B | organizar avaliações lógicas de fórmulas | Blocos II–III |
| **Tabela de Comparação** | `.comparison-table` / tabela comparativa equivalente | Tabela | **Consolidado** | B | comparar propriedades ou critérios lado a lado | Blocos I–IV |
| **Tabela de Análise** | `.analysis-table` | Tabela | **Consolidado** | B | decompor raciocínio segundo critérios explícitos | Blocos III–V |
| **Tabela de Trabalho** | `.worksheet-table` | Prática/tabular | **Consolidado** | B | fornecer estrutura parcialmente vazia para resolução | Blocos II–V |
| **Fala ou Formulação de Estudante** | `.student-quote` | Voz/análise | **Provisoriamente canônico** | B | apresentar fala ou formulação a ser examinada | Blocos I, III–V |
| **Frase-Chave / Resultado de Síntese** | `.key-statement` | Ênfase semântica | **Provisoriamente canônico** | B | destacar resultado curto que merece pausa | Blocos I–III |
| **Bloco de Tentativa** | `.attempt-block` | Investigação | **Provisoriamente canônico** | B | apresentar tentativa para diagnóstico/correção | Bloco V |
| **Pilha de Argumento** | `.argument-stack` | Raciocínio formal | **Provisoriamente canônico** | B | tornar visível a relação premissas → conclusão | Bloco V |
| **Esquema de Demonstração** | `.proof-schema` | Raciocínio formal | **Provisoriamente canônico** | B | organizar passos de prova quando a estrutura importa | Bloco V |
| **Exercício ↔ Gabarito Espelhado** | padrão, sem classe única | Padrão de composição | **Consolidado** | B | reapresentar a mesma estrutura em estado resolvido | Blocos II–V |

### Não promovidos nesta V1.0

Permanecem fora do repertório canônico comum:

- painéis geométricos específicos;
- `structure-panel`;
- `evaluation-panel`;
- `diagnostic-card`;
- `concept-comparison`;
- `reading-panel`;
- `quantifier-reading-grid`;
- `domain-panel-grid`;
- `counterexample-table` como componente independente;
- `domain-investigation-table` como componente independente;
- `inference-pair`;
- `math-sequence` como componente semântico;
- `case-block`, `direction-block` e `scenario-block` como classes canônicas, pois ainda não existe implementação estável suficiente com esses contratos.

---

# 8. Componentes consolidados

## 8.1 Definição Formal

**Nome canônico:** Definição Formal  
**Seletor principal:** `.definition-box`  
**Status:** **CONSOLIDADO**  
**Nível:** **B — Canônico Opcional**

### Função

Apresentar de forma inequivocamente distinguível uma definição formal ou um enunciado cuja função principal seja **fixar o significado de um conceito**.

### Usar quando

- o trecho define explicitamente um termo, relação ou objeto;
- a definição precisa ser reencontrada rapidamente;
- o estudante precisa distinguir “o que o conceito é” da explicação que o prepara ou interpreta.

### Não usar quando

- o trecho é apenas importante;
- é uma conclusão;
- é uma dica;
- é um princípio metodológico;
- é uma observação;
- é uma frase de síntese;
- o parágrafo simplesmente contém linguagem como “podemos dizer” sem exercer função definicional real.

### Conteúdo adequado

- um parágrafo definicional curto ou moderado;
- pequeno conjunto de parágrafos que formam uma única definição;
- lista curta que pertence à própria definição.

### Conteúdo inadequado

- explicação longa;
- exemplo resolvido;
- demonstração;
- exercício;
- várias definições independentes dentro da mesma caixa.

### Relação com a prosa

A prosa normalmente prepara o conceito; a caixa fixa a definição; a prosa seguinte interpreta consequências e limites.

### Estrutura HTML mínima

```html
<p class="definition-box">
  Uma <strong>definição</strong> ...
</p>
```

Para definição composta:

```html
<div class="definition-box definition-box--group">
  <p>...</p>
  <p>...</p>
</div>
```

### Dependências da arquitetura

- tokens canônicos;
- prosa-base;
- `.math-inline`, quando houver notação;
- política de atomicidade.

### Paginação

**B — Preferencialmente atômico quando curto.**

Uma definição comum deve permanecer inteira quando isso for razoável. Não transformar definição longa em unidade impossível de paginar apenas para preservar a caixa.

### Outline

**Não gera bookmark por si só.**

### Acessibilidade / semântica

Pode ser `<p>` ou `<div>` conforme a estrutura interna. Não requer ARIA especial.

### Variantes

- `.definition-box--group`: definição composta por mais de um parágrafo ou lista curta.

### Precedentes

- Bloco II — Proposições Compostas, Conectivos e Tabelas-Verdade;
- Bloco III — Condicional, Bicondicional e Condições Matemáticas;
- Bloco IV — Sentenças Abertas e Quantificadores;
- Bloco V — Argumentos, Validade e Demonstração Elementar.

---

## 8.2 Enunciado como Objeto de Análise

**Nome canônico:** Enunciado como Objeto de Análise  
**Seletor principal:** `.statement-example`  
**Status:** **CONSOLIDADO**  
**Nível:** **B — Canônico Opcional**

### Função

Isolar uma frase, proposição, formulação verbal ou pequeno enunciado que será tratado imediatamente como **objeto da análise**.

### Usar quando

- a explicação seguinte examinará diretamente aquela formulação;
- for pedagogicamente útil separar a frase analisada da prosa que fala sobre ela;
- a formulação precisar ser lida como unidade antes de ser decomposta, simbolizada ou classificada.

### Não usar quando

- a frase pertence naturalmente ao parágrafo;
- é apenas exemplo incidental;
- é uma definição;
- é fala de estudante;
- é resposta;
- é enunciado completo de exercício;
- o isolamento não acrescenta nenhuma função cognitiva.

### Conteúdo adequado

Uma formulação curta ou moderada, verbal, matemática ou híbrida.

### Relação com a prosa

A prosa normalmente introduz a situação, o componente apresenta a formulação e a prosa seguinte a interpreta.

### Estrutura HTML histórica mínima

```html
<blockquote class="statement-example">
  <p>Se p, então q.</p>
</blockquote>
```

### Dependências da arquitetura

- estilos-base de bloco/prosa;
- `.math-inline` e `.math-line`, quando necessários.

### Paginação

**B — Preferencialmente atômico quando curto.**

### Outline

**Não.**

### Acessibilidade / semântica

Os precedentes utilizam `<blockquote>`. Como nem todo `statement-example` é uma citação em sentido estrito, a futura implementação-base pode reavaliar o elemento HTML mantendo a função e o seletor semântico.

Esta V1.0 não renomeia precedentes históricos.

### Variantes

Nenhuma variante canônica definida.

### Precedentes

- Bloco I — Proposição, Valor Lógico e Negação;
- Bloco II — Proposições Compostas, Conectivos e Tabelas-Verdade;
- Bloco III — Condicional, Bicondicional e Condições Matemáticas.

---

## 8.3 Resposta Curta Destacada

**Nome canônico:** Resposta Curta Destacada  
**Seletor principal:** `.answer-box`  
**Helpers/variantes históricas:** `.answer-line`, `.answer-box--text`  
**Status:** **CONSOLIDADO**  
**Nível:** **B — Canônico Opcional**

### Função

Tornar rapidamente localizável uma resposta breve, valor, fórmula, conjunto de alternativas ou conclusão curta do gabarito.

### Usar quando

- a resposta é curta;
- o estudante deve conseguir localizá-la rapidamente antes de ler a justificativa;
- o destaque não substitui a explicação necessária.

### Não usar quando

- a solução inteira é longa;
- a resposta é uma definição;
- o conteúdo exige parágrafos completos;
- o destaque criaria aparência de “card” para toda conclusão;
- a questão avalia raciocínio e o box seria usado como substituto do gabarito comentado.

### Conteúdo adequado

- fórmula curta;
- número ou intervalo;
- alternativa;
- classificação breve;
- frase verbal curta.

### Estrutura HTML mínima

```html
<span class="answer-box">
  ¬(p→q) ≡ p∧¬q
</span>
```

### Dependências da arquitetura

- tokens;
- fonte matemática por padrão;
- `.math-inline`, quando necessário.

### Paginação

O box é normalmente inline/inline-block e **segue a unidade textual que o contém**. Não é unidade de página autônoma.

### Outline

**Não.**

### Acessibilidade / semântica

Não requer ARIA especial. A ordem de leitura continua a mesma da prosa.

### Variantes

- `.answer-box--text`: resposta verbal curta que precisa de fonte editorial e quebra normal;
- `.answer-line`: helper de posicionamento quando a resposta ocupa linha própria; não é componente independente.

### Precedentes

- Blocos II, III, IV e V.

---

## 8.4 Tabela de Tradução

**Nome canônico:** Tabela de Tradução  
**Seletor principal:** `.translation-table`  
**Status:** **CONSOLIDADO**  
**Nível:** **B — Canônico Opcional**

### Função

Relacionar duas ou mais representações equivalentes ou correspondentes de um mesmo conteúdo.

### Usar quando

- o estudante precisa traduzir entre linguagem verbal e simbólica;
- duas representações devem ser lidas em correspondência linha a linha;
- a simultaneidade é mais importante que uma sequência de exemplos separados.

### Não usar quando

- existe apenas um caso;
- a equivalência pode ser expressa de forma mais clara numa frase;
- as colunas não representam correspondência real;
- a tabela é usada apenas para comprimir texto.

### Conteúdo adequado

- linguagem verbal ↔ forma lógica;
- notação ↔ leitura;
- representação A ↔ representação B.

### Estrutura HTML mínima

```html
<div class="table-wrap">
  <table class="translation-table">
    <thead>
      <tr>
        <th scope="col">Linguagem verbal</th>
        <th scope="col">Forma lógica</th>
      </tr>
    </thead>
    <tbody>
      <tr>
        <td>...</td>
        <td>...</td>
      </tr>
    </tbody>
  </table>
</div>
```

### Dependências da arquitetura

- `.table-wrap`;
- infraestrutura HTML de tabelas;
- `.math-inline`.

### Paginação

**D — Tamanho dependente.**

Pequena: manter inteira. Longa: não aumentar indefinidamente a atomicidade; avaliar divisão pedagógica real.

### Outline

**Não.**

### Acessibilidade / semântica

Usar tabela HTML real, `<th>` e `scope` quando aplicável.

### Variantes

Pode combinar com `.worksheet-table` quando uma das representações deve ser produzida pelo estudante.

### Precedentes

- Bloco II — Proposições Compostas, Conectivos e Tabelas-Verdade.

---

## 8.5 Tabela-Verdade

**Nome canônico:** Tabela-Verdade  
**Seletor principal:** `.truth-table`  
**Status:** **CONSOLIDADO**  
**Nível:** **B — Canônico Opcional**

### Função

Representar avaliações lógicas de proposições ou fórmulas de maneira tabular, preservando simultaneamente valores de entrada, etapas intermediárias e resultado.

### Usar quando

- a tabela-verdade é o próprio instrumento matemático da análise;
- valores precisam ser comparados por linha;
- equivalência, falsidade, conectivos ou avaliações exigem visão simultânea.

### Não usar quando

- uma única avaliação basta;
- a tabela apenas repete uma explicação já completa;
- o número de colunas torna o A4 ilegível;
- o conteúdo não é verdadeiramente tabular.

### Estrutura HTML mínima

```html
<div class="table-wrap">
  <table class="truth-table">
    <thead>
      <tr>
        <th scope="col">p</th>
        <th scope="col">q</th>
        <th scope="col">p→q</th>
      </tr>
    </thead>
    <tbody>
      ...
    </tbody>
  </table>
</div>
```

### Dependências da arquitetura

- infraestrutura tabular;
- `.math-inline`;
- tokens.

### Paginação

**C — Atômico por natureza dentro do limite normal.**

Uma tabela-verdade deve ser percebida como unidade. Se não couber numa página nova, a solução não é permitir corte arbitrário: revisar número de colunas, escala local ou estratégia de representação.

### Outline

**Não.**

### Acessibilidade / semântica

Tabela HTML real, cabeçalhos explícitos.

### Variantes

Os precedentes possuem modificadores técnicos como:

- `--compact`;
- `--single`;
- `--wide`;
- `--dense`;
- `--six`;
- `--seven`.

Esses modificadores representam **acomodações dimensionais**, não componentes semânticos distintos.

A futura biblioteca pode racionalizá-los; não devem ser multiplicados sem necessidade real.

Também pode combinar com `.worksheet-table`.

### Precedentes

- Bloco II — Proposições Compostas, Conectivos e Tabelas-Verdade;
- Bloco III — Condicional, Bicondicional e Condições Matemáticas.

---

## 8.6 Tabela de Comparação

**Nome canônico:** Tabela de Comparação  
**Seletor principal histórico:** `.comparison-table`  
**Status:** **CONSOLIDADO**  
**Nível:** **B — Canônico Opcional**

### Função

Contrastar propriedades, condições, definições ou comportamentos segundo critérios compartilhados.

### Usar quando

- existem pelo menos dois objetos comparáveis;
- os mesmos critérios se aplicam às alternativas;
- ler por linha/coluna torna a diferença mais evidente que dois parágrafos separados.

### Não usar quando

- não há critérios comuns;
- a comparação é apenas narrativa;
- uma lista curta resolve melhor;
- a tabela só serve para preencher espaço ou alinhar frases.

### Conteúdo adequado

- conceito A × conceito B;
- condição necessária × suficiente;
- propriedade × comportamento;
- formas relacionadas sob critérios comuns.

### Estrutura HTML mínima

```html
<div class="table-wrap">
  <table class="comparison-table">
    <thead>...</thead>
    <tbody>...</tbody>
  </table>
</div>
```

### Dependências da arquitetura

Infraestrutura tabular.

### Paginação

**D — Tamanho dependente.**

### Outline

**Não.**

### Acessibilidade / semântica

Tabela real apenas quando a relação for genuinamente tabular.

### Variantes

Não confundir com grids visuais específicos, como `.concept-comparison`, que permanecem precedentes locais nesta V1.0.

### Precedentes

- Bloco I — Proposição, Valor Lógico e Negação;
- comparações tabulares dos Blocos II–IV.

---

## 8.7 Tabela de Análise

**Nome canônico:** Tabela de Análise  
**Seletor principal:** `.analysis-table`  
**Status:** **CONSOLIDADO**  
**Nível:** **B — Canônico Opcional**

### Função

Decompor um raciocínio, caso, avaliação ou objeto segundo critérios explícitos que o estudante precisa acompanhar simultaneamente.

### Usar quando

- as colunas representam perguntas ou critérios de análise;
- o estudante precisa relacionar estado inicial, operação, resultado ou justificativa;
- a comparação tabular revela a estrutura do raciocínio.

### Não usar quando

- a tabela é apenas lista de dados;
- uma sequência vertical de passos é mais natural;
- a quantidade de texto em cada célula torna a leitura tabular pior que prosa.

### Estrutura HTML mínima

```html
<div class="table-wrap">
  <table class="analysis-table">
    <thead>...</thead>
    <tbody>...</tbody>
  </table>
</div>
```

### Dependências da arquitetura

- infraestrutura tabular;
- `.math-inline`;
- eventualmente `.worksheet-table`.

### Paginação

**D — Tamanho dependente.**

### Outline

**Não.**

### Acessibilidade / semântica

Cabeçalhos devem nomear critérios reais de análise.

### Variantes

Modificadores de conteúdo como:

- `counterexample-table`;
- `domain-investigation-table`;
- `validity-analysis-table`;
- `chain-table`;

devem ser tratados como especializações locais **sobre a família de análise**, não como novos componentes canônicos automaticamente.

### Precedentes

- Bloco III — Condicional, Bicondicional e Condições Matemáticas;
- Bloco IV — Sentenças Abertas e Quantificadores;
- Bloco V — Argumentos, Validade e Demonstração Elementar.

---

## 8.8 Tabela de Trabalho

**Nome canônico:** Tabela de Trabalho / Worksheet  
**Seletor principal:** `.worksheet-table`  
**Status:** **CONSOLIDADO**  
**Nível:** **B — Canônico Opcional**

### Função

Transformar uma tabela já semanticamente adequada em uma estrutura parcialmente vazia para que o estudante registre análise, tradução ou resultado.

### Usar quando

- a própria tabela é instrumento de resolução;
- o preenchimento das células faz parte da atividade;
- a mesma estrutura poderá reaparecer preenchida no gabarito.

### Não usar quando

- o estudante deveria construir a estrutura por conta própria;
- o preenchimento é trivial e não acrescenta aprendizagem;
- a tabela antecipa demais o raciocínio;
- campos vazios substituem uma pergunta que deveria ser formulada verbalmente.

### Conteúdo adequado

`worksheet-table` funciona como **modificador funcional**, em composição com uma família tabular:

```html
<table class="translation-table worksheet-table">
  ...
</table>
```

```html
<table class="truth-table worksheet-table">
  ...
</table>
```

```html
<table class="analysis-table worksheet-table">
  ...
</table>
```

### Dependências da arquitetura

- infraestrutura tabular;
- componente-base de tabela correspondente.

### Paginação

Herda o comportamento da tabela que modifica. Não cria permissão para quebrar uma tabela que precisa ser percebida inteira.

### Outline

**Não.**

### Acessibilidade / semântica

Células vazias devem permanecer compreensíveis pelo contexto dos cabeçalhos. Espaços de resposta não devem depender apenas de cor.

### Variantes

Nenhuma variante semântica adicional consolidada.

### Precedentes

- Blocos II, III, IV e V.

---

# 9. Componentes provisoriamente canônicos

## 9.1 Fala ou Formulação de Estudante

**Nome canônico:** Fala ou Formulação de Estudante  
**Seletor principal:** `.student-quote`  
**Status:** **PROVISORIAMENTE CANÔNICO**  
**Nível:** **B — Canônico Opcional**

### Função

Apresentar como objeto separado uma fala, resposta, pergunta, interpretação ou formulação atribuída a um estudante real ou hipotético, para posterior leitura, avaliação ou comentário.

### Usar quando

- a voz do estudante é pedagogicamente relevante;
- a formulação será analisada como raciocínio, dúvida ou resposta;
- distinguir voz autoral e voz examinada evita ambiguidade.

### Não usar quando

- o conteúdo é apenas um enunciado neutro;
- a formulação é do próprio texto autoral;
- o componente seria usado somente para criar uma caixa visual;
- a frase já está adequadamente integrada à prosa.

### Estrutura HTML mínima

```html
<blockquote class="student-quote">
  <p>“...”</p>
</blockquote>
```

### Dependências da arquitetura

- `blockquote`;
- tokens;
- matemática fundamental, quando necessário.

### Paginação

**B — Preferencialmente atômico quando curto.**

### Outline

**Não.**

### Acessibilidade / semântica

`<blockquote>` é semanticamente apropriado quando a fala é apresentada como citação ou formulação distinta.

### Variantes / composições

Pode aparecer dentro de `.attempt-block` ou, em casos justificados, compartilhar a estrutura externa de uma demonstração transcrita.

A composição não deve criar caixa dentro de caixa sem nova função.

### Precedentes

- Bloco I;
- Bloco III;
- Bloco IV;
- Bloco V.

### Observação

O status permanece provisório porque o recurso depende fortemente do método pedagógico de cada tópico e não deve se tornar vício estilístico.

---

## 9.2 Frase-Chave / Resultado de Síntese

**Nome canônico:** Frase-Chave / Resultado de Síntese  
**Seletor principal:** `.key-statement`  
**Status:** **PROVISORIAMENTE CANÔNICO**  
**Nível:** **B — Canônico Opcional**

### Função

Destacar uma conclusão curta, princípio operacional ou resultado de síntese que precisa receber pausa perceptiva, sem transformá-lo em definição formal.

### Usar quando

- a frase resume uma relação já construída;
- o destaque facilita reencontro e consolidação;
- a frase possui autonomia suficiente para ser lida isoladamente.

### Não usar quando

- o trecho é definição: usar `.definition-box`;
- é apenas uma frase importante do parágrafo;
- o destaque existe para preencher espaço;
- vários `key-statement` seriam necessários em sequência;
- o componente substituiria uma síntese textual bem integrada.

### Estrutura HTML mínima

```html
<p class="key-statement">
  ...resultado curto...
</p>
```

### Dependências da arquitetura

Prosa-base e tokens.

### Paginação

**B — Preferencialmente atômico quando curto.**

### Outline

**Não.**

### Precedentes

- Blocos I, II e III.

### Observação

O seletor permanece no patrimônio técnico posterior, mas a ausência de uso relevante nos Blocos IV e V recomenda prudência.

Não deve ser promovido a destaque padrão de toda seção.

---

## 9.3 Bloco de Tentativa

**Nome canônico:** Bloco de Tentativa  
**Seletor principal:** `.attempt-block`  
**Status:** **PROVISORIAMENTE CANÔNICO**  
**Nível:** **B — Canônico Opcional**

### Função

Apresentar uma tentativa de resolução ou raciocínio que será analisada, diagnosticada, corrigida, reorganizada ou completada.

### Usar quando

- o estudante precisa auditar um raciocínio existente;
- a ordem dos passos é parte da questão;
- existe distinção entre “tentativa apresentada” e “análise do material”.

### Não usar quando

- a solução apresentada já é exemplo resolvido normal;
- existe apenas uma frase de estudante: considerar `.student-quote`;
- o conteúdo é uma demonstração correta que não precisa ser diagnosticada;
- o bloco seria apenas um contêiner decorativo.

### Conteúdo adequado

- pequena cadeia de passos;
- justificativas apresentadas;
- fala de estudante interna;
- matemática relevante à tentativa.

### Estrutura HTML mínima

```html
<div class="attempt-block">
  <div class="minor-title">Passo 1</div>

  <div class="math-line">
    ...
  </div>

  <p>Justificativa apresentada:</p>

  <blockquote class="student-quote">
    <p>...</p>
  </blockquote>
</div>
```

### Dependências da arquitetura

- `.minor-title`;
- matemática fundamental;
- eventualmente `.student-quote`.

### Paginação

**D — Tamanho dependente.**

Tentativa curta pode permanecer atômica. Tentativa longa não deve ser tornada indivisível apenas porque utiliza o mesmo componente.

### Outline

**Não.**

### Precedentes

- Bloco V — Argumentos, Validade e Demonstração Elementar.

### Observação

O `diagnostic-card` do Bloco II constitui precedente anterior de função aparentada, mas não é promovido separadamente nesta versão.

O `attempt-block` é mais geral e menos ligado a um formato específico de resposta.

---

## 9.4 Pilha de Argumento

**Nome canônico:** Pilha de Argumento  
**Seletor principal:** `.argument-stack`  
**Subestruturas:** `.argument-premises`, `.argument-premise`, `.argument-conclusion`, `.therefore-marker`  
**Status:** **PROVISORIAMENTE CANÔNICO**  
**Nível:** **B — Canônico Opcional**

### Função

Representar espacialmente uma estrutura inferencial em que uma ou mais premissas sustentam uma conclusão.

### Usar quando

- a distinção entre premissas e conclusão é parte do conceito;
- o argumento precisa ser lido como estrutura, e não como lista de fórmulas;
- o marcador de conclusão e a separação física ajudam a perceber função inferencial.

### Não usar quando

- existem apenas fórmulas sucessivas sem relação premissa/conclusão;
- uma frase inline resolve;
- a estrutura é cadeia de transformação algébrica;
- o componente seria usado apenas para centralizar matemática.

### Estrutura HTML mínima

```html
<div class="argument-stack">
  <div class="argument-premises">
    <div class="argument-premise">p→q</div>
    <div class="argument-premise">p</div>
  </div>

  <div class="argument-conclusion">
    <span class="therefore-marker">∴</span>
    <span>q</span>
  </div>
</div>
```

### Dependências da arquitetura

- fonte matemática;
- tokens;
- política de atomicidade.

### Paginação

**C — Atômico por natureza** para argumentos de dimensão normal.

Se uma estrutura inferencial se tornar extensa a ponto de não caber, provavelmente já não pertence a uma única `argument-stack`.

### Outline

**Não.**

### Acessibilidade / semântica

A ordem DOM deve preservar premissas antes da conclusão. O símbolo `∴` não substitui textualização quando a compreensão exigir explicação.

### Precedentes

- Bloco V — Argumentos, Validade e Demonstração Elementar.

---

## 9.5 Esquema de Demonstração

**Nome canônico:** Esquema de Demonstração  
**Seletor principal:** `.proof-schema`  
**Subestruturas históricas:** `.proof-step`, `.proof-step__role`, `.proof-justification`  
**Status:** **PROVISORIAMENTE CANÔNICO**  
**Nível:** **B — Canônico Opcional**

### Função

Organizar explicitamente passos ou papéis de uma demonstração quando a estrutura da prova — hipótese, transformação, justificativa, conclusão ou dependência entre etapas — é objeto pedagógico.

### Usar quando

- o estudante precisa perceber a arquitetura da demonstração;
- os passos precisam ser auditados separadamente;
- identificar papéis ou justificativas acrescenta compreensão.

### Não usar quando

- a demonstração em prosa contínua já é clara;
- cada fórmula seria transformada artificialmente em “passo”;
- o esquema alonga e fragmenta uma prova simples;
- o componente é usado apenas por aparência de formalidade.

### Estrutura HTML mínima

```html
<div class="proof-schema">
  <div class="proof-step">
    <div class="proof-step__role">Hipótese</div>
    <p>...</p>
  </div>

  <div class="proof-step">
    <div class="proof-step__role">Conclusão</div>
    <p>...</p>
  </div>
</div>
```

### Dependências da arquitetura

- prosa;
- `.math-inline`;
- `.math-line`;
- `.minor-title` ou rótulo equivalente;
- tokens.

### Paginação

**D — Tamanho dependente.**

Os precedentes tratam esquemas curtos como unidades coesas. Em demonstração longa, não se deve impor atomicidade ao conjunto inteiro se isso produzir overflow ou grandes distorções de paginação.

Proteger passos pequenos e dependências locais é preferível.

### Outline

**Não.**

### Acessibilidade / semântica

Papéis visuais não substituem frases necessárias à leitura lógica da prova.

### Composições

Pode aparecer em uma fala transcrita, como `student-quote + proof-schema`, quando a função dupla for real:

- fala do estudante;
- estrutura de demonstração.

Não usar a combinação apenas para obter duas camadas de destaque.

### Precedentes

- Bloco V — Argumentos, Validade e Demonstração Elementar.

---

# 10. Padrões canônicos de composição

## 10.1 Exercício ↔ Gabarito Espelhado

**Tipo:** padrão editorial, não classe única  
**Status:** **CONSOLIDADO**  
**Nível:** **B — Canônico Opcional**

### Função

Reutilizar a mesma estrutura visual no exercício e no gabarito, primeiro como estado de investigação e depois como estado resolvido.

```text
ESTRUTURA DE TRABALHO
        ↓
MESMA ESTRUTURA PREENCHIDA
```

### Usar quando

- a comparação direta ajuda o estudante a localizar seu erro;
- a estrutura é parte do método de resolução;
- o gabarito pode completar o mesmo objeto sem precisar reinventar a representação.

### Não usar quando

- o exercício pede construção livre da própria representação;
- a estrutura pronta entrega o caminho que deveria ser descoberto;
- o gabarito exige explicação muito diferente;
- a repetição visual acrescentaria volume sem benefício.

### Formas comprovadas

- `.translation-table + .worksheet-table` → mesma tradução preenchida;
- `.truth-table + .worksheet-table` → tabela-verdade resolvida;
- `.analysis-table + .worksheet-table` → análise completa;
- painéis investigativos locais, quando o mesmo desenho é pedagogicamente necessário.

### Paginação

Cada instância segue o contrato do componente concreto utilizado.

### Precedentes

- Blocos II, III, IV e V, com consolidação especialmente forte em IV e V.

---

## 10.2 Tabela-base + Modificador de Trabalho

**Tipo:** padrão de composição  
**Status:** **CONSOLIDADO**

Uma tabela pode expressar simultaneamente:

1. **o que ela representa** — `translation-table`, `truth-table`, `analysis-table`;
2. **o estado pedagógico** — `worksheet-table`.

Exemplo:

```html
<table class="analysis-table worksheet-table">
  ...
</table>
```

Essa composição é preferível a criar uma classe nova para cada combinação de conteúdo e exercício.

---

## 10.3 Tentativa → Diagnóstico

**Tipo:** padrão pedagógico  
**Status:** **PROVISORIAMENTE CANÔNICO**

```text
TENTATIVA APRESENTADA
        ↓
LOCALIZAÇÃO DO PRIMEIRO PROBLEMA
        ↓
EXPLICAÇÃO DO PORQUÊ
        ↓
CORREÇÃO / REORGANIZAÇÃO
```

Pode utilizar `attempt-block`, `student-quote`, tabela de análise ou prosa.

Não existe uma classe única que represente todo o movimento.

---

## 10.4 Texto prepara → componente organiza → texto interpreta

**Tipo:** padrão editorial  
**Status:** **CONSOLIDADO**

Um componente não deve ser abandonado no fluxo sem preparação ou interpretação quando carrega relação conceitual nova.

Esse padrão não obriga a existência de componente:

> **se a prosa basta, usa-se prosa.**

---

# 11. Regras de composição entre componentes

## 11.1 Composição deve acrescentar função

Combinar duas classes só é adequado quando cada uma representa um papel distinto.

Composições comprovadas:

```text
translation-table + worksheet-table
truth-table + worksheet-table
analysis-table + worksheet-table
attempt-block → student-quote interno
student-quote + proof-schema, em caso específico
```

## 11.2 Não empilhar decoração

Evitar:

```text
definition-box
  └── student-quote
      └── card genérico
          └── outro painel
```

se cada camada não acrescentar função semântica própria.

## 11.3 Uma função, uma camada suficiente

Se o objetivo é definição, usar definição.

Se o objetivo é fala de estudante, usar fala.

Não acrescentar um terceiro invólucro apenas para aumentar contraste.

---

# 12. Relação com paginação

O Catálogo utiliza quatro comportamentos de referência:

| Código | Comportamento | Exemplos |
|---|---|---|
| **A** | naturalmente quebrável | composição textual longa sem dependência rígida |
| **B** | preferencialmente atômico quando curto | definição, statement, student-quote, key-statement |
| **C** | atômico por natureza dentro do tamanho normal | argument-stack, truth-table comum |
| **D** | tamanho dependente; não prender o conjunto inteiro por padrão | translation-table, comparison-table, analysis-table, worksheet-table, proof-schema, attempt-block |

Regra geral:

> **A classe não deve transformar conteúdo grande em bloco indivisível apenas por existir.**

Se um componente de tamanho D crescer, a solução deve preservar unidades menores e dependências reais.

---

# 13. Relação com outline e semântica

Componentes **não geram bookmarks por padrão**.

Bookmark depende da função de navegação da unidade, não da aparência ou da importância local do componente.

Portanto:

- `.definition-box` → não;
- `.statement-example` → não;
- `.student-quote` → não;
- `.answer-box` → não;
- tabelas → não;
- `.argument-stack` → não;
- `.proof-schema` → não;
- `.attempt-block` → não.

Se um componente estiver dentro de uma seção que possui heading real, o heading pertence à seção, não ao componente.

---

# 14. Componentes e acessibilidade

Princípios mínimos:

- dados reais usam `<table>`;
- cabeçalhos usam `<th>` e `scope` quando adequado;
- citações/falas usam `<blockquote>` quando semanticamente justificadas;
- listas reais usam `<ul>`/`<ol>`;
- headings são reservados a unidades de navegação;
- elementos decorativos não recebem significado artificial;
- ARIA é usado apenas quando melhora a semântica real.

A implementação histórica de `.statement-example` em `<blockquote>` permanece como precedente, mas sua semântica poderá ser refinada futuramente se a biblioteca-base distinguir citação de “objeto de análise” não citado.

---

# 15. Precedentes locais não promovidos

Esta seção registra soluções úteis que **não** fazem parte do repertório canônico comum na V1.0.

## 15.1 Figuras e painéis geométricos do Bloco I

**Função local:** concretizar proposições, classificações e relações por objetos geométricos.  
**Origem:** Bloco I.  
**Por que permanece local:** fortemente dependente do conteúdo introdutório específico; não existe ainda biblioteca geométrica geral.  
**Reconsiderar se:** Geometria ou outros tópicos produzirem recorrência de funções gráficas equivalentes.

## 15.2 `structure-panel`

**Função local:** revelar alcance, conectivo principal e estrutura interna de fórmulas.  
**Origem:** Bloco II.  
**Por que permanece local:** é uma solução eficiente para análise de estrutura lógica, mas seu contrato ainda está ligado a esse tipo de fórmula.  
**Reconsiderar se:** reaparecer em análise algébrica ou estrutural de expressões com a mesma função abstrata.

## 15.3 `evaluation-panel`

**Função local:** permitir escolha ou inspeção de avaliações de componentes lógicos.  
**Origem:** Bloco II.  
**Por que permanece local:** a atividade possui forma muito específica; tabela ou worksheet resolve muitos casos aparentados.

## 15.4 `diagnostic-card`

**Função local:** apresentar raciocínio de estudante com campos explícitos de avaliação e correção.  
**Origem:** Bloco II.  
**Por que permanece local:** a função geral de diagnóstico posterior é mais bem coberta por `student-quote`, `attempt-block`, `worksheet-table` e prosa.  
**Reconsiderar se:** o formato “raciocínio + avaliação + correção” reaparecer de maneira estável como unidade autônoma.

## 15.5 `concept-comparison`

**Função local:** comparar bicondicional e equivalência lógica em dois painéis paralelos.  
**Origem:** Bloco III.  
**Por que permanece local:** a função geral de comparação já possui solução canônica tabular; o grid específico só se justifica quando a simultaneidade textual não é naturalmente tabular.  
**Reconsiderar se:** grids conceituais paralelos se tornarem recorrentes em novos tópicos.

## 15.6 Painéis de leitura e quantificadores

Incluem:

- `.reading-panel`;
- `.quantifier-reading-grid`;
- `.domain-panel-grid`;
- marcações específicas de quantificadores.

**Função local:** tornar visíveis domínio, universalidade, existência, testemunhos e exceções.  
**Origem:** Bloco IV.  
**Por que permanecem locais:** a forma está ligada à semântica dos quantificadores; ainda não há função abstrata suficientemente testada fora desse contexto.  
**Reconsiderar se:** a mesma estrutura surgir em funções, conjuntos, probabilidade ou outros tópicos com contrato equivalente.

## 15.7 `counterexample-table` e `domain-investigation-table`

**Função local:** especializar `.analysis-table` para conteúdo de contraexemplo ou domínio.  
**Origem:** Bloco IV.  
**Por que permanecem locais:** a família canônica é `analysis-table`; esses seletores representam principalmente colunas, larguras e ênfases próprias do conteúdo.  
**Reconsiderar se:** surgirem múltiplas apostilas com o mesmo contrato semântico.

## 15.8 `inference-pair`

**Função local:** comparar formas de inferência em paralelo.  
**Origem:** Bloco V.  
**Por que permanece local:** ainda existe apenas um contexto forte e a função pode ser satisfeita por comparação tabular ou por duas estruturas de argumento.  
**Reconsiderar se:** pares de formas inferenciais se tornarem padrão recorrente.

## 15.9 `math-sequence`

**Função local/técnica:** agrupar pequenas linhas matemáticas que formam uma sequência.  
**Origem:** Bloco V.  
**Por que não é componente canônico:** funciona mais como helper de agrupamento do que como unidade semântica autônoma. A Arquitetura já fornece atomicidade e matemática fundamental.  
**Reconsiderar se:** surgir contrato matemático próprio que não seja resolvido por `.atomic-group` + `.math-line`.

## 15.10 `scenario-block`, `case-block` e `direction-block`

Esses nomes aparecem como **candidatos conceituais** na consolidação, mas não possuem evidência técnica suficiente de seletor ou contrato estável nos precedentes maduros.

**Status:** não promovidos.  
**Reconsiderar se:** uma função recorrente for implementada e sobreviver a novos PDFs e preflights.

---

# 16. Componentes depreciados

**Nenhum componente formalmente depreciado na V1.0.**

A existência de precedentes locais que não devem ser copiados automaticamente não equivale a depreciação.

Um documento antigo pode continuar correto usando sua solução local.

---

# 17. Processo de promoção futura

A promoção deve permanecer simples:

```text
SOLUÇÃO LOCAL
    ↓
A FUNÇÃO REAPARECE
    ↓
A FUNÇÃO PODE SER DESCRITA SEM O EXEMPLO ORIGINAL
    ↓
A IMPLEMENTAÇÃO É TESTADA EM NOVA APOSTILA
    ↓
USO E NÃO USO FICAM CLAROS
    ↓
PROMOÇÃO PARA O CATÁLOGO
```

A promoção não deve ocorrer porque:

- a solução ficou bonita;
- a classe apareceu duas vezes por cópia;
- o CSS já existe;
- uma nova categoria deixaria o Catálogo “mais completo”.

---

# 18. Rebaixamento e depreciação

Um componente catalogado pode futuramente:

- ser fundido com uma família mais geral;
- tornar-se apenas variante;
- ser rebaixado a precedente;
- ser formalmente depreciado.

Se houver depreciação, registrar:

```text
STATUS: DEPRECIADO
SUBSTITUIR POR: <componente/padrão>
MOTIVO: <razão funcional ou técnica>
```

Não remover silenciosamente do Catálogo um seletor ainda presente em documentos congelados.

---

# 19. Relação com o futuro CSS Base

A implementação futura deve distinguir conceitualmente:

```text
BASE NÚCLEO
→ infraestrutura do Documento 03

CAMADA / BIBLIOTECA DE COMPONENTES
→ componentes do Documento 04
```

Esta V1.0 não decide se os dois grupos viverão:

- no mesmo arquivo CSS;
- em dois arquivos;
- em módulos separados.

A decisão deve priorizar:

- simplicidade de uso;
- remoção de CSS morto;
- clareza de dependências;
- facilidade de fornecer ao Codex somente o necessário.

O HTML Base não precisa instanciar todos os componentes.

O Catálogo é a referência para inseri-los quando a função existir.

---

# 20. Checklist para escolher um componente

Antes de inserir qualquer componente, verificar:

- [ ] Qual função precisa ser representada?
- [ ] Essa função já existe no mapa do Catálogo?
- [ ] O componente é consolidado ou provisório?
- [ ] O conteúdo satisfaz **Usar quando**?
- [ ] Alguma condição de **Não usar quando** se aplica?
- [ ] Prosa simples resolveria melhor?
- [ ] Matemática fundamental resolveria melhor?
- [ ] Uma tabela genérica resolveria melhor?
- [ ] O componente acrescenta percepção ou apenas contraste visual?
- [ ] O componente cabe na área útil?
- [ ] Seu comportamento de quebra é adequado ao tamanho real?
- [ ] Ele antecipa indevidamente a resposta?
- [ ] É necessário consultar um precedente completo?

Se não houver solução adequada:

> **criar extensão local primeiro.**

---

# 21. Checklist de auditoria de nova implementação

- [ ] Nenhum elemento da Arquitetura Técnica foi recriado como componente.
- [ ] Nenhum microajuste local virou classe semântica geral.
- [ ] O componente usado possui função independente do exemplo.
- [ ] O componente não foi escolhido apenas porque já existia.
- [ ] Não há duplicação desnecessária entre componente e prosa.
- [ ] Não há caixa dentro de caixa sem função distinta.
- [ ] Tabelas representam relações realmente tabulares.
- [ ] Modificadores dimensionais não foram transformados em novos componentes.
- [ ] Componentes provisórios foram usados com prudência.
- [ ] A paginação respeita o contrato do componente.
- [ ] O componente não gera bookmark indevido.
- [ ] A semântica HTML é adequada.
- [ ] A atividade não revela resposta por aparência.

---

# 22. Teste de usabilidade para agentes

## Caso A — “Preciso apresentar uma definição formal.”

Consultar:

> **Definição Formal → `.definition-box` → Consolidado → usar quando o trecho realmente define.**

Não é necessário abrir os Blocos II–V.

## Caso B — “Preciso mostrar um argumento com premissas e conclusão.”

Consultar:

> **Pilha de Argumento → `.argument-stack` → Provisoriamente canônico → estrutura inferencial.**

O precedente do Bloco V só precisa ser aberto se houver uma forma mais complexa que a ficha mínima.

## Caso C — “Preciso que o estudante preencha uma tabela e depois veja a mesma tabela resolvida.”

Consultar:

> **Tabela apropriada + `.worksheet-table` + padrão Exercício ↔ Gabarito Espelhado.**

## Caso D — “Preciso criar um diagrama novo para um conceito de Geometria.”

Se nenhuma ficha resolver a função:

> **extensão local primeiro.**

Não criar automaticamente um componente canônico.

---

# 23. Questões abertas

1. `.proof-schema` continuará útil em demonstrações de Álgebra, Teoria dos Números e Geometria ou permanecerá associado ao ensino introdutório de prova?
2. `.attempt-block` será transversal a outros tópicos ou continuará concentrado em auditoria de raciocínio lógico?
3. `.key-statement` deve permanecer componente próprio ou sua função será absorvida por prosa e sínteses editoriais?
4. O seletor `.statement-example` deve manter `<blockquote>` como estrutura principal quando o conteúdo não for literalmente citado?
5. Comparações paralelas não tabulares, como `.concept-comparison`, reaparecerão com frequência suficiente para justificar componente próprio?
6. As famílias tabulares precisarão de API mais explícita de variantes dimensionais no futuro CSS Base?
7. A biblioteca de componentes será incorporada ao CSS Base ou separada em camada própria?
8. Geometria exigirá biblioteca gráfica específica?
9. Gráficos estatísticos, diagramas de funções e representações cartesianas formarão nova família de componentes?
10. Painéis de domínio e leitura do Bloco IV podem ser abstraídos para uma família “painel de casos” sem perder sua função original?
11. Um componente formal de “caso” ou “direção” surgirá em tópicos futuros com implementação suficientemente estável?

Essas questões permanecem abertas até que novos conteúdos forneçam evidência real.

---

# 24. Base empírica

Este Catálogo foi consolidado a partir de:

### Documentos de autoridade

- **Arquitetura e Taxonomia Canônica do Sistema de Apostilas — Plano de Estudo Matemático — V1.0**;
- **Regras Gerais para Criação de HTML/CSS — Plano de Estudo Matemático — V3.0**;
- **Arquitetura Técnica HTML/CSS — Plano de Estudo Matemático — V1.0**;
- relatórios de classificação e consolidação associados disponíveis no projeto.

### Precedentes do Tópico 1.1 — Lógica Matemática

- **Bloco I — Proposição, Valor Lógico e Negação**;
- **Bloco II — Proposições Compostas, Conectivos e Tabelas-Verdade**;
- **Bloco III — Condicional, Bicondicional e Condições Matemáticas**;
- **Bloco IV — Sentenças Abertas e Quantificadores**;
- **Bloco V — Argumentos, Validade e Demonstração Elementar**.

Os Blocos III–V foram considerados os precedentes técnicos mais maduros. Blocos I–II foram utilizados quando necessários para confirmar componentes anteriores, especialmente:

- `statement-example`;
- tabelas de tradução;
- tabelas-verdade;
- comparação;
- estruturas iniciais de prática e diagnóstico.

---

# 25. Síntese canônica

O repertório desta V1.0 pode ser resumido em três grupos.

### Componentes consolidados

```text
Definição Formal
Enunciado como Objeto de Análise
Resposta Curta Destacada
Tabela de Tradução
Tabela-Verdade
Tabela de Comparação
Tabela de Análise
Tabela de Trabalho
Exercício ↔ Gabarito Espelhado — padrão
```

### Componentes provisoriamente canônicos

```text
Student Quote
Key Statement
Attempt Block
Argument Stack
Proof Schema
```

### Precedentes que permanecem locais

```text
figuras geométricas específicas
structure-panel
evaluation-panel
diagnostic-card
concept-comparison
painéis de quantificadores/domínio
counterexample/domain tables como componentes independentes
inference-pair
math-sequence
case/direction/scenario blocks ainda não estabilizados
```

A biblioteca deve crescer lentamente.

> **Se a prosa basta, use prosa.**
>
> **Se a infraestrutura basta, não crie componente.**
>
> **Se já existe componente adequado, reutilize.**
>
> **Se a função é nova, extensão local primeiro.**
>
> **Componentes devem ser consultáveis, não onipresentes.**
>
> **O passado deve ser condensado em sistema, não reaprendido indefinidamente.**