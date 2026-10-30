# 03\. Regras de negócio

## 1\. Objetivo

Definir os critérios que deverão orientar a interpretação, a comparação e a validação dos indicadores, estabelecendo condições verificáveis para o tratamento das divergências.

As regras apresentadas são propostas iniciais. Sua aplicação depende da análise das fontes, do levantamento das exceções e da aprovação dos responsáveis de negócio.

\*\*Status:\*\* proposto para validação. Nenhuma regra foi declarada oficialmente aprovada.



## \## 2. Regras de negócio propostas

|ID|Regra|Critério de aplicação|Evidência necessária|Status|
|-|-|-|-|-|
|RN01|Cada indicador deve possuir definição e fórmula documentadas|Registrar finalidade, fórmula, unidade de medida, filtros e critérios de inclusão e exclusão|Definição formal revisada e aprovada pelo responsável de negócio|Pendente|
|RN02|A apuração deve respeitar uma data de referência definida|Aplicar o período conforme o tipo de registro e a definição oficial do indicador|Regra de referência temporal documentada e exemplos conferidos|Pendente|
|RN03|Cancelamentos, ajustes e estornos devem seguir critérios explícitos|Definir como cada ocorrência afeta o resultado, considerando sua natureza e data de referência|Exemplos de registros, resultado esperado e decisão documentada|Pendente|
|RN04|Duplicidades não devem distorcer o indicador|Identificar a chave de negócio e distinguir duplicidades indevidas de registros legítimos com diferentes níveis de detalhe|Chave aprovada, amostra de dados e resultados dos testes de duplicidade|Pendente|
|RN05|Divergências devem possuir situação e histórico de tratamento|Registrar ocorrência, classificação, responsável, data, justificativa e encaminhamento|Registro de tratamento revisado e evidência de rastreabilidade|Pendente|
|RN06|Comparações devem utilizar critérios equivalentes|Garantir compatibilidade de fonte, período, filtros, unidade de medida e granularidade|Comparação documentada dos critérios aplicados em cada fonte|Pendente|
|RN07|Valores apresentados devem ser rastreáveis até sua origem|Permitir identificar os registros contribuintes e a origem do dado, conforme o nível de detalhe disponível|Consulta reproduzível que relacione resultado, registros e fonte|Pendente|
|RN08|Uma divergência não deve ser classificada como causa operacional sem investigação|Verificar qualidade dos dados e consistência das regras antes de concluir que existe desvio operacional real|Evidências da investigação e conclusão documentada|Pendente|
|RN09|Exceções devem seguir critérios formalmente definidos|Determinar quais situações permitem tratamento excepcional, quem pode aprová-las e como registrá-las|Critérios de exceção e aprovação do responsável competente|Pendente|
|RN010|Alterações nas regras devem ser rastreáveis|Registrar versão, data, responsável, justificativa e impacto das alterações relevantes|Histórico de alterações e comparação entre versões|Pendente|



## 3\. Tratamento de situações especiais

Os seguintes cenários exigem decisão do negócio antes da implementação das regras:

|Situação|Questão a resolver|Tratamento proposto para análise|
|-|-|-|
|Cancelamento|O registro deve ser excluído, compensado ou mantido no indicador?|Documentar o efeito conforme a natureza do indicador|
|Estorno|Qual data e qual valor devem ser considerados?|Definir o tratamento temporal e financeiro aplicável|
|Duplicidade|Os registros representam repetição indevida ou eventos distintos?|Investigar a chave de negócio e o nível de detalhe|
|Períodos divergentes|Qual data determina a competência do registro?|Aplicar a definição oficial após aprovação|
|Valores ausentes|O registro pode participar do cálculo?|Definir se bloqueia, fica pendente ou segue exceção autorizada|
|Resultado igual a zero|Como interpretar a variação percentual?|Definir tratamento para evitar divisão por zero e interpretações incorretas|
|Fontes divergentes|Qual fonte prevalece e sob quais condições?|Confirmar autoridade e finalidade de cada fonte|

Esses tratamentos são pontos de análise, não regras operacionais já aprovadas.



## 4\. Registro de decisão de negócio

O registro de decisão deverá documentar as alternativas avaliadas, os critérios considerados e a justificativa da escolha.

|ID|Decisão|Alternativas consideradas|Justificativa|Responsável|Data|Status|
|-|-|-|-|-|-|-|
|DEC-01|Definir a fonte oficial de referência do indicador|Fonte A; Fonte B; consolidação de ambas conforme regra aprovada|A definir após análise de confiabilidade, finalidade e governança das fontes|A identificar|A definir|Pendente|
|DEC-02|Definir a data de referência para apuração|Data do evento; data de lançamento; data de processamento|A definir conforme o significado do indicador e o processo de negócio|A identificar|A definir|Pendente|
|DEC-03|Definir o tratamento de cancelamentos e estornos|Exclusão; compensação; tratamento específico por tipo de ocorrência|A definir após análise de exemplos e impactos no resultado|A identificar|A definir|Pendente|
|DEC-04|Definir a chave para identificar duplicidades|Identificador do registro; chave composta; outro critério de negócio|A definir conforme a granularidade e a estrutura das fontes|A identificar|A definir|Pendente|
|DEC-05|Definir critérios para bloqueio ou liberação do indicador|Bloqueio; publicação com ressalva; liberação após aprovação de exceção| definir conforme criticidade e risco de decisão incorreta|A identificar|A definir|Pendente|

\*\*Importante:\*\* as alternativas são exemplos para orientar a discussão. A escolha não deve ocorrer antes da análise dos dados e da validação com os responsáveis.



## 5\. Processo de validação das regras

Para cada regra, seguir as etapas abaixo:

1\. \*\*Levantar:\*\* identificar a definição atual, as fontes e os exemplos relevantes.

2\. \*\*Analisar:\*\* avaliar impactos, exceções, riscos e possíveis interpretações.

3\. \*\*Propor:\*\* documentar a regra e os critérios de aplicação.

4\. \*\*Validar:\*\* apresentar a proposta ao responsável de negócio e registrar sua decisão.

5\. \*\*Testar:\*\* verificar o comportamento com cenários representativos e resultados esperados.

6\. \*\*Registrar:\*\* manter a regra, a decisão, a evidência e a versão correspondentes.

## 

## 6\. Critérios de aceite deste documento

O documento poderá ser considerado validado quando:

\- cada regra possuir identificação e descrição inequívocas;

\- as regras prioritárias estiverem relacionadas aos requisitos correspondentes;

\- as exceções relevantes estiverem documentadas;

\- os responsáveis pela aprovação estiverem identificados;

\- as decisões de negócio estiverem registradas;

\- os testes necessários para verificar a aplicação das regras estiverem definidos;

\- as pendências e os riscos remanescentes estiverem documentados.

A conclusão da documentação não equivale à aprovação das regras nem comprova sua execução técnica.



## 7\. Limitações e próximos passos

Este documento integra um estudo de caso simulado. As regras precisam ser confrontadas com as definições reais do indicador, a estrutura das fontes e as necessidades dos usuários antes de qualquer implementação.

O próximo passo é relacionar as regras aos requisitos funcionais e aos cenários de teste na matriz de rastreabilidade, garantindo que cada regra prioritária tenha uma forma objetiva de verificação.

