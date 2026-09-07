# Fluxo de Produção HTML/CSS
## Plano de Estudo Matemático — Versão 1.0

**Documento 05 da Consolidação Pós-Tópico 1.1**  
**Escopo:** fluxo canônico para transformar conteúdo mestre aprovado em apostila HTML/CSS validada, PDF oficial e versão congelada.

Este documento define a **ordem operacional** da produção e da manutenção das apostilas do Plano de Estudo Matemático.

Ele não substitui os documentos anteriores:

- **Documento 01 — Arquitetura e Taxonomia Canônica:** define o que pertence ao sistema e em que nível;
- **Documento 02 — Regras Gerais HTML/CSS:** define o que deve ser respeitado para conformidade;
- **Documento 03 — Arquitetura Técnica HTML/CSS:** define como a infraestrutura técnica funciona;
- **Documento 04 — Catálogo de Componentes HTML/CSS:** define soluções opcionais aprovadas, suas funções, usos e limites;
- **Documento 05 — Fluxo de Produção:** define em que ordem entendimento, classificação, herança, construção, validação, correção e congelamento acontecem;
- **Documento 06 — Guia Codex:** definirá como o agente executa esse processo com contexto, autonomia e custo adequados.

> **O Fluxo de Produção não determina a aparência da apostila; determina a ordem em que entendimento, decisões, construção e validação acontecem.**

---

# 1. FINALIDADE E ESCOPO

O Fluxo de Produção responde à pergunta:

> **Como uma apostila do Plano Matemático passa de conteúdo mestre aprovado a versão final congelada?**

Seu objetivo é tornar explícito um percurso comum sem transformar a produção em sequência burocrática.

O fluxo completo rege principalmente:

- novas apostilas;
- reconstruções de grande alcance;
- reaberturas justificadas que alterem significativamente a estrutura.

Tarefas locais de manutenção utilizam fluxos abreviados.

O documento não ensina:

- implementação detalhada da infraestrutura;
- código do paginator;
- CSS de componentes;
- comandos Git;
- geração por linha de comando;
- uso de VS Code;
- prompts ou políticas de agente;
- escolha de modelos;
- procedimentos operacionais específicos do Codex.

A função deste documento é coordenar os documentos anteriores em uma sequência verificável.

---

# 2. PRINCÍPIOS OPERACIONAIS

O fluxo adota os seguintes princípios.

## 2.1 Entender antes de construir

Código não deve ser a primeira forma de leitura do conteúdo.

A produção começa pela compreensão da estrutura pedagógica e matemática do material.

## 2.2 Classificar antes de representar

Antes de escolher classes, tabelas, destaques ou componentes, deve-se identificar a função editorial do conteúdo.

A pergunta não é primeiro:

> “Como isto deve parecer?”

A pergunta é:

> “Que função isto desempenha e que relação precisa permanecer perceptível?”

## 2.3 Uma apostila herda antes de criar

O movimento normal é:

**HERDAR → ADAPTAR → CRIAR SOMENTE O NOVO**

Infraestrutura estável deve ser herdada. Componentes aprovados devem ser reutilizados quando sua função existir. Extensão nova só aparece quando o sistema ainda não resolve adequadamente uma necessidade real.

## 2.4 Base estável; extensão local

Necessidade específica não deve contaminar a infraestrutura global.

Uma função nova nasce localmente, é testada no produto real e somente depois pode ser avaliada para eventual promoção.

## 2.5 Paginar por dependência, não por preenchimento

A página preserva relações pedagógicas.

Espaço branco legítimo não constitui defeito apenas porque poderia receber mais conteúdo.

## 2.6 Validar o produto real

Preview, inspeção de HTML e auditoria estática são etapas necessárias, mas não encerram a produção.

A autoridade final sobre paginação e integridade do produto pertence ao **PDF oficial gerado em Windows + Chrome**.

## 2.7 Corrigir somente o necessário

A correção deve atuar sobre a causa com a menor superfície de alteração compatível com o defeito.

Quanto mais madura a apostila, menor deve ser a superfície de alteração.

## 2.8 O custo da correção deve ser proporcional ao impacto

Defeito crítico justifica investigação e correção completas.

Defeito local justifica a menor intervenção suficiente.

Imperfeição cosmética sem impacto normalmente não justifica novo ciclo.

## 2.9 O fluxo seleciona contexto; não acumula contexto

Uma produção não deve exigir releitura indiscriminada de apostilas anteriores, do Catálogo inteiro ou de todos os precedentes.

O contexto normal é formado pelos documentos canônicos vigentes, pelo conteúdo mestre e pelas soluções diretamente relevantes.

Precedentes são consultados sob demanda.

## 2.10 O fluxo precisa terminar

O objetivo não é atingir perfeição abstrata, mas obter um produto correto, íntegro, legível, conforme e pedagogicamente funcional.

> **A ausência de perfeição absoluta não impede o congelamento; a presença de defeito real, sim.**

---

# 3. VISÃO GERAL DO FLUXO

```text
CONTEÚDO MESTRE APROVADO
        ↓
PREPARAÇÃO DA TAREFA
        ↓
LEITURA DO CONTEÚDO MESTRE
        ↓
MAPEAMENTO SEMÂNTICO
        ↓
CLASSIFICAÇÃO EDITORIAL
        ↓
HERANÇA DA INFRAESTRUTURA
        ↓
SELEÇÃO DE COMPONENTES
        ↓
IDENTIFICAÇÃO DE FUNÇÕES NOVAS
        ↓
CONSTRUÇÃO HTML
        ↓
APLICAÇÃO / EXTENSÃO DO CSS
        ↓
PAGINAÇÃO E ATOMICIDADE
        ↓
AUDITORIA ESTÁTICA
        ↓
PDF OFICIAL — WINDOWS + CHROME
        ↓
PREFLIGHT
        ↓
HÁ DEFEITO REAL?
      ↙             ↘
    NÃO              SIM
     ↓                ↓
 APROVAR          CLASSIFICAR
     ↓                ↓
 CONGELAR         PATCH MÍNIMO
                      ↓
                  REGENERAR
                      ↓
                  REVALIDAR
                      ↓
                   PREFLIGHT
```

O percurso completo pode ser condensado em:

**ENTENDER → CLASSIFICAR → HERDAR → CONSTRUIR → VALIDAR → CORRIGIR SOMENTE O NECESSÁRIO → CONGELAR**

---

# 4. ESTADOS DE UMA APOSTILA

O fluxo utiliza poucos estados, cada um associado a uma mudança real do trabalho.

| Estado | Significado |
|---|---|
| **CONTEÚDO APROVADO** | O conteúdo mestre está suficientemente estável para entrar em produção editorial. |
| **EM PREPARAÇÃO** | Escopo, entradas, saídas e documentos vigentes estão sendo organizados. |
| **EM CONSTRUÇÃO** | HTML/CSS ainda está sendo estruturado, classificado, estilizado ou paginado. |
| **CANDIDATA A PDF** | Construção e auditoria estática foram concluídas; o material está apto à geração oficial. |
| **PDF EM PREFLIGHT** | O PDF oficial está sendo avaliado como produto final. |
| **EM CORREÇÃO** | Existe defeito real identificado que exige intervenção. |
| **APROVADA** | O preflight não encontrou defeitos que impeçam o encerramento. |
| **CONGELADA** | A versão aprovada foi encerrada e passa a ser preservada como estado final. |
| **REABERTA EXCEPCIONALMENTE** | Uma versão congelada voltou ao fluxo por motivo real e documentável. |

Estados não devem ser multiplicados para representar pequenas tarefas internas.

---

# 5. ENTRADAS OBRIGATÓRIAS

Uma nova produção utiliza normalmente:

- conteúdo mestre aprovado;
- Regras Gerais vigentes;
- Arquitetura Técnica vigente;
- Catálogo de Componentes vigente;
- instruções específicas da apostila;
- HTML/CSS Base, quando existir.

Também deve estar identificada a **versão vigente** dos documentos canônicos utilizados.

Precedentes anteriores não fazem parte da leitura obrigatória por padrão.

Devem ser consultados apenas quando:

- houver dúvida real não resolvida pelos documentos canônicos;
- for necessário confirmar comportamento de solução já aprovada;
- for necessário compreender um caso concreto de patch, preflight ou congelamento;
- a Base ainda não existir e for preciso materializar um detalhe não suficientemente determinado pela Arquitetura Técnica.

Princípio:

> **Consultar o menor precedente suficiente.**

Se ainda não existir HTML/CSS Base definitivo, a construção deve derivar do Documento 03 e recorrer apenas ao precedente mínimo necessário.

---

# 6. FASE 0 — PREPARAÇÃO DA TAREFA

**Estado:** CONTEÚDO APROVADO → EM PREPARAÇÃO

## Objetivo

Definir com precisão o que será produzido antes de iniciar implementação ou redesign.

## Verificar

- tópico;
- bloco, quando houver;
- nome completo da apostila;
- conteúdo mestre correspondente;
- arquivos de entrada;
- arquivos de saída;
- documentos canônicos vigentes;
- instruções específicas;
- necessidades especiais já conhecidas;
- existência ou não de HTML/CSS Base;
- existência de componentes já identificados como provavelmente necessários.

Não se decide nesta fase a aparência local de cada elemento.

## Saída

**ESCOPO DE PRODUÇÃO DEFINIDO**

A produção só avança quando é possível identificar claramente qual conteúdo será materializado e quais artefatos finais deverão corresponder entre si.

---

# 7. FASE 1 — LEITURA DO CONTEÚDO MESTRE

**Estado:** EM PREPARAÇÃO → EM CONSTRUÇÃO

## Objetivo

Compreender o material antes de representá-lo.

## Identificar

- Texto Teórico e Texto Prático;
- Partes;
- seções e subseções;
- sequência pedagógica;
- definições;
- fórmulas e notações;
- exemplos;
- tabelas;
- exercícios;
- quiz, quando existir;
- gabarito;
- relações matemáticas importantes;
- traduções entre representações;
- visuais previstos;
- unidades que possuem dependência forte entre si.

A leitura deve procurar estrutura e função, não oportunidades de decoração.

Não se decide ainda a quebra exata de páginas.

## Saída

**MAPA BRUTO DO CONTEÚDO**

---

# 8. FASE 2 — MAPEAMENTO SEMÂNTICO

## Objetivo

Transformar o mapa bruto em unidades editoriais explícitas.

Uma estrutura possível é:

```text
TEXTO TEÓRICO
├── PARTE I
├── PARTE II
└── PARTE III

TEXTO PRÁTICO
├── EXEMPLOS RESOLVIDOS
├── QUIZ, quando aplicável
├── EXERCÍCIOS
└── GABARITO COMENTADO
```

A quantidade e a presença dessas unidades dependem do conteúdo mestre.

Também devem ser reconhecidas funções locais, como:

- definição;
- princípio;
- observação;
- objeto imediato de análise;
- comparação;
- tradução entre representações;
- tabela;
- investigação;
- tentativa;
- argumento;
- demonstração;
- resposta;
- estrutura exercício ↔ gabarito.

A função semântica deve ser reconhecida antes de qualquer decisão sobre componente.

## Saída

**ESTRUTURA SEMÂNTICA DA APOSTILA**

---

# 9. FASE 3 — CLASSIFICAÇÃO EDITORIAL

## Objetivo

Definir qual nível de representação cada unidade exige.

## Classificar

Conforme a função, o conteúdo pode permanecer como:

- prosa normal;
- matemática inline;
- matemática em linha própria;
- matemática estrutural;
- tabela;
- componente catalogado;
- visual específico;
- estrutura paralela entre exercício e gabarito;
- extensão local, somente quando necessária.

A pergunta central é:

> **Já existe solução aprovada para esta função?**

A ordem de preferência é:

1. prosa;
2. tipografia e hierarquia;
3. espaçamento;
4. estrutura HTML;
5. matemática fundamental;
6. tabela;
7. componente existente;
8. extensão local nova.

Essa ordem não significa que toda decisão precise percorrer mecanicamente oito etapas. Ela estabelece uma preferência pela solução mais simples suficiente.

## Saída

**MAPA EDITORIAL**

---

# 10. FASE 4 — INSTANCIAÇÃO DA INFRAESTRUTURA

## Objetivo

Criar o chassi técnico sem copiar resíduos de apostilas anteriores.

## Quando existir HTML/CSS Base

Instanciar a Base vigente e preencher apenas o que pertence à nova apostila.

Preparar, conforme definido pela Arquitetura Técnica:

- metadados;
- tema;
- capa;
- identidade documental;
- cabeçalho;
- rodapé;
- estrutura de fonte semântica;
- seções-fonte;
- contextos de cabeçalho;
- infraestrutura de paginação e impressão.

## Quando ainda não existir HTML/CSS Base definitivo

Materializar somente o núcleo definido pelo Documento 03.

Não utilizar a última apostila completa como template informal.

Precedente anterior pode esclarecer um ponto real, mas não substituir a Arquitetura Técnica.

## Saída

**CHASSI TÉCNICO DA APOSTILA**

---

# 11. FASE 5 — SELEÇÃO DE COMPONENTES

## Objetivo

Selecionar somente componentes cuja função já foi identificada no mapa editorial.

O Documento 04 deve ser consultado por necessidade, não como lista de recursos a preencher.

Exemplos de consulta funcional:

- definição formal → componente de definição, quando adequado;
- tabela de análise → componente tabular correspondente;
- estrutura parcialmente vazia → componente de investigação, quando adequado;
- tentativa → componente de tentativa, quando adequado;
- premissas → conclusão → estrutura inferencial, quando adequado.

A existência de nomes como `definition-box`, `analysis-table`, `worksheet-table`, `attempt-block` ou `argument-stack` não obriga seu uso. A decisão depende do contrato semântico registrado no Catálogo.

Não selecionar componente porque:

- existe;
- ficou visualmente interessante;
- apareceu em outro bloco;
- parece tornar a página mais completa.

## Saída

**REPERTÓRIO DE COMPONENTES DA APOSTILA**

---

# 12. FASE 6 — IDENTIFICAÇÃO DE FUNÇÕES NOVAS

## Objetivo

Distinguir necessidade real de novidade decorativa.

Pergunta:

> **Há alguma relação pedagógica importante que o sistema atual ainda não sabe representar adequadamente?**

Se a resposta for **não**, não se cria componente novo.

Se a resposta for **sim**, seguir:

```text
FUNÇÃO NOVA
    ↓
SOLUÇÃO MAIS SIMPLES SUFICIENTE
    ↓
EXTENSÃO LOCAL
    ↓
TESTE EM CONTEÚDO REAL
    ↓
VALIDAÇÃO NO PDF
```

Uma extensão local não é promovida automaticamente a componente canônico.

Eventual promoção pertence a avaliação posterior, baseada em reutilização, clareza funcional, estabilidade e sobrevivência ao produto real.

## Saída

**EXTENSÕES LOCAIS JUSTIFICADAS**, quando houver.

Na ausência de função nova, a saída é simplesmente a confirmação de que a infraestrutura e os componentes existentes são suficientes.

---

# 13. FASE 7 — CONSTRUÇÃO HTML

## Objetivo

Materializar integralmente a estrutura semântica e editorial do conteúdo.

Ao final desta fase, o HTML deve conter:

- conteúdo mestre integral;
- ordem correta;
- seções-fonte corretas;
- headings semanticamente adequados;
- componentes necessários;
- matemática classificada;
- tabelas reais;
- atributos de contexto;
- atributos de atomicidade somente quando necessários;
- estrutura compatível com outline e paginação.

A construção não deve:

- reescrever teoria por conveniência de layout;
- cortar conteúdo para caber em página;
- duplicar trechos;
- corrigir silenciosamente conteúdo mestre;
- inserir quebras artificiais para “montar” páginas manualmente;
- promover visualmente trechos sem função correspondente.

Se a construção revelar problema conceitual no conteúdo, o problema retorna ao conteúdo mestre ou exige autorização explícita de correção.

## Saída

**HTML SEMÂNTICO COMPLETO**

---

# 14. FASE 8 — APLICAÇÃO E EXTENSÃO DO CSS

## Objetivo

Aplicar identidade, infraestrutura e componentes sem acumular herança histórica desnecessária.

O movimento esperado é:

```text
CSS BASE
+
COMPONENTES NECESSÁRIOS
+
EXTENSÃO LOCAL MÍNIMA
```

Não:

```text
CSS COMPLETO DO BLOCO ANTERIOR
+
RESÍDUOS
+
PATCHES ACUMULADOS
```

## Verificar

- CSS morto;
- seletores sem uso;
- herança desnecessária;
- redefinições globais indevidas;
- valores locais que deveriam utilizar tokens existentes;
- contaminação da infraestrutura por componente específico;
- duplicação de regras que a Base ou o Catálogo já resolvem.

## Saída

**HTML/CSS CANDIDATO À PAGINAÇÃO**

---

# 15. FASE 9 — PAGINAÇÃO E ATOMICIDADE

## Objetivo

Fazer a estrutura renderizada respeitar dependências pedagógicas sem transformar páginas em caixas rígidas.

Aplicar a Arquitetura Técnica vigente aos elementos pertinentes, incluindo, quando necessários:

- contexto de seção;
- seções-fonte;
- aberturas de Parte;
- aberturas de seção;
- `keep-with-next`;
- `data-keep-count`;
- `atomic-group`;
- tabelas;
- visuais;
- exercícios e respostas longas.

Princípio:

> **Proteja dependências pequenas; deixe unidades longas quebrarem naturalmente.**

Uma unidade longa não deve ser tornada atomicamente indivisível apenas para evitar uma quebra normal.

Não se pagina para alcançar preenchimento geométrico uniforme.

O preview serve para detectar problemas e ajustar contratos de paginação. A autoridade final continua pertencendo ao PDF oficial.

## Saída

**DOCUMENTO PAGINADO EM PREVIEW**

---

# 16. FASE 10 — AUDITORIA ESTÁTICA

## Objetivo

Impedir que problemas detectáveis no código ou no preview sejam enviados desnecessariamente ao ciclo de PDF.

A auditoria deve cobrir pelo menos cinco eixos.

## A. Conteúdo

Verificar:

- integridade do conteúdo;
- ordem correta;
- correspondência entre exercícios e respostas;
- ausência de duplicação;
- ausência de omissão.

## B. HTML

Verificar:

- estrutura de tags;
- IDs;
- headings;
- contextos;
- semântica;
- outline esperado;
- atributos estruturais necessários.

## C. CSS

Verificar:

- seletores mortos relevantes;
- overflow previsível;
- CSS herdado sem uso;
- redefinições indevidas;
- componentes corretamente carregados;
- extensão local confinada ao seu alcance.

## D. Matemática

Verificar:

- inline;
- linha própria;
- estrutural;
- símbolos;
- glifos previsíveis;
- quebras;
- hierarquia;
- relações preservadas.

## E. Componentes

Verificar:

- função correta;
- ausência de uso decorativo;
- ausência de redundância;
- exercício não revela resposta;
- paginação compatível com o componente;
- variante escolhida somente quando necessária.

## Saída

**CANDIDATA A PDF**

Se a auditoria revelar problema real, o material permanece **EM CONSTRUÇÃO** até a correção.

---

# 17. FASE 11 — GERAÇÃO DO PDF OFICIAL

**Estado:** CANDIDATA A PDF → PDF EM PREFLIGHT

O fluxo oficial é:

```text
HTML/CSS CANDIDATO
        ↓
WINDOWS + CHROME
        ↓
PDF OFICIAL
```

Outros renderizadores podem auxiliar durante desenvolvimento e diagnóstico.

Eles não possuem autoridade final sobre paginação, quebras ou acabamento oficial.

O procedimento técnico específico de geração não pertence a este documento.

## Saída

**PDF DE PRODUÇÃO**

---

# 18. FASE 12 — PREFLIGHT

## Objetivo

Validar o produto real que será estudado e preservado.

O preflight possui cinco eixos.

## 18.1 Estrutural

Verificar:

- número e ordem de páginas;
- clipping;
- overflow;
- quebras inadequadas;
- tabelas;
- visuais;
- páginas vazias acidentais;
- integridade de cabeçalhos e rodapés.

## 18.2 Textual

Verificar:

- presença do conteúdo;
- símbolos;
- caracteres;
- respostas;
- ausência de perda, duplicação ou corrupção textual.

## 18.3 Visual

Verificar:

- hierarquia;
- alinhamentos;
- relações visuais;
- legibilidade;
- espaço branco legítimo;
- ausência de composição que sugira relação inexistente.

## 18.4 Tipográfico

Verificar:

- fontes;
- glifos;
- matemática;
- compatibilidade e incorporação quando relevantes ao produto final.

## 18.5 Navegação

Verificar:

- outline;
- bookmarks;
- ordem;
- nomes;
- níveis necessários;
- ausência de entradas acidentais.

## Saída

Uma das duas:

**PDF LIMPO**

ou

**LISTA DE DEFEITOS REAIS**

---

# 19. FASE 13 — CLASSIFICAÇÃO DE DEFEITOS

Todo problema encontrado no preflight deve ser classificado antes de qualquer correção.

## A — DEFEITO CRÍTICO

Exemplos:

- conteúdo ausente;
- erro matemático ou conceitual presente no produto;
- resposta indevidamente revelada;
- clipping;
- overflow;
- bookmark quebrado;
- glifo corrompido;
- estrutura necessária ausente;
- perda textual;
- relação visual que altera o sentido.

**Ação:** corrigir obrigatoriamente.

Quando o defeito estiver no conteúdo mestre, a correção deve ocorrer na origem apropriada; não apenas no HTML final.

## B — DEFEITO REAL LOCAL

Exemplos:

- quebra inadequada;
- espaçamento localizado com impacto real;
- largura inadequada;
- alinhamento defeituoso;
- composição específica prejudicial;
- atomicidade mal calibrada.

**Ação:** patch mínimo.

## C — IMPERFEIÇÃO COSMÉTICA

Exemplos:

- preferência estética;
- possibilidade de preencher mais uma página;
- diferença mínima sem impacto;
- alternativa ligeiramente mais elegante;
- microvariação visual que não compromete função.

**Ação:** normalmente preservar.

A classificação impede que toda observação de preflight seja tratada como motivo de redesign.

---

# 20. FASE 14 — PATCH MÍNIMO

**Estado:** PDF EM PREFLIGHT → EM CORREÇÃO

## Princípio

> **Corrigir a causa com a menor superfície de alteração.**

Exemplo:

**Problema:** uma tabela específica ultrapassa a largura útil.

Não presumir que todas as tabelas precisam ser reduzidas.

Preferir corrigir:

- a instância;
- a variante;
- o contrato local;
- ou, se for realmente a causa, o componente responsável.

A superfície do patch deve acompanhar o alcance do defeito.

Quanto mais madura a apostila, menor deve ser a área reaberta.

Patch local não é oportunidade para:

- limpar todo o CSS;
- redesenhar páginas já aprovadas;
- substituir componentes funcionais;
- uniformizar retrospectivamente decisões antigas.

## Saída

**VERSÃO CORRIGIDA**

---

# 21. FASE 15 — REGENERAÇÃO E REVALIDAÇÃO

## Objetivo

Confirmar que o defeito foi eliminado sem produzir regressões.

O movimento é:

```text
HTML/CSS CORRIGIDO
        ↓
NOVO PDF OFICIAL
        ↓
VERIFICAÇÃO DO DEFEITO
        +
VERIFICAÇÃO DOS EFEITOS COLATERAIS PLAUSÍVEIS
```

A extensão da revalidação deve ser proporcional à extensão da mudança.

Exemplo:

**Patch de espaçamento em uma tabela**

Verificar:

- a tabela;
- a página;
- páginas cuja paginação possa ter mudado;
- outline apenas se a estrutura afetada puder alterá-lo.

Não refazer automaticamente toda a auditoria conceitual de um documento cuja essência permaneceu congelada.

Se o patch atingir infraestrutura, componente compartilhado ou comportamento de paginação geral, a revalidação deve se ampliar para todas as instâncias plausivelmente afetadas.

## Saída

**PDF REVALIDADO**

O documento retorna ao preflight até não existir defeito real impeditivo.

---

# 22. FASE 16 — APROVAÇÃO E CONGELAMENTO

**Estado:** PDF EM PREFLIGHT → APROVADA → CONGELADA

Uma apostila pode ser aprovada quando:

- conteúdo está correto;
- estrutura está correta;
- PDF está íntegro;
- paginação está aceitável;
- matemática está legível;
- outline está correto;
- não existem defeitos críticos;
- não existem defeitos locais relevantes;
- eventuais problemas restantes são apenas cosméticos e não justificam nova rodada.

O congelamento encerra a superfície normal de alteração.

Após o congelamento:

- não realizar polimento indefinido;
- não reabrir para melhorar preferências estéticas;
- não redesenhar para aproximar uma apostila antiga de uma mais recente.

## Saída

**VERSÃO FINAL CONGELADA**

---

# 23. PÓS-CONGELAMENTO

O estado congelado deve preservar de forma coerente:

- HTML aprovado;
- CSS aprovado;
- PDF correspondente;
- identidade da versão;
- conteúdo mestre e fontes necessárias à manutenção, quando aplicável;
- registro documental suficiente para reconhecer o estado final.

HTML, CSS e PDF devem representar o mesmo estado aprovado.

O procedimento Git detalhado não pertence a este documento.

O congelamento deve tornar possível distinguir claramente:

**versão oficial preservada**  
de  
**trabalho posterior ainda não aprovado**.

---

# 24. REABERTURA EXCEPCIONAL

Uma versão congelada só deve voltar ao fluxo quando houver motivo real.

Exemplos:

- erro conceitual descoberto;
- conteúdo incorreto;
- problema técnico relevante;
- incompatibilidade de renderização com impacto;
- mudança normativa crítica que torne a versão inadequada;
- defeito editorial com impacto pedagógico ou documental real.

Não reabrir por:

- preferência estética tardia;
- desejo de uniformizar documentos antigos;
- diferença mínima de espaçamento;
- simples existência de solução mais recente;
- possibilidade abstrata de “ficar melhor”.

A reabertura deve começar pelo diagnóstico do alcance do problema.

Somente as fases necessárias são reativadas.

O novo Fluxo não obriga retronormalização dos Blocos I–V nem de outras apostilas já congeladas que continuem corretas.

---

# 25. FLUXOS ABREVIADOS DE MANUTENÇÃO

Nem toda tarefa exige o fluxo completo.

## 25.1 Construção nova

Executa as fases principais:

**0 → 16**

A ordem pode conter pequenas iterações internas, mas nenhuma fase estrutural relevante deve ser omitida.

## 25.2 Patch local

```text
DIAGNÓSTICO LOCALIZADO
        ↓
CLASSIFICAÇÃO DO DEFEITO
        ↓
PATCH MÍNIMO
        ↓
NOVO PDF OFICIAL
        ↓
PREFLIGHT LOCALIZADO + EFEITOS PLAUSÍVEIS
        ↓
RECONGELAMENTO
```

Uma quebra ruim em uma página não justifica refazer o mapeamento semântico da apostila inteira.

## 25.3 Correção textual mínima

Quando a correção pertence ao conteúdo:

```text
CORRIGIR NA ORIGEM APROPRIADA
        ↓
ATUALIZAR HTML CORRESPONDENTE
        ↓
REGERAR PDF
        ↓
VERIFICAR O TRECHO
        ↓
VERIFICAR PAGINAÇÃO AFETADA
        ↓
RECONGELAR
```

Correção textual não deve ser feita silenciosamente apenas na camada HTML quando altera o conteúdo mestre.

## 25.4 Ajuste de componente

```text
IDENTIFICAR ALCANCE DO COMPONENTE
        ↓
PATCH
        ↓
VERIFICAR TODAS AS INSTÂNCIAS AFETADAS
        ↓
GERAR PDF
        ↓
PREFLIGHT PROPORCIONAL
        ↓
RECONGELAR
```

Quanto mais compartilhado o componente, maior a área mínima de revalidação.

## 25.5 Correção sistêmica

Quando o defeito pertence à infraestrutura ou a uma decisão canônica:

```text
IDENTIFICAR DEFEITO SISTÊMICO
        ↓
NÃO CORRIGIR SILENCIOSAMENTE APENAS NA APOSTILA
        ↓
IDENTIFICAR DOCUMENTO / IMPLEMENTAÇÃO CANÔNICA RESPONSÁVEL
        ↓
REVISAR O SISTEMA PELO PROCESSO ADEQUADO
        ↓
APLICAR ÀS PRODUÇÕES REALMENTE AFETADAS
```

Uma correção sistêmica não implica retronormalização indiscriminada de documentos congelados.

---

# 26. CUSTO PROPORCIONAL E SUPERFÍCIE DE ALTERAÇÃO

O fluxo adota o princípio:

> **Quanto menor o impacto pedagógico, editorial ou técnico de um problema, menor deve ser o custo operacional aceitável para corrigi-lo.**

Em termos práticos:

| Tipo | Resposta |
|---|---|
| **Defeito crítico** | Investigação e correção necessárias; revalidação compatível com o alcance. |
| **Defeito real local** | Menor ferramenta, patch e preflight suficientes. |
| **Imperfeição cosmética** | Normalmente nenhum novo ciclo. |

O mesmo princípio vale para contexto.

Uma tarefa local não deve carregar toda a história do projeto.

Uma construção nova precisa do sistema vigente, mas não de releitura integral de todas as apostilas anteriores.

> **O passado deve ser condensado em sistema, não reaprendido indefinidamente.**

---

# 27. CRITÉRIOS DE PARADA

O fluxo termina quando todas as condições abaixo são verdadeiras:

- não há defeito crítico;
- não há defeito real relevante;
- o produto cumpre sua função pedagógica;
- o produto cumpre sua função editorial;
- o PDF oficial está íntegro;
- novas alterações seriam predominantemente preferência, não correção.

Critério canônico:

> **A ausência de perfeição absoluta não impede o congelamento; a presença de defeito real, sim.**

Também deve ser interrompido um ciclo de revisão quando sucessivas alterações passam a trocar uma solução correta por outra igualmente correta sem ganho funcional verificável.

O objetivo do preflight é encontrar defeitos, não produzir uma sequência infinita de preferências.

---

# 28. MATRIZ DE ENTRADAS E SAÍDAS

| Fase | Entrada principal | Saída |
|---|---|---|
| **0 — Preparação** | conteúdo aprovado + documentos vigentes + instruções | escopo de produção definido |
| **1 — Leitura** | conteúdo mestre | mapa bruto do conteúdo |
| **2 — Mapeamento** | mapa bruto | estrutura semântica |
| **3 — Classificação** | estrutura semântica | mapa editorial |
| **4 — Infraestrutura** | Arquitetura Técnica / Base | chassi técnico |
| **5 — Componentes** | mapa editorial + Catálogo | repertório selecionado |
| **6 — Funções novas** | lacunas reais de representação | extensões locais justificadas, se necessárias |
| **7 — HTML** | conteúdo + mapa editorial + chassi | HTML semântico completo |
| **8 — CSS** | Base + componentes + extensões | HTML/CSS candidato à paginação |
| **9 — Paginação** | HTML/CSS | preview paginado |
| **10 — Auditoria** | preview + código | candidata a PDF |
| **11 — PDF** | candidata a PDF | PDF oficial de produção |
| **12 — Preflight** | PDF oficial | PDF limpo ou lista de defeitos |
| **13 — Classificação** | defeitos | criticidade e alcance definidos |
| **14 — Patch** | defeito classificado | versão corrigida |
| **15 — Revalidação** | versão corrigida | PDF revalidado |
| **16 — Congelamento** | PDF aprovado | versão final congelada |

---

# 29. CHECKLIST OPERACIONAL DE CONSTRUÇÃO NOVA

- [ ] Conteúdo mestre aprovado.
- [ ] Documentos canônicos vigentes identificados.
- [ ] Escopo e arquivos de saída definidos.
- [ ] Conteúdo lido integralmente.
- [ ] Macroestrutura mapeada.
- [ ] Funções editoriais classificadas.
- [ ] Base ou infraestrutura instanciada.
- [ ] Componentes selecionados por função.
- [ ] Funções novas identificadas.
- [ ] Extensões locais justificadas, quando necessárias.
- [ ] HTML completo e fiel ao conteúdo.
- [ ] CSS sem herança morta relevante.
- [ ] Paginação e atomicidade configuradas.
- [ ] Auditoria estática concluída.
- [ ] PDF oficial gerado em Windows + Chrome.
- [ ] Preflight concluído.
- [ ] Defeitos classificados.
- [ ] Patches mínimos aplicados quando necessários.
- [ ] PDF regenerado e revalidado.
- [ ] Critérios de parada satisfeitos.
- [ ] Versão congelada.

---

# 30. TESTE DE NÃO BUROCRATIZAÇÃO

O fluxo deve continuar respondendo corretamente aos seguintes casos.

## Caso A — Nova apostila

**Pergunta:** uma nova apostila precisa das fases principais?

**Resposta:** sim.

Ela precisa compreender, classificar, herdar, construir, paginar, gerar o produto real, validar e congelar.

## Caso B — Quebra ruim em uma página

**Pergunta:** uma correção de margem, espaçamento ou quebra localizada precisa percorrer as 16 fases?

**Resposta:** não.

Utiliza diagnóstico localizado, classificação, patch mínimo, regeneração e preflight proporcional.

## Caso C — Função visual nova

**Pergunta:** um visual novo deve virar componente canônico durante a própria construção?

**Resposta:** não.

Primeiro surge como extensão local justificada, é testado em conteúdo real e sobrevive ao PDF. Eventual promoção é decisão posterior.

## Caso D — Problema de infraestrutura

**Pergunta:** um defeito sistêmico deve ser escondido por patch exclusivo em uma apostila?

**Resposta:** não.

A causa deve retornar ao nível canônico responsável.

---

# 31. ECONOMIA DE CONTEXTO

O fluxo normal não exige:

- leitura de todas as apostilas anteriores;
- leitura de todo precedente disponível;
- consulta de componentes sem relação com o conteúdo;
- reconstrução histórica de decisões já formalizadas.

Uma nova construção deve trabalhar com:

- conteúdo mestre;
- documentos canônicos vigentes;
- partes do Catálogo pertinentes às funções identificadas;
- instruções específicas;
- precedente mínimo, somente quando necessário.

O Documento 06 definirá como esse conjunto será entregue e operado por agentes.

Este documento define apenas o princípio:

> **O fluxo seleciona contexto; não acumula contexto.**

---

# 32. RELAÇÃO COM O GUIA CODEX

O Documento 05 define:

**O PROCESSO.**

O Documento 06 definirá:

**COMO O AGENTE EXECUTA O PROCESSO COM CONTEXTO, AUTONOMIA E CUSTO ADEQUADOS.**

Por isso, este Fluxo não determina:

- formato de prompt;
- modelo a utilizar;
- políticas de commit;
- comandos;
- limites de uso;
- divisão detalhada de tarefas entre agentes;
- instruções operacionais de ferramentas.

O Guia Codex deve herdar este fluxo sem duplicá-lo integralmente.

---

# 33. QUESTÕES ABERTAS

As seguintes questões permanecem deliberadamente abertas até que exista base suficiente para decisão:

- em que etapa a futura Base HTML/CSS será formalmente validada como artefato canônico;
- se o congelamento deverá sempre corresponder a uma tag ou outro marcador específico no Git;
- quais partes da auditoria estática poderão ser automatizadas com segurança;
- quais partes do preflight poderão ser automatizadas sem substituir inspeção do PDF real;
- em que momento uma extensão local deverá receber registro formal como candidata a componente;
- como o fluxo precisará ser ampliado para gráficos, imagens, construções geométricas e outras representações tecnicamente complexas;
- quais aspectos deste fluxo poderão ser generalizados para outros Planos de Estudo após experiência empírica suficiente.

A ausência de decisão deve permanecer explícita.

Não se cria norma futura por antecipação.

---

# 34. BASE EMPÍRICA E DOCUMENTAL

Este Fluxo foi consolidado a partir de:

- **Documento 01 — Arquitetura e Taxonomia Canônica do Sistema de Apostilas — Versão 1.0**;
- **Documento 02 — Regras Gerais HTML/CSS do Plano de Estudo Matemático — Versão 3.0**;
- **Documento 03 — Arquitetura Técnica HTML/CSS do Plano de Estudo Matemático — Versão 1.0**;
- **Documento 04 — Catálogo de Componentes HTML/CSS do Plano de Estudo Matemático — Versão 1.0**;
- relatórios de transição e consolidação produzidos entre esses documentos;
- experiência acumulada na produção, correção, geração e congelamento dos Blocos I–V do Tópico 1.1 — Lógica Matemática.

Os precedentes do Tópico 1.1 constituem base empírica do sistema, mas não precisam ser relidos integralmente em cada nova produção.

---

# 35. SÍNTESE OPERACIONAL

O Fluxo de Produção pode ser reduzido às seguintes decisões:

1. **Entender antes de construir.**
2. **Classificar antes de representar.**
3. **Uma apostila herda antes de criar.**
4. **Base estável; extensão local.**
5. **Paginar por dependência, não por preenchimento.**
6. **Validar o produto real.**
7. **Corrigir a causa com a menor superfície de alteração.**
8. **Quanto mais madura a apostila, menor a superfície de alteração.**
9. **O custo da correção deve ser proporcional ao impacto.**
10. **O fluxo seleciona contexto; não acumula contexto.**
11. **Uma tarefa local não percorre desnecessariamente um fluxo de construção nova.**
12. **A ausência de perfeição absoluta não impede o congelamento; a presença de defeito real, sim.**
13. **O passado deve ser condensado em sistema, não reaprendido indefinidamente.**

O fluxo começa com conteúdo aprovado.

Termina quando HTML, CSS e PDF formam uma versão coerente, validada e congelada.

Entre esses dois pontos, toda etapa deve alterar o estado do trabalho ou impedir um erro real.

Se apenas repete informação que já pertence a outro documento, não pertence a este Fluxo.
