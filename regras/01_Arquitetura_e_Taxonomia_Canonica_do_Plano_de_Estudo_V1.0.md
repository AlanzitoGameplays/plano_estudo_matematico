# Arquitetura e Taxonomia Canônica do Sistema de Apostilas
## Plano de Estudo Matemático — Versão 1.0

**Documento 01 da Consolidação Pós-Tópico 1.1**  
**Status:** Fundação arquitetônica do sistema editorial  
**Norma vigente durante sua elaboração:** Regras Gerais HTML/CSS do Plano Matemático — Versão 2.2

---

## 1. Finalidade do documento

Este documento define a arquitetura conceitual do sistema de apostilas do Plano de Estudo Matemático. Sua finalidade não é especificar código, substituir as Regras Gerais vigentes, criar um template técnico ou descrever detalhadamente o uso de agentes. Sua função é anterior a essas tarefas: estabelecer **o que pertence ao sistema, em que nível pertence, por que pertence e como novas decisões deverão ser classificadas no futuro**.

A consolidação parte da experiência acumulada na produção das cinco apostilas definitivas do Tópico 1.1 — Lógica Matemática:

- Bloco I — Proposição, Valor Lógico e Negação;
- Bloco II — Proposições Compostas, Conectivos e Tabelas-Verdade;
- Bloco III — Condicional, Bicondicional e Condições Matemáticas;
- Bloco IV — Sentenças Abertas e Quantificadores;
- Bloco V — Argumentos, Validade e Demonstração Elementar.

Essas apostilas não devem ser tratadas como cinco templates concorrentes. Em conjunto, constituem a base empírica a partir da qual se pode distinguir:

- identidade permanente;
- infraestrutura reutilizável;
- componentes funcionais opcionais;
- soluções específicas;
- microajustes locais;
- precedentes;
- decisões que merecem promoção;
- decisões que devem permanecer locais.

O documento estabelece também um princípio de economia cognitiva e operacional: o conhecimento adquirido na construção de apostilas anteriores deve ser **condensado em sistema**, e não reaprendido indefinidamente por meio da releitura integral de todos os artefatos já produzidos.

Este documento **não substitui** as Regras Gerais HTML/CSS 2.2. Até a aprovação de uma futura Versão 3.0, as Regras 2.2 permanecem a norma canônica vigente.

---

## 2. O Plano de Estudo como sistema editorial

Uma apostila do Plano de Estudo não é uma página isolada nem um produto criado do zero. Ela é a materialização editorial de um conteúdo mestre dentro de uma infraestrutura previamente estabelecida.

A relação fundamental é:

> **CONTEÚDO MESTRE + INFRAESTRUTURA CANÔNICA + COMPONENTES FUNCIONAIS RELEVANTES + ADAPTAÇÕES ESPECÍFICAS JUSTIFICADAS = APOSTILA**

Cada termo possui função distinta.

### 2.1 Conteúdo mestre

O conteúdo mestre determina aquilo que precisa ser ensinado e praticado. Inclui, conforme o documento:

- conceitos;
- sequência pedagógica;
- definições;
- explicações;
- exemplos;
- relações conceituais;
- exercícios;
- quiz;
- gabarito;
- conclusões;
- terminologia;
- escopo.

A camada editorial não recebe autoridade para alterar silenciosamente esse conteúdo.

### 2.2 Infraestrutura canônica

A infraestrutura canônica reúne as decisões suficientemente estáveis para não precisarem ser redescobertas a cada apostila. Ela fornece identidade, previsibilidade documental e uma base técnica comum.

A infraestrutura não é conteúdo e não determina antecipadamente a forma exata de cada página. Ela elimina decisões repetitivas sem impedir adaptação.

### 2.3 Componentes funcionais relevantes

Componentes são soluções semânticas reutilizáveis para funções recorrentes: definição, comparação, resposta, citação, tabela, estrutura inferencial, cenário, tentativa, entre outras.

Um componente só deve aparecer quando sua função existe no conteúdo.

### 2.4 Adaptações específicas justificadas

Uma apostila pode exigir uma solução que ainda não existe no repertório canônico. Nesses casos, a solução deve nascer de uma necessidade editorial, pedagógica ou técnica identificável.

Adaptação não significa liberdade irrestrita de redesign.

### 2.5 O que esta fórmula não significa

A relação anterior não autoriza:

- conversão mecânica de conteúdo em template;
- repetição idêntica da mesma composição em todos os blocos;
- preenchimento obrigatório de uma lista fixa de componentes;
- criação de visuais apenas para produzir variedade;
- alteração livre da identidade;
- transformação do documento em aplicação web;
- submissão do conteúdo à diagramação.

O sistema existe para **preservar decisões maduras e liberar atenção para aquilo que realmente é novo**.

---

## 3. Princípios fundamentais

### 3.1 A forma serve ao conteúdo

O princípio superior permanece:

> **A forma deve servir ao conteúdo. O conteúdo não deve ser deformado para preencher a forma.**

Nenhuma decisão de composição deve:

- expandir artificialmente uma explicação;
- fragmentar a prosa sem necessidade;
- resumir uma relação importante para fazê-la caber;
- duplicar conteúdo porque existe um componente visual;
- introduzir nova conclusão;
- substituir uma distinção conceitual por conveniência gráfica.

### 3.2 Herdar, adaptar, criar somente o novo

O movimento canônico de construção é:

> **HERDAR → ADAPTAR → CRIAR SOMENTE O NOVO**

**Herdar** significa utilizar por padrão aquilo que já é estável, testado e compatível.

**Adaptar** significa ajustar a aplicação da infraestrutura às necessidades do conteúdo sem abandonar a identidade comum.

**Criar somente o novo** significa introduzir um componente, comportamento ou solução apenas quando o repertório existente não resolve adequadamente uma função real.

O anti-padrão é:

> **LER APOSTILAS ANTERIORES → REDESCOBRIR O SISTEMA → RECONSTRUIR A INFRAESTRUTURA → CRIAR VARIAÇÕES DESNECESSÁRIAS**

Esse segundo movimento desperdiça contexto, aumenta inconsistência e transforma precedentes em fonte contínua de reinvenção.

### 3.3 Uma arquitetura madura não elimina adaptação

Princípio central:

> **Uma arquitetura madura não elimina adaptação; ela elimina decisões que não precisam mais ser tomadas.**

Maturidade reduz:

- redesign;
- redescoberta;
- decisões repetitivas;
- contexto necessário para agentes;
- divergências acidentais;
- ciclos de correção.

Maturidade preserva:

- especificidade pedagógica;
- adaptação à disciplina;
- inovação funcional;
- resposta a novos tipos de conteúdo.

### 3.4 Identidade não é uniformização

> **IDENTIDADE COMUM ≠ APARÊNCIA IDÊNTICA**

A identidade do Plano Matemático deve ser reconhecível por um conjunto de constantes editoriais e técnicas, e não pela repetição mecânica das mesmas páginas.

Lógica, Álgebra, Geometria, Estatística e outros conteúdos podem exigir formas diferentes de organização.

Da mesma maneira, uma futura extensão dos princípios para Linguagem, Física, Química, História ou outras disciplinas não autoriza presumir que todas devam parecer “Matemática com outro texto”.

### 3.5 Novidade conceitual não exige novidade decorativa

> **Novidade conceitual não exige novidade decorativa.**

Antes de criar um novo componente, deve-se verificar se a função pode ser resolvida adequadamente por:

1. prosa;
2. tipografia;
3. espaçamento;
4. estrutura HTML;
5. tabela;
6. componente existente;
7. componente novo;
8. recurso gráfico mais complexo.

Essa ordem representa uma preferência pela **solução mais simples suficiente**, não uma proibição absoluta dos recursos posteriores.

### 3.6 Função é mais importante que aparência

A unidade de análise do sistema é a função editorial.

Uma tabela não se torna canônica por possuir determinado cabeçalho azul. O que pode tornar-se canônico é, por exemplo, a função de:

- comparar estados;
- traduzir duas representações;
- investigar casos;
- registrar passos;
- confrontar exercício e gabarito.

### 3.7 Preservar é preferível a reinventar

Quando uma solução aprovada permanece adequada, preservá-la é preferível a substituí-la por uma versão apenas diferente.

Mudança exige motivo:

- conceitual;
- editorial;
- técnico;
- de acessibilidade;
- de compatibilidade;
- de manutenção.

Preferência estética isolada não é justificativa suficiente.

### 3.8 Maturidade reduz superfície de alteração

> **Quanto mais madura estiver uma apostila, menor deve ser a superfície de alteração.**

Uma correção local deve produzir, sempre que possível, um patch local.

Revisão não é autorização para reescrever ou redesenhar partes que já funcionam.

---

## 4. Taxonomia de canonicidade

O sistema adota quatro níveis de canonicidade. Esses níveis classificam **o alcance da solução**, não sua qualidade.

Uma solução local pode ser excelente e definitiva sem jamais precisar tornar-se universal.

| Nível | Definição | Escopo | Herança | Exemplos típicos | Critério de alteração |
|---|---|---|---|---|---|
| **A — Canônico Universal do Plano Matemático** | Elemento estrutural, editorial ou técnico que define o funcionamento ou identidade estável do sistema matemático | Toda nova apostila do Plano Matemático, salvo exceção justificada | Herdado por padrão | A4, identidade tipográfica/cromática, capa institucional, cabeçalho/rodapé, prosa em uma coluna, outline econômico, fidelidade ao conteúdo mestre, paginação controlada | Alteração sistêmica, deliberada e documentada |
| **B — Canônico Opcional** | Solução reutilizável aprovada para uma função recorrente | Onde a função existir | Selecionado por necessidade | definição, exemplo destacado, resposta, tabela funcional, fala de estudante, comparação, estrutura exercício↔gabarito, componentes especializados aprovados | Pode evoluir por função; não deve ser usado por obrigação |
| **C — Específico de disciplina, tópico ou bloco** | Solução correta, porém ligada a necessidade particular | Escopo local ou temático | Não herdado automaticamente | figura geométrica específica, visual de quantificadores, arranjo de alcance, componente exclusivo de determinado conteúdo | Alterado conforme o conteúdo local; pode ser promovido |
| **D — Microajuste Local** | Ajuste de composição sem valor normativo | Ocorrência específica | Nunca herdado por padrão | margem localizada, gap, largura excepcional, keep-with-next, correção de overflow, quebra pontual | Pode mudar ou desaparecer sem alterar a identidade |

### 4.1 Nível A — Canônico Universal do Plano Matemático

O Nível A inclui aquilo que a experiência do Tópico 1.1 e as Regras 2.2 já tornam suficientemente estável no Plano Matemático.

São considerados **consolidados**, em nível conceitual:

- precedência do conteúdo mestre sobre a diagramação;
- separação entre conteúdo e artefato editorial;
- documento concebido desde o início para A4;
- composição normal de prosa em uma coluna;
- identidade visual matemática comum;
- capa institucional sóbria;
- cabeçalho contextual e rodapé documental;
- hierarquia de grandes aberturas, seções e subseções;
- outline econômico baseado em unidades reais de navegação;
- HTML e CSS separados;
- PDF como produto final de estudo;
- paginação orientada por dependências pedagógicas;
- matemática classificada por função editorial;
- uso de visual apenas quando existe função cognitiva;
- preservação de soluções maduras;
- preflight do PDF real como etapa de validação.

Os detalhes de implementação desses itens pertencem ao futuro Documento 03 — Arquitetura Técnica, e não a este documento.

### 4.2 Nível B — Canônico Opcional

Um componente de Nível B pertence ao repertório do sistema, mas não à estrutura obrigatória de todas as apostilas.

O princípio é:

> **Canônico não significa obrigatório. Significa que, quando esta função existir, já existe uma solução aprovada.**

Componentes que já possuem forte evidência para o repertório opcional incluem:

- definição formal;
- enunciado ou afirmação apresentada como objeto;
- resposta curta destacada;
- fala/citação funcional de estudante;
- tabelas de tradução;
- tabelas de comparação;
- tabelas-verdade;
- quadros investigativos;
- estrutura visual compartilhada entre exercício e gabarito.

Alguns componentes especializados surgidos no Bloco V, como estruturas explícitas de argumento, demonstração, tentativa ou direção, são **provisoriamente canônicos**: sua função é clara e sua implementação funcionou, mas sua generalidade deve ser testada em novos tópicos antes de ser tratada como repertório estável de todo o Plano Matemático.

### 4.3 Nível C — Específico de disciplina, tópico ou bloco

Nível C não é um nível inferior de qualidade.

Uma solução permanece local quando sua função depende de um conteúdo específico.

Exemplos:

- painéis de figuras utilizados para proposições sobre objetos geométricos;
- representação específica de alcance em fórmulas;
- quadros de domínio e quantificação;
- comparações desenhadas exclusivamente para determinada relação lógica;
- arranjos vinculados a operação conceitual que não reaparece fora daquele contexto.

Uma solução de Nível C pode ser definitiva dentro do bloco que a originou.

### 4.4 Nível D — Microajuste Local

O Nível D contém correções e acomodações de composição.

Incluem-se, por exemplo:

- pequenos ajustes de margens;
- alterações locais de espaçamento;
- largura específica de tabela;
- associação de título com primeiro parágrafo;
- prevenção de quebra pedagogicamente ruim;
- ajuste pontual de escala;
- correção de clipping;
- acomodação de expressão longa.

Esses ajustes não devem ser copiados para outras apostilas sem que a mesma necessidade exista.

---

## 5. Nível de canonicidade e grau de certeza

O nível A/B/C/D e o grau de certeza são eixos diferentes.

O sistema utiliza três estados de maturidade.

### 5.1 Consolidado

Há evidência suficiente de que a solução cumpre de forma estável a função que lhe foi atribuída.

### 5.2 Provisoriamente canônico

A solução possui forte justificativa funcional e passou por implementação real, mas ainda deve ser observada em novos tópicos ou disciplinas.

### 5.3 Local

Não existe motivo suficiente para promoção. A solução continua válida no escopo em que foi criada.

Exemplos:

- **A4:** Nível A, Consolidado no Plano Matemático.
- **Caixa de definição:** Nível B, Consolidado.
- **Estrutura explícita de argumento:** Nível B em potencial, Provisoriamente canônico.
- **Painel geométrico específico do Bloco I:** Nível C, Local.
- **Margem especial de uma ocorrência:** Nível D, Local.

---

## 6. Promoção, manutenção e rebaixamento

### 6.1 Critérios de promoção

Uma solução de Nível C só deve ser candidata à promoção quando:

1. sua função pode ser descrita sem mencionar o exemplo particular que a originou;
2. resolve um problema recorrente ou evidentemente geral;
3. pode ser reutilizada sem deformar conteúdos diferentes;
4. possui semântica editorial clara;
5. é coerente com a identidade do Plano;
6. foi implementada em documento real;
7. sobreviveu ao ciclo HTML/CSS → PDF → preflight;
8. existe critério claro para utilizá-la;
9. existe critério claro para **não** utilizá-la;
10. sua promoção reduz improvisação sem criar rigidez.

Princípio:

> **Repetição visual não basta para canonização. O que deve ser canonizado é a função.**

### 6.2 Critérios de não promoção

Uma solução não deve tornar-se canônica quando:

- funciona apenas em um conteúdo;
- depende de exemplo particular;
- existe apenas para preencher espaço;
- é predominantemente decorativa;
- duplica uma função já resolvida;
- cria falsa uniformidade;
- nasce de um bug local sem valor geral;
- foi usada apenas por conveniência histórica;
- aumenta complexidade sem reduzir ambiguidade;
- seria artificial em outro tópico ou disciplina.

### 6.3 Manutenção

Componentes canônicos devem evoluir pela menor mudança suficiente.

A manutenção deve preservar:

- semântica;
- função;
- identidade;
- compatibilidade com documentos existentes, quando viável.

### 6.4 Rebaixamento

Canonicidade não é irrevogável.

Uma solução pode ser rebaixada quando:

- um componente mais geral absorve sua função;
- sua generalidade foi superestimada;
- navegadores ou renderizadores mudam;
- a arquitetura técnica evolui;
- uma nova disciplina revela limitações;
- o custo de manutenção supera seu benefício.

O rebaixamento deve ser deliberado e documentado.

---

## 7. Movimento geral de produção

O sistema adota o seguinte movimento:

> **CONTEÚDO MESTRE APROVADO**  
> ↓  
> **MAPEAMENTO SEMÂNTICO**  
> ↓  
> **CLASSIFICAÇÃO EDITORIAL**  
> ↓  
> **HERANÇA DA BASE CANÔNICA**  
> ↓  
> **SELEÇÃO DE COMPONENTES EXISTENTES**  
> ↓  
> **IDENTIFICAÇÃO DE FUNÇÕES REALMENTE NOVAS**  
> ↓  
> **CONSTRUÇÃO HTML/CSS**  
> ↓  
> **PAGINAÇÃO CONCEITUAL**  
> ↓  
> **AUDITORIA ESTÁTICA**  
> ↓  
> **PDF REAL EM WINDOWS + CHROME**  
> ↓  
> **PREFLIGHT**  
> ↓  
> **PATCH MÍNIMO, SE NECESSÁRIO**  
> ↓  
> **CONGELAMENTO**

### 7.1 Conteúdo mestre aprovado

A produção visual começa depois que o conteúdo possui versão de referência suficientemente estável.

### 7.2 Mapeamento semântico

Antes de diagramar, identificam-se:

- macroestrutura;
- Partes;
- seções;
- unidades práticas;
- definições;
- fórmulas;
- relações;
- tabelas;
- visuais previstos;
- dependências pedagógicas.

### 7.3 Classificação editorial

Cada elemento é classificado por função, não pela aparência herdada do arquivo-fonte.

### 7.4 Herança da base canônica

A apostila recebe a infraestrutura já aprovada do sistema.

### 7.5 Seleção de componentes

Utilizam-se somente componentes que respondem a funções existentes.

### 7.6 Funções novas

Só depois se identifica aquilo que exige nova solução.

### 7.7 Construção

HTML concentra conteúdo, semântica e estrutura. CSS concentra aparência, paginação e acabamento.

### 7.8 Paginação conceitual

O documento é distribuído respeitando dependências pedagógicas, não uma meta artificial de preenchimento.

### 7.9 Auditoria estática

Verificam-se estrutura, resíduos, links, classes, matemática, overflow previsível e integridade.

### 7.10 PDF real

A autoridade final de paginação pertence ao ambiente oficial de geração.

### 7.11 Preflight

O PDF é verificado como produto editorial: renderização, legibilidade, paginação, outline e integridade.

### 7.12 Patch mínimo

Defeitos concretos recebem a menor correção suficiente.

### 7.13 Congelamento

Uma apostila aprovada deixa de ser superfície aberta para melhorias arbitrárias.

---

## 8. Movimento pedagógico-editorial interno

A experiência dos cinco blocos revela uma gramática recorrente:

> **TEXTO PREPARA**  
> ↓  
> **SÍMBOLO PRECISA**  
> ↓  
> **VISUAL ORGANIZA, SE NECESSÁRIO**  
> ↓  
> **TEXTO INTERPRETA**  
> ↓  
> **PRÁTICA EXIGE APLICAÇÃO**  
> ↓  
> **GABARITO RECONSTRÓI**

Essa gramática não é uma sequência obrigatória em toda seção.

### 8.1 Texto prepara

A prosa constrói o problema conceitual, fornece contexto e cria necessidade.

### 8.2 Símbolo precisa

A notação entra quando oferece:

- concisão;
- generalização;
- precisão;
- capacidade de transformação.

### 8.3 Visual organiza

O visual entra quando uma relação é percebida melhor espacialmente do que apenas em prosa.

### 8.4 Texto interpreta

O estudante não deve ser abandonado diante de um visual que carregue sozinho uma definição ou conclusão delicada.

### 8.5 Prática exige aplicação

A prática transforma compreensão em operação intelectual observável.

### 8.6 Gabarito reconstrói

O gabarito mostra o suficiente para que o estudante compreenda onde acertou, errou ou perdeu a estrutura do raciocínio.

---

## 9. Conteúdo mestre e camada editorial

O sistema distingue rigorosamente conteúdo e materialização.

### 9.1 O conteúdo mestre possui autoridade sobre

- conceitos;
- sequência;
- exemplos;
- escopo;
- terminologia;
- exercícios;
- respostas;
- argumentos;
- demonstrações;
- relações conceituais.

### 9.2 A camada editorial possui autoridade sobre

- hierarquia visual;
- organização espacial;
- paginação;
- representação;
- componentes;
- ritmo;
- legibilidade;
- integração entre prosa, símbolo e visual.

### 9.3 Limite editorial

HTML/CSS não deve:

- corrigir silenciosamente deficiência conceitual;
- introduzir conteúdo novo;
- remover conteúdo para resolver paginação;
- mudar relação lógica;
- reescrever teoria por conveniência visual;
- antecipar respostas em exercícios.

Se a diagramação revelar um problema conceitual real, o problema retorna ao conteúdo mestre.

---

## 10. Arquitetura da matemática

A matemática deve ser classificada por **função editorial**, não pelo delimitador utilizado no arquivo-fonte.

### 10.1 Matemática inline

É o padrão quando a expressão integra naturalmente a frase.

A notação não deve quebrar a prosa apenas por conter símbolos.

### 10.2 Matemática em linha própria

É apropriada quando uma expressão precisa tornar-se objeto imediato da análise, mas não exige composição espacial especial.

Linha própria não implica centralização.

### 10.3 Matemática estrutural

É apropriada quando o arranjo espacial ajuda a perceber:

- equivalência;
- transformação;
- agrupamento;
- alcance;
- precedência;
- sequência;
- sistema;
- estrutura formal relevante.

### 10.4 Componente especializado

Quando fórmulas formam uma unidade conceitualmente maior, a estrutura deve ser representada como tal.

Por exemplo, `A→B` pode ser apenas uma fórmula.

Uma organização formada por premissas e conclusão constitui, porém, um argumento. Sua função não deve ser reduzida à presença de três linhas matemáticas.

### 10.5 Heurística de destaque

Pergunta de controle:

> **Se os símbolos fossem substituídos por palavras, a ideia ainda mereceria o mesmo destaque?**

Se não, a notação provavelmente deve permanecer subordinada à prosa.

---

## 11. Visualização funcional

Princípio canônico:

> **O melhor visual não é aquele que representa o tema; é aquele que torna visível uma relação que o estudante precisa compreender.**

### 11.1 Funções observadas no Tópico 1.1

**Bloco I — concretização e classificação**  
Figuras, exemplos simples e tabelas ajudam a distinguir tipos de expressão e valor lógico.

**Bloco II — tradução e estrutura**  
Tabelas, agrupamentos e comparações evidenciam relações entre linguagem verbal, conectivos e fórmulas.

**Bloco III — direção e condição**  
A composição torna perceptíveis antecedente, consequente, condição de verdade e diferença entre direções condicionais.

**Bloco IV — domínio e globalidade**  
Tabelas e quadros ajudam a perceber domínio, atribuição, universalidade, existência, testemunho e contraexemplo.

**Bloco V — dependência e justificação**  
Estruturas de argumento e demonstração evidenciam premissas, conclusão, disponibilidade de informação e legitimidade dos passos.

### 11.2 Visual não deve decorar

Não se cria visual apenas porque:

- a página possui muito texto;
- existe espaço livre;
- outro bloco possuía figura;
- o conceito parece visualizável.

### 11.3 Visual não entrega resposta

Em atividades investigativas, o recurso não deve indicar a solução por:

- cor;
- ícone;
- rótulo;
- preenchimento;
- destaque assimétrico;
- nome de classe com resposta embutida;
- relação já desenhada quando ela precisa ser descoberta.

### 11.4 Texto, símbolo e visual formam um sistema

A prosa continua sendo o condutor do raciocínio.

Visual e símbolo ampliam capacidade de percepção e precisão; não substituem a explicação quando ela ainda é necessária.

---

## 12. Paginação e espaço

### 12.1 Paginação conceitual

Princípio:

> **A unidade de paginação deve seguir dependências pedagógicas, não a vontade de preencher geometricamente a página.**

### 12.2 A página não precisa

- terminar sempre cheia;
- eliminar todo espaço branco;
- manter um exercício extenso inteiro;
- comprimir a prosa;
- aumentar ilustrações apenas para ocupar área.

### 12.3 A paginação deve evitar

- título órfão;
- rótulo separado do elemento;
- introdução separada do objeto que apresenta;
- tabela dividida de maneira prejudicial;
- visual isolado de sua interpretação imediata;
- unidade pedagógica pequena fragmentada sem necessidade.

### 12.4 Espaço branco legítimo

Espaço branco pode sinalizar:

- encerramento;
- pausa;
- mudança de movimento;
- separação conceitual;
- impossibilidade natural de acomodar a unidade seguinte.

Espaço branco não é, por si só, falha.

### 12.5 Atomicidade proporcional

Unidades pequenas com dependência imediata podem permanecer juntas.

Unidades extensas devem poder quebrar naturalmente.

---

## 13. Outline e navegação

O outline faz parte do produto editorial.

### 13.1 Função

O outline responde à necessidade de navegação entre grandes unidades, e não à necessidade de reproduzir toda a hierarquia visual do documento.

### 13.2 Economia

Em apostilas de bloco, o padrão consolidado é representar:

- Texto Teórico;
- Partes reais;
- Texto Prático;
- grandes seções práticas.

Exemplos individuais, questões, exercícios e pequenas subseções não recebem bookmark apenas por possuírem título.

### 13.3 Semântica antes da aparência

A hierarquia HTML deve ser planejada a partir da navegação real.

Um texto pode parecer visualmente um título sem precisar participar do outline.

### 13.4 Lição de compatibilidade com Chromium

A experiência do Bloco IV consolidou:

> **Heading que gera bookmark deve, sempre que possível, possuir um único nó textual contínuo.**

Fragmentações internas destinadas apenas a controlar quebra visual podem produzir concatenações inadequadas no bookmark.

A quebra visual deve preferencialmente ser resolvida pelo CSS e pelo navegador.

---

## 14. Texto Teórico e Texto Prático

### 14.1 Texto Teórico

Função principal:

> **construir compreensão.**

A prosa conduz o raciocínio; símbolos e visuais entram conforme função.

### 14.2 Texto Prático

Funções principais:

- testar;
- transferir;
- investigar;
- justificar;
- consolidar;
- diagnosticar.

### 14.3 Estrutura recorrente

A experiência do Tópico 1.1 consolidou como linguagem recorrente:

- Exemplos Resolvidos;
- Quiz, quando necessário;
- Exercícios;
- Gabarito Comentado.

A presença recorrente dessa macroestrutura não autoriza fixar quantidade universal de exemplos, questões ou exercícios.

### 14.4 Estrutura funcional não é quantificação local

O sistema pode padronizar tipos de seção sem padronizar números.

---

## 15. Progressão da prática

A dificuldade prática não deve crescer apenas por:

- quantidade;
- contas maiores;
- fórmulas mais longas;
- enunciados mais extensos.

Ela pode crescer por mudança de operação intelectual:

> **reconhecimento → classificação → tradução → aplicação → comparação → construção → investigação → diagnóstico de erro → justificativa → integração**

O Bloco V mostra uma etapa madura dessa progressão: o estudante não apenas obtém respostas, mas audita raciocínios, localiza falhas, distingue tese de prova e reconstrói demonstrações.

O princípio generalizável é:

> **A prática deve aumentar autonomia, não apenas volume.**

---

## 16. Gabarito como instrumento pedagógico

Princípio:

> **O gabarito deve permitir ao estudante compreender a estrutura da solução na medida exigida pelo objetivo do exercício.**

### 16.1 Proporcionalidade

Questão imediata:

- resposta;
- razão essencial.

Questão estrutural:

- resposta;
- passos relevantes;
- justificativa;
- diagnóstico, quando necessário.

### 16.2 O gabarito não deve

- repetir integralmente a teoria;
- transformar toda resposta em aula longa;
- reduzir raciocínio complexo a resultado seco.

### 16.3 Simetria entre exercício e gabarito

Quando a comparação beneficia a aprendizagem:

> **ESTRUTURA NO EXERCÍCIO ↔ MESMA ESTRUTURA PREENCHIDA NO GABARITO**

Esse padrão foi fortalecido nos Blocos IV e V.

Uma tabela vazia usada para registrar raciocínio pode reaparecer preenchida no gabarito. O estudante compara o mesmo objeto em dois estados, em vez de traduzir entre representações diferentes.

---

## 17. Precedentes

### 17.1 Definição

Um precedente é uma implementação anterior aprovada que demonstra como determinada função foi resolvida.

### 17.2 Precedente não é norma

Um precedente não se torna automaticamente:

- regra;
- template;
- componente universal;
- obrigação;
- justificativa para copiar uma página inteira.

### 17.3 Consulta sob demanda

Princípio:

> **Consultar o menor precedente suficiente.**

Exemplos:

- nova tabela-verdade → consultar precedente de tabela-verdade;
- exercício vazio e gabarito preenchido → consultar precedente dessa relação;
- figura geométrica → consultar precedente gráfico apropriado;
- argumento formal → consultar precedente inferencial.

Não é necessário reler todos os blocos anteriores apenas porque pertencem ao mesmo projeto.

---

## 18. Economia de contexto e agentes

A consolidação arquitetônica possui também função econômica.

### 18.1 Princípio de contexto proporcional

> **A quantidade de contexto fornecida a um agente deve ser proporcional à novidade real da tarefa.**

### 18.2 Conhecimento já consolidado não deve ser reaprendido

> **Material já convertido em regra, arquitetura, template ou componente canônico não deve ser reaprendido pela leitura repetida de apostilas antigas.**

Uma futura tarefa deve receber preferencialmente:

- normas atuais;
- arquitetura atual;
- template vigente;
- conteúdo mestre;
- componentes relevantes;
- precedentes específicos somente quando necessários.

Não deve receber automaticamente:

- todos os PDFs anteriores;
- todos os HTML anteriores;
- todos os CSS anteriores;
- toda a história de desenvolvimento.

### 18.3 O passado deve ser condensado

> **O passado deve ser condensado em sistema, não reaprendido indefinidamente.**

### 18.4 Princípio de custo proporcional

> **Quanto menor o impacto pedagógico, editorial ou técnico de um problema, menor deve ser o custo operacional aceitável para corrigi-lo.**

Hierarquia abstrata:

> **manual → assistência diagnóstica → automação simples → agente de construção → capacidade superior para exceções**

O futuro Guia Codex detalhará os critérios operacionais sem vincular a arquitetura a nomes de modelos ou limites de uso que possam mudar.

---

## 19. Defeitos e custo de correção

### 19.1 Defeito crítico

Exemplos:

- conteúdo ausente;
- matemática incorreta;
- resposta antecipada;
- clipping;
- overflow;
- outline quebrado;
- corrupção estrutural;
- Parte omitida.

A correção é obrigatória.

### 19.2 Defeito real e local

Exemplos:

- espaçamento;
- quebra ruim;
- pequena inconsistência;
- largura;
- propriedade isolada.

Preferência:

> **patch local pelo meio de menor custo suficiente.**

### 19.3 Imperfeição cosmética

Exemplos:

- preferência estética;
- diferença mínima sem impacto;
- alternativa que seria apenas ligeiramente mais bonita.

Em documento maduro, normalmente não justifica reabertura.

---

## 20. Distinções fundamentais

| Categoria | Não se confunde com | Distinção |
|---|---|---|
| **Regra** | Arquitetura | Regra define obrigação, proibição ou critério; arquitetura explica como o sistema se organiza |
| **Arquitetura** | Componente | Arquitetura define relações gerais; componente resolve uma função localizada |
| **Componente** | Precedente | Componente é solução reutilizável formalizada; precedente é uma implementação anterior que pode inspirá-la |
| **Precedente** | Obrigação | Um caso aprovado demonstra possibilidade, não necessidade universal |
| **Solução local** | Regra | Correção ou visual de um caso não ganha alcance sistêmico automaticamente |
| **Bug fix** | Princípio editorial | Um remendo técnico não deve ser elevado a filosofia do sistema sem função geral |
| **Repetição** | Canonicidade | Duas aparições iguais podem ser coincidência; a função precisa ser estável |
| **Uniformidade** | Identidade | Identidade aceita variação funcional |
| **Espaço em branco** | Erro de paginação | Espaço pode ser consequência legítima do fluxo |
| **Matemática em bloco no Markdown** | Matemática estrutural no HTML | Delimitador da fonte não determina tratamento editorial |
| **Destaque visual** | Importância conceitual | Caixa, cor ou centralização não devem criar artificialmente importância |
| **Complexidade do conteúdo** | Complexidade visual | Conteúdo complexo não exige layout mais ornamentado |

---

## 21. Semântica de componentes

Um componente deve ser nomeado por sua função.

Preferir categorias como:

- definição;
- comparação;
- argumento;
- tentativa;
- cenário;
- direção;
- resposta.

Evitar nomes vinculados a:

- página;
- exercício específico;
- cor;
- julgamento de correção;
- exemplo particular.

O catálogo técnico posterior poderá materializar essas funções em classes concretas.

---

## 22. Componente sem resposta embutida

Em exercício investigativo, a forma editorial não deve responder pela atividade.

É inadequado indicar a solução por:

- verde/vermelho;
- check/X;
- fundo privilegiado;
- rótulo “correto/incorreto”;
- ligação antecipada;
- preenchimento;
- ordem gráfica que elimina a investigação.

O componente serve à tarefa; não a resolve.

---

## 23. Resultado renderizado como critério real

A qualidade de uma solução não deve ser avaliada apenas pela elegância abstrata do HTML/CSS.

O produto final de estudo é o PDF.

Por isso, possuem precedência prática:

- legibilidade;
- integridade;
- paginação;
- ausência de clipping;
- qualidade do outline;
- coerência visual;
- relação entre conteúdo e espaço.

O código continua importante para manutenção e previsibilidade, mas não deve vencer o resultado editorial real por purismo abstrato.

O ambiente oficial de geração permanece, conceitualmente:

> **Windows + Chrome**

Renderizadores auxiliares podem ser utilizados para inspeção e comparação, mas não possuem autoridade final sobre paginação.

---

## 24. Relação com outras disciplinas

A experiência do Tópico 1.1 é suficiente para consolidar o sistema do **Plano Matemático**, mas não para declarar automaticamente que toda solução é multidisciplinar.

Devem ser distinguidos três escopos.

### 24.1 Canônico do sistema de apostilas

Princípios potencialmente transversais:

- forma a serviço do conteúdo;
- fidelidade ao conteúdo mestre;
- identidade sem uniformização;
- precedência da função visual;
- paginação conceitual;
- outline econômico;
- mínima superfície de alteração;
- contexto proporcional.

Esses princípios possuem forte potencial multidisciplinar.

### 24.2 Canônico do Plano Matemático

Elementos validados especificamente nas apostilas matemáticas:

- paleta matemática;
- tipografia matemática;
- tratamento de fórmulas;
- linguagem de tabelas;
- notação;
- componentes matemáticos especializados.

### 24.3 Específico da Matemática ou de um tópico

Elementos cuja validade depende diretamente da natureza do conteúdo.

Não devem migrar automaticamente para Linguagem, História ou outras disciplinas.

### 24.4 Princípio de prudência

Onde a experiência ainda não permite decidir:

> **registrar a questão como aberta em vez de inventar universalidade.**

---

## 25. Evidências extraídas dos Blocos I–V

A arquitetura atual não surgiu pronta. O Tópico 1.1 documenta sua maturação.

| Bloco | Desafio editorial principal | Lição consolidada | Nível predominante |
|---|---|---|---|
| **I** | Introduzir lógica sem aparato excessivo | concretização, contraste, economia visual e identidade inicial | A/B |
| **II** | Acomodar maior densidade simbólica, tabelas e equivalências | matemática por função; evitar fragmentação; eliminar herança morta; visual não duplica texto | A/B |
| **III** | Sustentar documento extenso com relações condicionais e prática densa | infraestrutura de página, matemática hierárquica, componentes recorrentes e paginação controlada | A |
| **IV** | Representar domínio, quantificação e contraexemplo sem copiar a linguagem do III | visual como operação intelectual; exercício/gabarito espelhados; preflight maduro; lição do outline/Chromium | A/B |
| **V** | Incorporar argumento e demonstração sem redesenhar o sistema | infraestrutura madura suporta conteúdo novo; componente novo nasce de função nova; primeira construção já altamente madura | A/B |

### 25.1 Bloco I

O Bloco I estabeleceu a identidade editorial inicial e mostrou que conteúdos introdutórios podem ser ensinados com alta clareza sem grande aparato visual.

Seu principal precedente é a relação:

> **concreto → contraste → definição → simbolização → aplicação**

### 25.2 Bloco II

O Bloco II expôs os limites de uma transposição excessivamente literal da marcação matemática da fonte.

Sua revisão consolidou a regra de que o tratamento visual de uma expressão depende de sua função, e não de seu delimitador original.

Também consolidou:

- necessidade de eliminar duplicação entre texto e visual;
- auditoria de tabelas largas;
- remoção de CSS morto herdado;
- aceitação de espaços brancos legítimos.

### 25.3 Bloco III

O Bloco III tornou estável uma infraestrutura capaz de sustentar apostila longa:

- páginas A4;
- running header/footer;
- aberturas;
- matemática;
- tabelas;
- componentes recorrentes;
- paginação por unidades.

Tornou-se principal precedente técnico para os blocos seguintes.

### 25.4 Bloco IV

O Bloco IV mostrou que a identidade específica de um bloco deve nascer de sua função conceitual, e não da reprodução visual do precedente anterior.

O visual passou a operar intelectualmente sobre:

- domínio;
- globalidade;
- testemunho;
- exceção;
- contraexemplo.

Também consolidou a importância do PDF real e revelou uma limitação concreta de headings fragmentados no outline do Chromium.

### 25.5 Bloco V

O Bloco V é a principal evidência de maturidade do sistema.

Mesmo sendo o bloco conceitualmente mais complexo, não exigiu novo layout-base. Apenas as funções realmente novas — argumento, dependência inferencial, demonstração e tentativa — exigiram componentes específicos.

A primeira construção já ter chegado muito próxima do congelamento mostra que a qualidade deixou de depender principalmente de tentativa e erro local.

---

## 26. Não retronormalizar o Tópico 1.1

A consolidação pós-Tópico 1.1 não autoriza reabrir os cinco blocos apenas para torná-los mais iguais.

Pequenas diferenças são legítimas quando:

- refletem o conteúdo;
- pertencem à evolução histórica;
- não quebram identidade;
- não prejudicam uso;
- já foram aprovadas.

O objetivo da consolidação é **melhorar o futuro**, e não apagar a história de amadurecimento dos documentos já congelados.

---

## 27. Fronteira deste documento

Este Documento 01 define **o que o sistema é**. A implementação detalhada pertence aos documentos seguintes.

### 27.1 Documento 02 — Regras Gerais HTML/CSS 3.0

Responderá:

> **O que é obrigatório, proibido ou exigido para conformidade?**

Conterá:

- princípios normativos;
- obrigações;
- proibições;
- precedências;
- critérios de conformidade;
- política de alteração.

### 27.2 Documento 03 — Arquitetura Técnica HTML/CSS

Responderá:

> **Como a infraestrutura canônica é materializada tecnicamente?**

Conterá:

- skeleton;
- estrutura DOM;
- relações entre classes estruturais;
- páginas;
- cabeçalho/rodapé;
- outline;
- paginator;
- impressão.

### 27.3 Documento 04 — Catálogo de Componentes

Responderá:

> **Quais soluções reutilizáveis existem e quando devem ser utilizadas?**

Conterá, para cada componente:

- função;
- status;
- quando usar;
- quando não usar;
- precedentes;
- relação com outros componentes.

### 27.4 Documento 05 — Fluxo de Produção

Responderá:

> **Como uma apostila passa de conteúdo mestre a versão congelada?**

Conterá:

- fases;
- entradas;
- saídas;
- auditorias;
- geração de PDF;
- preflight;
- congelamento.

### 27.5 Documento 06 — Guia Codex

Responderá:

> **Como utilizar o agente com o mínimo de contexto e custo suficiente?**

Conterá:

- seleção de fontes;
- estrutura de prompt;
- precedentes sob demanda;
- limites de autonomia;
- política de patches;
- relação com Git.

### 27.6 Modelo HTML/CSS

Materializará a base técnica já consolidada.

### 27.7 AGENTS.md

Funcionará como memória operacional curta e de alta frequência do repositório.

---

## 28. Hierarquia documental

A relação conceitual entre os documentos futuros é:

> **DOCUMENTO 01 — Arquitetura e Taxonomia Canônica**  
> define o sistema  
> ↓  
> **DOCUMENTO 02 — Regras Gerais**  
> normatiza o sistema  
> ↓  
> **DOCUMENTO 03 — Arquitetura Técnica**  
> materializa estruturalmente o sistema  
> ↓  
> **DOCUMENTO 04 — Catálogo de Componentes**  
> organiza soluções reutilizáveis  
> ↓  
> **DOCUMENTO 05 — Fluxo de Produção**  
> define o processo  
> ↓  
> **DOCUMENTO 06 — Guia Codex**  
> operacionaliza o agente  
> ↓  
> **MODELO HTML/CSS**  
> materializa a base  
> ↓  
> **AGENTS.md**  
> resume instruções operacionais de alta frequência

Essa hierarquia reduz duplicação documental.

---

## 29. Estado de maturidade

Depois do Tópico 1.1, o sistema encontra-se em uma etapa intermediária importante:

- a identidade do Plano Matemático está consolidada;
- a infraestrutura editorial central está consolidada;
- a matemática por função editorial está consolidada;
- a paginação conceitual está consolidada;
- o outline econômico está consolidado;
- o preflight do PDF real está consolidado;
- existe repertório de componentes reutilizáveis;
- ainda falta separar tecnicamente base e componentes;
- ainda falta testar alguns componentes em novos tópicos;
- ainda falta distinguir, com experiência adicional, o que é matemático daquilo que será multidisciplinar.

O objetivo da consolidação não é declarar o sistema imutável.

É reduzir o número de decisões fundamentais que permanecem abertas.

---

## 30. Questões abertas

As seguintes questões não devem ser resolvidas apenas com base no Tópico 1.1:

1. Quais elementos da identidade visual serão compartilhados integralmente com o Plano Linguístico?
2. A mesma gramática de capa deverá permanecer em todas as disciplinas ou haverá uma identidade institucional comum com variações disciplinares?
3. Quais componentes matemáticos serão úteis em Física e Química?
4. Que biblioteca gráfica será necessária para Geometria?
5. Quais estruturas próprias surgirão para textos literários, análise sintática e corpora linguísticos?
6. Qual parte do catálogo poderá ser promovida a uma biblioteca multidisciplinar?
7. O modelo técnico único será suficiente para disciplinas com estruturas documentais muito diferentes?
8. Como documentos com imagens, mapas, gráficos ou fontes históricas alterarão a relação entre texto e visual?
9. Quais componentes surgidos no Bloco V permanecerão específicos de argumentação formal e quais serão reutilizados em demonstrações matemáticas futuras?
10. Até que ponto a macroestrutura Exemplos Resolvidos → Quiz → Exercícios → Gabarito permanecerá adequada em todos os tópicos matemáticos?
11. Quais ajustes de acessibilidade devem integrar explicitamente a próxima arquitetura técnica?
12. Quais decisões atuais são condicionadas ao comportamento do Chrome e precisarão ser revistas caso o ambiente oficial mude?

A incerteza deve permanecer documentada até que nova evidência permita decisão.

---

## 31. Síntese canônica

Os princípios que orientam a continuação da consolidação são:

1. **Uma apostila herda antes de criar.**
2. **A forma serve ao conteúdo.**
3. **Função é mais importante que aparência.**
4. **Canônico não significa obrigatório.**
5. **Solução local não vira regra por repetição acidental.**
6. **Novidade conceitual não exige novidade decorativa.**
7. **Visual precisa tornar uma relação intelectualmente perceptível.**
8. **A prosa continua sendo o condutor do raciocínio.**
9. **Matemática é classificada pela função editorial, não pela marcação original.**
10. **Quebra de linha, centralização e destaque são decisões independentes.**
11. **Paginação segue dependência pedagógica.**
12. **Espaço branco pode ser legítimo.**
13. **Outline representa navegação real, não toda a hierarquia visível.**
14. **Headings de bookmark devem ser semanticamente simples e compatíveis com o ambiente real de geração.**
15. **Exercício e gabarito podem compartilhar a mesma estrutura visual quando isso melhora a conferência.**
16. **A dificuldade prática deve crescer em autonomia e operação intelectual, não apenas em volume.**
17. **Precedentes são consultados sob demanda.**
18. **Maturidade reduz a superfície de alteração.**
19. **O custo da correção deve ser proporcional ao impacto do defeito.**
20. **O contexto de um agente deve ser proporcional à novidade da tarefa.**
21. **Material já convertido em sistema não deve ser reaprendido por releitura integral de documentos antigos.**
22. **Uma arquitetura madura não elimina adaptação; ela elimina decisões que não precisam mais ser tomadas.**
23. **O passado deve ser condensado em sistema, não reaprendido indefinidamente.**

---

## 32. Base empírica da consolidação

Este documento foi construído a partir das seguintes fontes de referência do projeto.

### Norma vigente

**Regras Gerais para Criação de HTML/CSS — Plano de Estudo Matemático — Versão Definitiva 2.2 — 2026**

### Apostilas definitivas do Tópico 1.1 — Lógica Matemática

**Bloco I — Proposição, Valor Lógico e Negação**

**Bloco II — Proposições Compostas, Conectivos e Tabelas-Verdade**

**Bloco III — Condicional, Bicondicional e Condições Matemáticas**

**Bloco IV — Sentenças Abertas e Quantificadores**

**Bloco V — Argumentos, Validade e Demonstração Elementar**

### Artefatos técnicos consultados

- HTML/CSS definitivos disponíveis;
- especialmente os precedentes técnicos dos Blocos III, IV e V;
- conteúdo mestre e registro de revisão final do Bloco II;
- instruções de construção e preflight consolidadas nos Blocos IV e V.

---

## 33. Encerramento

O Plano de Estudo Matemático passa, com esta consolidação, a possuir uma teoria explícita de sua própria arquitetura editorial.

Essa teoria não pretende impedir evolução. Seu objetivo é impedir que evolução seja confundida com reinvenção permanente.

A partir deste ponto, uma nova apostila não deve começar pela pergunta:

> **“Como devemos desenhar este documento?”**

Deve começar pela pergunta:

> **“O que este conteúdo exige além daquilo que o sistema já sabe fazer?”**

Essa mudança de perspectiva permite preservar identidade, reduzir contexto, limitar retrabalho e concentrar atenção exatamente onde uma nova decisão é necessária.

> **Uma arquitetura madura não elimina adaptação; ela elimina decisões que não precisam mais ser tomadas.**

> **O passado deve ser condensado em sistema, não reaprendido indefinidamente.**
