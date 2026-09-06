# Regras Gerais para Criação de HTML/CSS
## Plano de Estudo Matemático — Versão 3.0

**Documento 02 da Consolidação Pós-Tópico 1.1**  
**Escopo:** norma geral para produção, revisão e validação das apostilas HTML/CSS do Plano de Estudo Matemático.

Esta versão consolida o patrimônio normativo das Regras Gerais 2.2 à luz da **Arquitetura e Taxonomia Canônica do Sistema de Apostilas — Versão 1.0**. Seu objetivo é dizer **o que deve ser respeitado** para que uma produção seja considerada conforme, sem transformar as Regras Gerais em manual de implementação, catálogo de componentes ou guia de agente.

Quando adotada como norma vigente do projeto, a Versão 3.0 substitui a Versão 2.2 para novas produções e revisões. Apostilas anteriormente congeladas não precisam ser retronormalizadas apenas por causa da nova redação normativa.

---

# REGRA SUPERIOR

> **A forma deve servir ao conteúdo.**

O conteúdo não deve ser expandido, reduzido, reescrito, fragmentado, duplicado ou deformado para servir à composição. A flexibilidade editorial permite adaptação funcional, não improvisação arbitrária.

---

# I — STATUS, ESCOPO E PRECEDÊNCIA

## 1. ESTAS REGRAS DEFINEM A CONFORMIDADE NORMATIVA DO PLANO MATEMÁTICO

As Regras Gerais 3.0 estabelecem obrigações, proibições, critérios e limites para a construção e revisão das apostilas HTML/CSS do Plano de Estudo Matemático.

Detalhes de implementação pertencem aos documentos técnicos próprios do sistema.

## 2. A ORDEM DE PRECEDÊNCIA DEVE SER RESPEITADA

Diante de uma decisão editorial, estrutural ou técnica, consultar nesta ordem:

1. conteúdo mestre aprovado;
2. Regras Gerais vigentes;
3. Arquitetura Técnica vigente;
4. componente canônico aplicável no Catálogo de Componentes;
5. precedente comparável, quando necessário;
6. instruções específicas da tarefa.

Uma instrução de nível inferior não pode violar silenciosamente uma decisão de nível superior.

## 3. AMBIGUIDADES ESTRUTURAIS RELEVANTES NÃO DEVEM SER RESOLVIDAS POR IMPROVISAÇÃO

Quando conteúdo mestre, regras, arquitetura e precedentes não forem suficientes para decidir uma mudança de alcance relevante, deve-se interromper a decisão e solicitar orientação.

Microajustes de composição que não alterem significado, identidade ou convenção sistêmica podem ser resolvidos localmente.

---

# II — CANONICIDADE, HERANÇA E CONTROLE DE MUDANÇA

## 4. O SISTEMA DISTINGUE QUATRO NÍVEIS DE CANONICIDADE

A classificação normativa é:

| Nível | Natureza | Regra de herança |
|---|---|---|
| **A — Canônico Universal do Plano Matemático** | identidade ou funcionamento geral do sistema | herdado por padrão; alteração exige decisão sistêmica |
| **B — Canônico Opcional** | solução aprovada para uma função recorrente | utilizado somente quando a função existir |
| **C — Específico** | solução válida de disciplina, tópico ou bloco | não é herdado automaticamente |
| **D — Microajuste Local** | correção pontual de composição | não possui valor normativo nem deve ser copiado por padrão |

Canônico opcional não significa obrigatório.

## 5. UMA APOSTILA DEVE HERDAR ANTES DE CRIAR

O movimento padrão é:

> **HERDAR → ADAPTAR → CRIAR SOMENTE O NOVO**

Primeiro preservam-se as soluções canônicas adequadas; depois adaptam-se ao conteúdo; somente então se cria uma solução nova para função ainda não atendida.

## 6. PRESERVAR É PREFERÍVEL A REINVENTAR

Quando uma solução aprovada continuar funcionalmente adequada, ela deve ser mantida.

Não se redesenha infraestrutura, identidade, componente ou convenção recorrente apenas para produzir variedade visual.

## 7. SOLUÇÕES LOCAIS NÃO PODEM SER PROMOVIDAS SILENCIOSAMENTE

Repetição visual, conveniência histórica ou sucesso em um caso isolado não bastam para tornar uma solução canônica.

Uma solução só pode ser promovida quando sua função:

- puder ser descrita independentemente do exemplo que a originou;
- for recorrente ou claramente geral;
- possuir semântica clara;
- puder ser reutilizada sem deformar conteúdos diferentes;
- tiver sido testada em implementação real e no PDF;
- possuir critérios claros de uso e de não uso;
- reduzir improvisação sem criar rigidez desnecessária.

## 8. CANONICIDADE PODE SER REVISTA DELIBERADAMENTE

Uma solução canônica pode ser rebaixada, substituída ou absorvida por outra quando sua função se mostrar mais local do que se supunha, quando a arquitetura evoluir ou quando o custo de manutenção superar o benefício.

A revisão deve ser consciente e documentada, nunca casual.

## 9. DOCUMENTOS MADUROS DEVEM TER SUPERFÍCIE MÍNIMA DE ALTERAÇÃO

Quanto mais madura estiver uma apostila, menor deve ser a área atingida por uma correção.

Revisão não é oportunidade para reescrever ou redesenhar partes que já funcionam. Problemas locais devem produzir, sempre que possível, patches locais.

## 10. A NOVA NORMA NÃO OBRIGA RETRONORMALIZAÇÃO DE DOCUMENTOS CONGELADOS

Apostilas já aprovadas permanecem válidas quando continuam funcionalmente corretas, não apresentam defeito crítico e preservam a identidade do sistema.

Diferenças decorrentes da evolução histórica não justificam, por si só, reabertura.

---

# III — CONTEÚDO MESTRE E RESPONSABILIDADE EDITORIAL

## 11. O CONTEÚDO MESTRE É INDEPENDENTE DA DIAGRAMAÇÃO

O conteúdo mestre define conceitos, sequência, explicações, exemplos, exercícios, respostas, relações, argumentos e demonstrações.

A camada HTML/CSS organiza e representa esse conteúdo; não recebe autoridade para modificá-lo silenciosamente.

## 12. PROBLEMAS CONCEITUAIS ENCONTRADOS NA DIAGRAMAÇÃO DEVEM RETORNAR AO CONTEÚDO

Se a composição revelar definição incompleta, erro matemático, ambiguidade, contradição ou insuficiência pedagógica, a correção deve ocorrer no conteúdo mestre ou ser explicitamente autorizada.

Não se corrige silenciosamente o conhecimento apenas no HTML final.

## 13. HTML É ARTEFATO DE PRODUÇÃO; PDF É PRODUTO FINAL DE ESTUDO

O HTML deve priorizar semântica, estrutura, composição e previsibilidade de impressão.

Não deve ser tratado como site ou aplicação interativa quando essas funções não pertencem ao documento.

## 14. HTML E CSS DEVEM PERMANECER SEPARADOS

Como princípio de manutenção:

- HTML concentra conteúdo, semântica e estrutura;
- CSS concentra identidade visual, tipografia, espaçamento, paginação e acabamento.

Exceções técnicas só se justificam quando documentadas e necessárias.

## 15. FIDELIDADE SEMÂNTICA É OBRIGATÓRIA

A representação editorial não pode:

- remover condição necessária;
- acrescentar relação inexistente;
- sugerir propriedade não dada;
- alterar o sentido de uma fórmula;
- antecipar conclusão não contida no conteúdo mestre.

Quando uma simplificação visual puder ser confundida com simplificação conceitual, a fidelidade conceitual prevalece.

---

# IV — IDENTIDADE E ARQUITETURA DOCUMENTAL

## 16. A IDENTIDADE VISUAL MATEMÁTICA É CANÔNICA

A identidade do Plano Matemático utiliza como referência:

- Índigo — `#252B5E`;
- Cobalto — `#3657A7`;
- Violeta — `#6558A6`;
- Azul técnico — `#7396C8`;
- Neblina — `#EEF2F8`;
- Cinza-azulado — `#C5CEDD`;
- Grafite — `#252A33`;
- Cinza editorial — `#6F7583`;
- Branco editorial — `#FBFCFE`.

Como famílias de referência:

- Arial ou equivalente confiável para títulos e elementos editoriais;
- Georgia para corpo discursivo;
- Cambria Math, STIX ou equivalente confiável para notação matemática quando necessário.

Mudança deliberada da identidade pertence ao sistema, não a uma apostila isolada.

## 17. IDENTIDADE COMUM NÃO SIGNIFICA LAYOUT IDÊNTICO

A unidade do sistema nasce de tipografia, paleta, hierarquia, ritmo, cabeçalho, rodapé, acabamento e disciplina editorial.

Lógica, Álgebra, Geometria, Estatística e outros conteúdos podem exigir composições diferentes sem deixar de pertencer ao mesmo Plano.

## 18. CAPA, FORMATO A4 E FLUXO PRINCIPAL DEVEM PRESERVAR A GRAMÁTICA CANÔNICA

A apostila deve ser concebida desde o início para A4 e manter a capa institucional sóbria já consolidada.

O fluxo normal da prosa é de uma única coluna. Colunas múltiplas só são justificadas quando simultaneidade, comparação ou contraste possuem função real.

## 19. CABEÇALHO E RODAPÉ POSSUEM FUNÇÕES DOCUMENTAIS DISTINTAS

Toda página interna deve manter orientação contextual e identidade documental consistentes:

- cabeçalho localiza o leitor dentro da apostila;
- rodapé identifica a apostila e sua paginação.

Devem ser discretos e não competir com os títulos.

## 20. A HIERARQUIA EDITORIAL DEVE SER INEQUÍVOCA

Grandes Partes, seções e subseções precisam possuir diferenças claras de escala, espaçamento e função.

Uma subseção não deve parecer abertura de Parte; um parágrafo normal não deve ser promovido artificialmente a composição especial.

---

# V — COMPOSIÇÃO, MATEMÁTICA E REPRESENTAÇÃO VISUAL

## 21. A PROSA PERMANECE O CONDUTOR DO RACIOCÍNIO

Símbolos, tabelas e visuais devem cooperar com a explicação, não substituí-la automaticamente.

O movimento preferencial é:

> texto prepara → representação precisa → visual organiza, se necessário → texto interpreta e continua.

## 22. A MATEMÁTICA DEVE SER CLASSIFICADA POR FUNÇÃO EDITORIAL

A hierarquia normativa é:

- **inline**: padrão quando a expressão pertence naturalmente à frase;
- **linha própria**: quando a expressão é objeto imediato de análise;
- **estrutural**: quando a disposição espacial revela relações relevantes;
- **componente especializado**: quando fórmulas formam uma unidade conceitual maior, como argumento, sistema, cadeia ou demonstração.

O delimitador utilizado no Markdown ou em outra fonte não determina sozinho o tratamento visual final.

## 23. QUEBRA DE LINHA, CENTRALIZAÇÃO E DESTAQUE SÃO DECISÕES INDEPENDENTES

Uma expressão pode ocupar linha própria sem ser centralizada.

Centralização é excepcional e deve possuir função espacial clara. A mera presença de símbolos, tamanho da fórmula ou sensação de importância não constitui justificativa suficiente para destaque.

## 24. TRANSFORMAÇÕES E TRADUÇÕES MATEMÁTICAS DEVEM SER ACOMPANHÁVEIS

Quando a aprendizagem depende da passagem entre representações, equivalências, etapas ou transformações, a composição deve tornar o percurso legível.

Não se devem saltar relações essenciais apenas para obter página mais compacta.

## 25. VISUAL SÓ DEVE EXISTIR QUANDO POSSUI FUNÇÃO COGNITIVA

Antes de inserir um recurso visual, deve ser possível responder o que ele torna perceptível que prosa, símbolo ou composição simples não tornam suficientemente claro.

Visualidade não é quantidade de visuais.

## 26. O VISUAL NÃO PODE ENTREGAR O RACIOCÍNIO QUE O ESTUDANTE DEVE PRODUZIR

Em atividades investigativas, a forma não deve revelar a resposta por cor, ícone, preenchimento, rótulo, ordem privilegiada ou conexão já resolvida.

O componente serve à tarefa; não a responde.

## 27. A REPRESENTAÇÃO DEVE PRESERVAR A ESTRUTURA MATEMÁTICA

Diagramas, figuras, tabelas e esquemas não podem acrescentar condições, eliminar exceções, depender exclusivamente de cor ou sugerir propriedades geométricas não fornecidas.

Quando uma figura for esquemática e sua aparência puder induzir interpretação indevida, a limitação relevante deve ser explicitada.

## 28. A SOLUÇÃO MAIS SIMPLES SUFICIENTE DEVE SER PREFERIDA

A prioridade geral de composição é:

> prosa → tipografia → espaçamento → estrutura → tabela/componente existente → componente novo → recurso gráfico mais complexo.

Novidade conceitual não exige novidade decorativa.

---

# VI — COMPONENTES, TABELAS E DESTAQUES

## 29. COMPONENTES DEVEM SER USADOS POR FUNÇÃO, NÃO POR OBRIGAÇÃO

Componentes canônicos opcionais só devem aparecer quando sua função semântica existir no conteúdo.

Se uma solução canônica adequada já existe, não se deve criar uma nova variante apenas para diferenciar a apostila.

## 30. CAIXAS E DESTAQUES DEVEM POSSUIR SEMÂNTICA EXPLÍCITA

Definição formal, princípio, síntese, observação e resposta não são automaticamente a mesma categoria visual.

Uma caixa aprovada para definição não deve virar destaque genérico. Quando tudo é destacado, a hierarquia deixa de existir.

## 31. TABELAS E COLUNAS SERVEM À ESTRUTURA REALMENTE COMPARATIVA OU TABULAR

Tabelas são adequadas quando linhas e colunas representam categorias, casos, valores, traduções ou relações simultâneas.

Colunas e cartões não devem ser usados apenas para preencher espaço ou fragmentar prosa normal.

## 32. DIAGRAMAS E RECURSOS GRÁFICOS DEVEM REPRESENTAR RELAÇÕES REAIS

Conectores representam relações; não substituem conceitos.

Ramificações devem possuir origem clara. Geometria que exige precisão deve ser representada por recurso tecnicamente adequado, sem ornamentação desnecessária.

## 33. MATERIAIS EXTERNOS DEVEM TER FIDELIDADE E CRÉDITO ADEQUADOS

Questões reproduzidas, figuras, textos ou materiais externos diretamente presentes na apostila devem preservar o conteúdo original dentro do necessário e receber identificação compatível com seu uso.

Bibliografia de construção e fonte direta de material reproduzido são categorias distintas.

---

# VII — PAGINAÇÃO, ESPAÇO E NAVEGAÇÃO

## 34. PAGINAÇÃO DEVE SEGUIR DEPENDÊNCIAS PEDAGÓGICAS

A página deve preservar relações de leitura, não perseguir preenchimento geométrico uniforme.

Espaço branco pode ser legítimo quando resulta do encerramento natural de uma unidade, de uma pausa conceitual ou da necessidade de manter a próxima unidade coesa.

## 35. ATOMICIDADE DEVE SER PROPORCIONAL À UNIDADE

Devem permanecer juntas, quando possível, unidades pequenas e fortemente dependentes, como título + abertura imediata ou rótulo + objeto correspondente.

Unidades extensas — especialmente exercícios, exemplos e respostas longas — devem poder quebrar naturalmente quando isso não prejudicar compreensão.

## 36. TÍTULOS ÓRFÃOS, CLIPPING E OVERFLOW DEVEM SER EVITADOS

A paginação deve controlar títulos órfãos, elementos cortados, ultrapassagem da largura útil e fragmentações claramente inadequadas.

Viúvas e órfãs de texto devem ser reduzidas quando razoável, sem provocar espaços excessivos ou rigidez artificial.

## 37. O OUTLINE DEVE SER ECONÔMICO E BASEADO EM NAVEGAÇÃO REAL

Bookmarks representam unidades que o leitor procurará diretamente, e não toda a hierarquia visual existente na página.

Em apostilas de bloco, a árvore deve privilegiar Texto Teórico, Partes reais e grandes unidades do Texto Prático.

## 38. HEADINGS QUE GERAM BOOKMARKS DEVEM SER SEMANTICAMENTE SIMPLES

Sempre que possível, um heading destinado ao outline deve conter texto contínuo e evitar fragmentações internas criadas apenas para controlar quebra visual.

A quebra visual deve ser responsabilidade preferencial do CSS e do navegador.

---

# VIII — TEXTO TEÓRICO, TEXTO PRÁTICO E GABARITO

## 39. TEXTO TEÓRICO E TEXTO PRÁTICO POSSUEM FUNÇÕES DISTINTAS E COMPLEMENTARES

O Texto Teórico constrói compreensão.

O Texto Prático testa, transfere, investiga e consolida essa compreensão.

A estrutura recorrente — Exemplos Resolvidos, Quiz quando aplicável, Exercícios e Gabarito Comentado — é funcional, não uma imposição de quantidades fixas.

## 40. A PRÁTICA DEVE PROGREDIR POR OPERAÇÃO INTELECTUAL, NÃO APENAS POR VOLUME

A dificuldade pode crescer por reconhecimento, classificação, tradução, aplicação, comparação, construção, investigação, diagnóstico de erro, justificativa e integração.

Aumentar apenas o tamanho da conta ou o número de itens não constitui, por si só, progressão pedagógica.

## 41. O GABARITO DEVE SER PROPORCIONAL AO RACIOCÍNIO EXIGIDO

Questões imediatas podem receber resposta e justificativa curta. Questões estruturais devem apresentar os passos necessários para que o estudante diagnostique o próprio raciocínio.

O gabarito não deve repetir desnecessariamente a teoria nem reduzir raciocínio complexo a resultado seco.

## 42. EXERCÍCIO E GABARITO PODEM COMPARTILHAR A MESMA ESTRUTURA VISUAL

Quando a comparação for pedagogicamente útil, a estrutura usada pelo estudante para investigar pode reaparecer preenchida no gabarito.

Essa simetria não é obrigatória; deve ser usada quando reduz carga de tradução visual e melhora a conferência.

---

# IX — PRODUÇÃO, VALIDAÇÃO E CONGELAMENTO

## 43. O DOCUMENTO DEVE SER CONCEBIDO DESDE O INÍCIO PARA O PDF FINAL

A geração oficial e a validação de paginação são realizadas em **Windows + Chrome**.

Outros renderizadores podem ser usados como apoio, mas não possuem autoridade final sobre a paginação oficial.

## 44. O HTML NÃO É CONSIDERADO CONCLUÍDO ANTES DO PREFLIGHT DO PDF

Antes do congelamento, o produto real deve ser auditado quanto a:

- integridade do conteúdo;
- renderização;
- legibilidade;
- paginação;
- matemática;
- clipping e overflow;
- cabeçalho e rodapé;
- outline;
- fidelidade à identidade canônica.

## 45. A CORREÇÃO DEVE SER PROPORCIONAL À GRAVIDADE DO DEFEITO

Aplicar a seguinte distinção:

- **defeito crítico** — deve ser corrigido;
- **defeito real e local** — deve receber o menor patch suficiente;
- **imperfeição cosmética sem impacto** — normalmente não justifica reabertura.

Quanto menor o impacto pedagógico, editorial ou técnico do problema, menor deve ser o custo operacional aceitável para corrigi-lo.

## 46. UMA VERSÃO APROVADA DEVE SER CONGELADA

Depois de conteúdo, estrutura, paginação, outline e acabamento passarem pelo preflight, a apostila deixa de ser superfície aberta para melhorias arbitrárias.

Nova alteração requer defeito concreto ou mudança deliberada de sistema.

---

# X — PRECEDENTES, MANUTENÇÃO E ECONOMIA DE CONTEXTO

## 47. PRECEDENTES DEVEM SER CONSULTADOS SOB DEMANDA

Um precedente demonstra como determinada função já foi resolvida; não é automaticamente norma, template ou obrigação.

Deve-se consultar o menor precedente suficiente para a dúvida em questão.

## 48. CONHECIMENTO JÁ CONVERTIDO EM SISTEMA NÃO DEVE SER REAPRENDIDO INDEFINIDAMENTE

Material já formalizado em regra, arquitetura, template ou componente canônico não precisa ser reconstruído pela releitura integral de apostilas anteriores.

O passado deve ser condensado em sistema.

## 49. O CONTEXTO FORNECIDO A AGENTES DEVE SER PROPORCIONAL À NOVIDADE DA TAREFA

Uma tarefa normal deve receber o conjunto mínimo de normas, arquitetura, conteúdo mestre, componentes e precedentes necessários para sua execução.

O detalhamento operacional dessa economia pertence ao Guia Codex e não a estas Regras Gerais.

---

# XI — CONFORMIDADE E FRONTEIRAS DOCUMENTAIS

## 50. UMA APOSTILA É CONSIDERADA CONFORME QUANDO PRESERVA O SISTEMA E O CONTEÚDO

A conformidade exige, no mínimo:

- conteúdo mestre preservado;
- Regras Gerais respeitadas;
- identidade matemática mantida;
- componentes usados semanticamente;
- paginação íntegra;
- outline coerente;
- ausência de defeitos críticos no PDF final.

Conformidade não significa que todas as apostilas tenham aparência idêntica.

## 51. AS REGRAS GERAIS NÃO SUBSTITUEM OS DOCUMENTOS ESPECIALIZADOS

As fronteiras do sistema são:

- **Documento 01 — Arquitetura e Taxonomia Canônica:** define o que pertence ao sistema e em que nível;
- **Documento 02 — Regras Gerais:** define o que é obrigatório, proibido ou necessário para conformidade;
- **Documento 03 — Arquitetura Técnica:** define a materialização estrutural e técnica;
- **Documento 04 — Catálogo de Componentes:** define componentes, função, uso e não uso;
- **Documento 05 — Fluxo de Produção:** define fases, auditorias, geração e congelamento;
- **Documento 06 — Guia Codex:** define contexto, autonomia e operação do agente;
- **Modelo HTML/CSS:** materializa a infraestrutura-base;
- **AGENTS.md:** resume instruções operacionais de alta frequência.

Uma informação deve permanecer no documento correspondente ao seu nível.

---

# NOTA FINAL DE ESCOPO

Estas Regras Gerais são, neste momento, regras do **Plano de Estudo Matemático**. Alguns princípios possuem potencial para outros Planos de Estudo, mas essa generalização deve ser validada por experiência própria de cada disciplina.

A Versão 3.0 deve ser lida em conjunto com a Arquitetura e Taxonomia Canônica vigente. Sua função é normativa: **dizer tudo o que precisa ser norma sem tentar dizer tudo o que o sistema sabe**.

> **Uma arquitetura madura não elimina adaptação; ela elimina decisões que não precisam mais ser tomadas.**

> **Uma apostila herda antes de criar.**

> **Canônico não significa obrigatório.**

> **O passado deve ser condensado em sistema, não reaprendido indefinidamente.**
