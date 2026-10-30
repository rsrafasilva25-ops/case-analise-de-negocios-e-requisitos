# 01\. Contexto e declaração do problema

## 1.Status do documento

Estudo de caso simulado. As premissas apresentadas deverão ser verificadas em uma execução prática. Não há causas confirmadas nesta etapa.



## 2.Situação proposta

Uma área utiliza relatórios provenientes de diferentes fontes para acompanhar um indicador operacional. Em determinadas consultas, os valores apresentados divergem, mesmo quando o usuário seleciona aparentemente o mesmo período e os mesmos filtros.

A divergência exige uma investigação que permita distinguir inconsistências nos dados ou nos critérios de cálculo de possíveis variações reais do processo operacional.



## 3.Problema de negócio

Ausência de critérios suficientemente claros, padronizados e rastreáveis para consolidar, interpretar e validar as informações utilizadas no acompanhamento operacional.

Essa condição pode dificultar a comparação entre resultados, aumentar o esforço de conferência e reduzir a confiabilidade das informações utilizadas na tomada de decisão.



## 4.Objetivo

Investigar as possíveis causas das divergências, identificar as necessidades dos envolvidos, estabelecer critérios de negócio e especificar uma solução que permita reproduzir, explicar e validar os resultados apresentados.



## 5.Perguntas de investigação

* Quais relatórios, sistemas e fontes de dados estão envolvidos?
* Qual indicador apresenta divergência e quais decisões dependem dele?
* Quais filtros, datas de referência, níveis de detalhe e regras de cálculo cada fonte utiliza?
* Como cancelamentos, ajustes, estornos, duplicidades e registros incompletos são tratados?
* Existe uma fonte oficial de referência para o indicador? Quem responde por sua definição e aprovação?
* Qual é a diferença observada entre os resultados e em quais condições ela ocorre?
* Quais evidências são necessárias para confirmar ou descartar cada hipótese?
* Quais critérios devem ser atendidos antes de considerar o indicador validado?



## 6.Registro de evidências

|ID|Pergunta ou hipótese|Fonte prevista para consulta|Evidência necessária|Conclusão|Status|
|-|-|-|-|-|-|
|INV-01|Quais fontes geram os resultados divergentes?|Relatórios e responsáveis pelas fontes|Identificação das fontes, período de atualização e critérios utilizados|A preencher após consulta|Pendente|
|INV-02|Os relatórios utilizam o mesmo período de referência?|Filtros dos relatórios e documentação das fontes|Datas, calendário e regra de definição do período|A preencher após comparação|Pendente|
|INV-03|As regras de cálculo são equivalentes?|Fórmulas, consultas e documentação do indicador|Comparação das fórmulas, filtros e tratamentos aplicados|A preencher após análise|Pendente|
|INV-04|Existem registros duplicados ou incompletos?|Dados de origem e regras de qualidade|Registros identificados e critérios de validação aplicados|A preencher após teste|Pendente|
|INV-05|Qual referência deve prevalecer?|Responsável pelo indicador e documentação de negócio|Definição aprovada da fonte e da regra oficial|A preencher após validação com o responsável|Pendente|

Observação: as fontes indicadas são propostas para a investigação. Sua disponibilidade e adequação ainda precisam ser confirmadas.



## 7.Distinção entre hipótese e conclusão

Uma hipótese representa uma explicação possível para a divergência. Ela somente deverá ser registrada como causa confirmada quando houver evidência verificável, critério de análise definido e resultado reproduzível.

Quando não houver evidências suficientes, a conclusão deverá permanecer como inconclusiva ou pendente, com indicação das informações necessárias para avançar.



## 8.Resultado esperado desta etapa

Produzir uma definição clara do problema, delimitar o escopo da investigação, identificar as fontes e os responsáveis envolvidos e estabelecer uma base verificável para o levantamento de requisitos e a análise das causas.

