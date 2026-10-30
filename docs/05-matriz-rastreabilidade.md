# 05\. Matriz de rastreabilidade

## 1\. Objetivo

Estabelecer a relação entre as necessidades do negócio, os requisitos, as regras de negócio, os casos de teste e as evidências esperadas, permitindo verificar se cada necessidade está contemplada e se os critérios de aceite poderão ser demonstrados.

A matriz também apoia a análise de impacto de mudanças, a identificação de lacunas e o acompanhamento da validação da solução proposta.

#### 

#### 2\. Status

Matriz inicial elaborada para um caso simulado de Análise de Negócios. Os vínculos, critérios de aceite e evidências são propostas que dependem de validação com os responsáveis de negócio e de execução dos testes.



## 3\. Matriz de rastreabilidade

|Necessidade de negócio|Requisito|Regra associada|Caso de teste|Evidência de aceite esperada|Status|
|-|-|-|-|-|-|
|NB01 — Consultar o indicador com critérios definidos|RF01 — Consulta por período e dimensões|RN01, RN02 e RN06|CT01 — Consulta e conferência do indicador|Resultado reproduzível para o período, filtros, escopo e definição aprovados|Pendente|
|NB02 — Identificar divergências entre resultados comparáveis|RF02 — Identificação de divergências|RN02, RN06 e RN08|CT02 — Comparação entre fontes|Diferença identificada sob critérios equivalentes, com valores e condições da comparação registrados|Pendente|
|NB03 — Investigar a origem dos valores|RF03 — Rastreabilidade dos registros|RN07|CT03 — Rastreamento da origem|Registros de origem localizados e relacionados ao valor analisado, conforme a granularidade definida|Pendente|
|NB04 — Registrar e acompanhar inconsistências|RF04 — Registro e tratamento de ocorrências|RN05 e RN08|CT04 — Registro e acompanhamento|Ocorrência registrada com status, responsável, evidências e justificativa quando aplicável|Pendente|
|NB05 — Consultar detalhes necessários à investigação|RF05 — Detalhamento da análise|RN07 e RN10|CT05 — Consulta de detalhes e permissões|Usuário autorizado acessa as informações previstas; acesso não autorizado é tratado conforme os requisitos de segurança|Pendente|
|NB04 — Acompanhar a validação após o tratamento|RF06 — Registro da validação|RN05 e RN08|CT06 — Revalidação da ocorrência|Resultado da verificação registrado, com conclusão e evidência vinculadas à ocorrência|Pendente|
|NB04 — Consultar o histórico das alterações|RF07 — Histórico de alterações|RN05 e RN10|CT07 — Consulta do histórico|Alterações relevantes podem ser identificadas com data, responsável, motivo e versão, conforme o escopo aprovado|Pendente|

\*\*Observação:\*\* os identificadores NB01–NB05, RF01–RF07 e RN01–RN10 devem permanecer consistentes com os documentos de requisitos e regras de negócio. Os casos CT01–CT07 são propostos e ainda precisam ser detalhados no plano de testes.



## 4\. Controle de cobertura

A matriz deverá ser revisada para identificar as seguintes situações:

|Verificação|Critério|Tratamento quando houver lacuna|
|-|-|-|
|Necessidade sem requisito|Toda necessidade aprovada deve estar contemplada por um ou mais requisitos|Registrar a lacuna e avaliar o requisito necessário|
|Requisito sem necessidade relacionada|Todo requisito deve ter justificativa de negócio ou técnica|Confirmar a necessidade ou avaliar a exclusão|
|Requisito sem regra associada|Verificar se a execução depende de regra de negócio|Identificar a regra necessária ou justificar a ausência de vínculo|
|Regra sem requisito ou controle relacionado|Avaliar como a regra será aplicada e verificada|Relacionar a requisito, controle ou teste pertinente|
|Requisito sem caso de teste|Todo requisito verificável deve possuir forma de validação definida|Criar o teste ou documentar e aprovar a justificativa|
|Teste sem critério de aceite|O resultado esperado deve ser objetivo e verificável|Definir o critério antes da execução|
|Teste sem evidência prevista|Deve ser possível demonstrar o resultado obtido|Definir qual registro, comparação ou documento comprovará o resultado|
|Mudança de requisito ou regra|Os vínculos impactados devem ser identificados|Revisar requisitos, regras, testes e critérios de aceite relacionados|



## 5\. Gestão de mudanças e impactos

Quando houver alteração em uma necessidade, requisito ou regra de negócio, deverão ser avaliados:

1\. Os requisitos e regras diretamente afetados.

2\. Os casos de teste que precisam ser criados ou revisados.

3\. Os critérios de aceite que podem deixar de ser válidos.

4\. As evidências que precisam ser atualizadas ou reexecutadas.

5\. Os impactos nas etapas do processo e nos controles propostos.

6\. A necessidade de nova aprovação pelo responsável de negócio.

As alterações deverão ser registradas com identificador, descrição, justificativa, responsável, data e itens impactados.



## 6\. Critérios de aceite da matriz

A matriz poderá ser considerada validada quando:

\- As necessidades de negócio estiverem identificadas e aprovadas.

\- Os requisitos relacionados estiverem documentados e priorizados.

\- As regras aplicáveis estiverem associadas aos requisitos pertinentes.

\- Os casos de teste cobrirem os requisitos verificáveis.

\- Os critérios de aceite e as evidências esperadas estiverem definidos.

\- As lacunas e dependências estiverem registradas.

\- As mudanças puderem ser rastreadas até os artefatos afetados.

A conclusão da rastreabilidade documental não comprova, isoladamente, que o indicador está correto. A correção deverá ser demonstrada por meio de regras aprovadas, dados adequados e testes executados com resultados registrados.



## 7\. Limitações e próximos passos

Esta matriz é inicial e conceitual. Os vínculos propostos ainda precisam ser revisados conforme as necessidades e regras forem validadas.

O próximo passo é detalhar os casos de teste no plano de testes, definindo objetivo, pré-condições, dados de entrada, procedimento, resultado esperado, resultado obtido e evidência. Após a execução, os status deverão ser atualizados com base nos resultados reais, sem antecipar aprovações ou conclusões.



