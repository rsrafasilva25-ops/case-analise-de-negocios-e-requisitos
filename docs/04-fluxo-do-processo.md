# 04\. Fluxo do processo AS-IS TO-BE

## 1\. Objetivo

Representar o fluxo de tratamento dos dados e de investigação das divergências entre indicadores, identificando etapas, participantes, entradas, saídas, controles e pontos que precisam ser confirmados.

O mapeamento tem como objetivo apoiar a compreensão do processo atual, identificar possíveis lacunas de controle e estruturar uma proposta de processo futuro com critérios definidos e rastreabilidade.



## 2\. Status do mapeamento

\*\*AS-IS:\*\* fluxo hipotético inicial, pendente de levantamento e validação com os usuários e responsáveis pelo processo.

\*\*TO-BE:\*\* fluxo futuro proposto, sujeito à validação das regras de negócio, dos requisitos, da viabilidade técnica e dos critérios de aceite.

Os fluxos apresentados não representam um processo real já mapeado, implantado ou validado.



## 3\. Fluxo atual hipotético — AS-IS

#### Etapas identificadas como hipótese de trabalho

1\. \*\*Recebimento dos dados:\*\* informações provenientes de sistemas, relatórios ou arquivos.

2\. \*\*Tratamento e consolidação:\*\* aplicação de filtros, ajustes e transformações para preparação dos dados.

3\. \*\*Geração dos indicadores:\*\* apresentação dos resultados em relatórios ou ferramentas de análise.

4\. \*\*Identificação da divergência:\*\* usuário identifica resultados diferentes entre relatórios ou fontes.

5\. \*\*Investigação e conferência:\*\* equipe verifica informações, critérios de cálculo, períodos, filtros e registros envolvidos.

6\. \*\*Tratamento da ocorrência:\*\* divergência é corrigida, justificada ou encaminhada para análise adicional.

7\. \*\*Disponibilização do resultado:\*\* resultado tratado é utilizado pelo usuário, conforme o procedimento existente, ainda a confirmar.

#### Representação simplificada

\*\*Fontes de dados → Tratamento e consolidação → Relatórios e indicadores → Identificação da divergência → Investigação → Correção ou justificativa → Utilização do resultado\*\*

O fluxo deverá ser ajustado após a confirmação das etapas efetivamente realizadas, incluindo possíveis retornos para correção e reprocessamento.



## 4\. Pontos de investigação do AS-IS



|Dimensão|O que investigar|Evidência esperada|
|-|-|-|
|Entradas e saídas|Quais dados entram e quais resultados são gerados em cada etapa?|Arquivos, relatórios, consultas ou documentação|
|Sistemas e fontes|Quais sistemas, tabelas, arquivos e relatórios participam do processo?|Identificação das fontes e responsáveis|
|Responsabilidades|Quem executa, valida, aprova e utiliza cada etapa?|Confirmação dos papéis envolvidos|
|Transformações|Quais filtros, cálculos, junções e tratamentos são aplicados?|Consultas, fórmulas, especificações ou exemplos reproduzíveis|
|Regras de negócio|Como são tratados períodos, cancelamentos, estornos, duplicidades e exceções?|Regras documentadas e validação do responsável de negócio|
|Atividades manuais|Existem ajustes em planilhas, correções manuais ou conferências paralelas?|Procedimentos, registros e exemplos|
|Controles|Quais verificações identificam dados incompletos, inconsistentes ou duplicados?|Evidências dos controles e respectivos resultados|
|Tratamento de divergências|Como a ocorrência é registrada, investigada, corrigida e encerrada?|Histórico, responsáveis, justificativas e critérios de encerramento|
|Disponibilização|Quem autoriza o uso do indicador e em quais condições?| Critérios de validação e aprovação|

\*\*Resultado esperado do levantamento:\*\* obter evidências suficientes para descrever o processo real, identificar lacunas e distinguir causas confirmadas de hipóteses ainda não verificadas.

### 

### 5\. Fluxo futuro proposto — TO-BE

#### Etapas propostas

1\. \*\*Receber os dados:\*\* identificar as fontes, o período de referência e a versão dos dados utilizados.

2\. \*\*Validar a entrada:\*\* verificar estrutura, preenchimento, integridade e condições mínimas para processamento.

3\. \*\*Aplicar regras aprovadas:\*\* executar os tratamentos e cálculos conforme definições validadas pelos responsáveis de negócio.

4\. \*\*Consolidar o indicador:\*\* calcular os resultados com critérios consistentes e possibilidade de rastreamento até os registros de origem.

5\. \*\*Executar verificações:\*\* avaliar consistência, reconciliação, duplicidades relevantes e demais controles definidos para o indicador.

6\. \*\*Identificar divergências:\*\* comparar os resultados sob condições equivalentes de período, filtros, escopo e regras.

7\. \*\*Registrar a ocorrência:\*\* documentar a diferença encontrada, as fontes envolvidas, as evidências disponíveis, o responsável e o status.

8\. \*\*Investigar e tratar:\*\* analisar a causa com base em evidências e encaminhar a correção, a justificativa ou a necessidade de decisão de negócio.

9\. \*\*Revalidar o resultado:\*\* executar novamente os controles aplicáveis e verificar se o tratamento resolveu a ocorrência sem introduzir novas inconsistências.

10\. \*\*Autorizar a disponibilização:\*\* liberar o resultado conforme critérios de aceite e responsabilidades previamente definidos.

11\. \*\*Manter o histórico:\*\* preservar as evidências, decisões, alterações e justificativas necessárias à auditoria e à análise posterior.



#### Representação simplificada

\*\*Recebimento → Validação dos dados → Aplicação das regras aprovadas → Consolidação → Testes de consistência → Comparação dos indicadores → Registro e investigação das divergências → Tratamento → Revalidação → Disponibilização autorizada\*\*

\*\*Ponto de decisão:\*\* se a validação identificar uma inconsistência, o resultado deverá seguir o tratamento definido para aquela situação. A possibilidade de bloquear ou liberar parcialmente a disponibilização precisa ser acordada com o responsável de negócio.



## 6\. Controles propostos para o processo futuro

|Controle|Objetivo|Evidência esperada|
|-|-|-|
|Validação de entrada|Identificar dados ausentes ou fora do padrão esperado|Resultado das verificações|
|Consistência de cálculo|Confirmar aplicação das regras aprovadas|Memória de cálculo ou resultado reproduzível|
|Reconciliação|Explicar diferenças entre valores e fontes comparáveis|Comparativo com critérios e valores de referência|
|Rastreabilidade|Relacionar o indicador aos registros que contribuíram para o resultado|Identificadores dos registros e origem dos dados|
|Gestão de ocorrências|Evitar divergências sem responsável ou tratamento documentado|Registro com status, responsável e evidências|
|Revalidação|Confirmar o resultado após uma correção ou ajuste|Evidência do teste executado|
|Histórico de alterações|Permitir compreender o que mudou e por quê|Registro de alteração, data, responsável e justificativa|

Os controles são propostas iniciais. Sua implementação, abrangência e forma de execução dependem dos requisitos aprovados e da análise de viabilidade.



## 7\. Decisões e pontos pendentes

|ID|Questão pendente|Responsável a confirmar|Status|
|-|-|-|-|
|PROC-01|Quais fontes e etapas compõem o processo atual?|Responsável pelo processo|Pendente|
|PROC-02|Quem é responsável pela definição e aprovação do indicador?|Área de negócio|Pendente|
|PROC-03|Quais verificações devem ser executadas antes da comparação?|Negócio e equipe técnica|Pendente|
|PROC-04|Quais divergências impedem a disponibilização do resultado?|Responsável de negócio|Pendente|
|PROC-05|Como registrar, priorizar e encerrar as ocorrências?|Responsáveis pelo tratamento|Pendente|
|PROC-06|Quais evidências devem ser preservadas para auditoria?|Negócio e áreas envolvidas|Pendente|
|PROC-07|Quais etapas podem ser automatizadas e quais dependem de análise humana?|Negócio e equipe técnica|Pendente|



## 8\. Critérios de validação do fluxo

O mapeamento poderá ser considerado validado quando:

\- As etapas do processo atual forem confirmadas com os envolvidos.

\- As entradas, saídas, sistemas e responsabilidades estiverem identificados.

\- As regras e transformações relevantes tiverem origem e responsáveis definidos.

\- Os pontos de controle e as atividades manuais estiverem documentados.

\- O fluxo futuro estiver alinhado aos requisitos e às regras de negócio aprovados.

\- Os critérios de tratamento, revalidação e disponibilização estiverem definidos.

\- Os pontos pendentes, riscos e decisões estiverem registrados.



## 9\. Limitações e próximos passos

O AS-IS ainda não foi confirmado por entrevistas, observação do processo ou análise de evidências reais. O TO-BE representa uma proposta conceitual, não uma solução implementada ou testada.

A próxima etapa é validar o processo atual com os envolvidos, confrontar as hipóteses com evidências e ajustar o fluxo futuro de acordo com os requisitos e as regras aprovados.

O fluxo validado deverá ser relacionado à matriz de rastreabilidade e ao plano de testes, permitindo conectar etapas do processo, requisitos, controles e evidências de validação.



