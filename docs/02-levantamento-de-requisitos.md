# 02\. Levantamento de requisitos

## 1.Objetivo

Identificar e documentar as necessidades dos envolvidos, convertendo-as em requisitos claros, verificáveis, priorizáveis e rastreáveis. Os requisitos deverão orientar a especificação da solução, a definição dos critérios de aceitação e o planejamento dos testes.

\*\*Status:\*\* proposta inicial, sujeita à validação com os stakeholders e à confirmação das regras oficiais do indicador.

## 

## 2.Stakeholders a identificar

|Stakeholder|Necessidade ou responsabilidade|
|-|-|
|Usuários dos indicadores|Consultar resultados consistentes, compreender divergências e apoiar decisões|
|Responsável de negócio pelo indicador|Definir o significado, as regras, as exceções e os critérios de aprovação|
|Responsável pelos dados de origem|Esclarecer a origem, a estrutura, a atualização e as limitações dos dados|
|Equipe técnica ou de integração|Avaliar fontes, dependências, viabilidade técnica e mecanismos de rastreabilidade|
|Responsável por segurança e acessos|Definir permissões para consulta e acesso aos detalhes dos registros, quando aplicável|

A identificação dos responsáveis nominais, suas atribuições formais e sua disponibilidade deverá ocorrer durante o levantamento.

## 

## 3.Perguntas de elicitação

##### \### Necessidade e contexto de negócio

\- Qual decisão operacional ou gerencial o indicador apoia?

\- Qual problema ocorre atualmente e como ele afeta o processo?

\- Quem utiliza o resultado e qual é o impacto de uma informação incorreta?

\- Qual resultado esperado caracterizaria uma solução adequada?

##### \### Dados e regras

\- Qual é a definição oficial do indicador?

\- Quais fontes, períodos, filtros e dimensões devem ser considerados?

\- Qual é a granularidade mínima necessária para comparação?

\- Como são tratados cancelamentos, ajustes, estornos e duplicidades?

\- Existe uma fonte de referência aprovada? Quem valida sua utilização?

##### \### Tratamento de divergências

\- Quais tipos de inconsistência precisam ser identificados?

\- O que deve acontecer quando os valores divergirem?

\- Quais situações bloqueiam a validação e quais admitem exceção?

\- Quem será responsável por investigar, corrigir e aprovar cada ocorrência?

\- Quais evidências devem ser registradas para concluir a investigação?

##### \### Uso, segurança e aceitação

\- Quais usuários poderão consultar os dados detalhados?

\- Qual frequência de atualização e tempo de resposta são necessários?

\- Como será demonstrado que os resultados estão corretos?

\- Quem aprovará os critérios de aceite e a conclusão dos testes?



## 4.Necessidades de negócio identificadas no cenário

|ID|Necessidade|Resultado esperado|
|-|-|-|
|NB01|Compreender a origem das divergências|Possibilidade de investigar e documentar causas com evidências|
|NB02|Comparar resultados de maneira consistente|Aplicação de períodos, filtros e regras aprovados|
|NB03|Rastrear os valores apresentados|Identificação dos registros de origem que compõem o resultado|
|NB04|Controlar o tratamento das inconsistências|Registro de situação, responsável, justificativa e encaminhamento|
|NB05|Apoiar decisões com informações verificáveis|Disponibilização de resultados acompanhados de status de validação|

As necessidades acima foram derivadas do cenário proposto e deverão ser confirmadas com os stakeholders.



## 5.Requisitos funcionais propostos

|ID|Requisito|Prioridade|Critério de aceitação|Status|
|-|-|-|-|-|
|RF01|Permitir a consulta do indicador por período e dimensões aprovadas|Alta|Para uma massa de teste conhecida, os filtros retornam os registros correspondentes e respeitam o período selecionado|Proposto|
|RF02|Identificar divergências em relação à fonte de referência aprovada|Alta|Dada uma divergência reproduzível, o sistema sinaliza a diferença e permite identificar os valores comparados|Proposto|
|RF03|Permitir rastrear os valores até os registros de origem|Alta|Para um resultado consultado, é possível localizar os registros contribuintes e a fonte correspondente, conforme as permissões definidas|Proposto|
|RF04|Registrar o tratamento das inconsistências|Alta|Cada ocorrência tratada possui situação, responsável, data e justificativa; campos obrigatórios são validados|Proposto|
|RF05|Disponibilizar detalhes para investigação|Média|Usuário autorizado consegue consultar os campos necessários para analisar a divergência, respeitando as regras de acesso|Proposto|
|RF06|Exibir o status de validação do indicador|Alta|O resultado diferencia estados como pendente, validado e bloqueado, conforme critérios aprovados|Proposto|
|RF07|Registrar alterações relevantes no tratamento das ocorrências|Média|Alterações de status e justificativas mantêm histórico de autor, data e informação alterada|Proposto|

\### Observações sobre priorização

As prioridades são preliminares. A classificação definitiva deverá considerar impacto no negócio, risco de decisão incorreta, dependências técnicas, esforço e urgência operacional.



## 6.Requisitos não funcionais propostos

|ID|Requisito|Critério de verificação|Status|
|-|-|-|-|
|RNF01|Rastreabilidade|Resultados e ocorrências podem ser relacionados à fonte, ao período e à execução correspondente|Proposto|
|RNF02|Integridade|Validações identificam campos obrigatórios ausentes e inconsistências previstas nas regras aprovadas|Proposto|
|RNF03|Segurança e controle de acesso|Consultas e detalhes respeitam os perfis e as permissões definidos|Proposto|
|RNF04|Auditabilidade|Alterações relevantes possuem histórico consultável por usuários autorizados|Proposto|
|RNF05|Desempenho|O tempo de resposta atende ao limite que será acordado com os usuários para o volume previsto|A definir|
|RNF06|Usabilidade|Usuários representativos conseguem identificar o resultado, seu status e as divergências sem ambiguidade nos testes de aceitação|Proposto|

Os limites quantitativos de desempenho, os perfis de acesso e os critérios de usabilidade precisam ser definidos antes da aprovação final.



## 7.Restrições, dependências e decisões pendentes



|ID|Item|Ação necessária|
|-|-|-|
|DP01|Fonte oficial de referência|Confirmar a fonte e o responsável pela aprovação|
|DP02|Definição do indicador|Documentar fórmula, filtros, período e granularidade|
|DP03|Tratamento de exceções|Definir situações bloqueantes e exceções autorizadas|
|DP04|Acesso aos dados|Confirmar perfis, campos sensíveis e permissões|
|DP05|Desempenho esperado|Estabelecer volume de dados, frequência e tempo máximo de resposta|
|DP06|Aceite da solução|Identificar responsáveis pela execução e aprovação dos testes|



## 8.Rastreabilidade e próximos passos

Os requisitos deverão ser relacionados às necessidades de negócio, às regras de negócio e aos casos de teste por meio da matriz de rastreabilidade.

Antes de estabelecer uma baseline aprovada, será necessário:



1\. Confirmar as necessidades com os stakeholders.

2\. Resolver ou registrar as decisões pendentes.

3\. Revisar prioridade, escopo e dependências.

4\. Aprovar os requisitos e seus critérios de aceitação.

5\. Relacionar cada requisito prioritário a pelo menos um teste verificável.



\*\*Limitação:\*\* os requisitos e critérios apresentados constituem uma especificação inicial para um estudo de caso simulado. Não há evidência de aprovação por usuários, implementação ou execução dos testes.

