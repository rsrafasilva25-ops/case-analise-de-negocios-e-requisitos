# 06\. Plano de testes

## 1\. Objetivo

Definir os testes necessários para verificar os requisitos funcionais, as regras de negócio e os controles propostos para a investigação de divergências entre indicadores.

O plano estabelece os cenários, as pré-condições, os procedimentos, os resultados esperados e as evidências necessárias para demonstrar a conformidade com os critérios de aceite.



## 2\. Status e premissas

Este plano foi elaborado para um caso simulado de Análise de Negócios. Os testes estão documentados, mas \*\*nenhum teste foi executado ou aprovado neste estudo\*\*.

A execução depende da definição e aprovação das regras de negócio, da identificação dos dados de teste e da disponibilidade do ambiente e dos recursos necessários.

Os dados numéricos apresentados são fictícios e servem exclusivamente para demonstrar a estrutura de validação.



## 3\. Casos de teste

#### CT01 — Conferência do total consolidado

\*\*Objetivo:\*\* verificar se o total calculado corresponde à soma dos registros válidos do conjunto de teste.

\*\*Requisito relacionado:\*\* RF01 — Consulta do indicador por período e dimensões.

\*\*Regra relacionada:\*\* RN01 — Definição e fórmula do indicador.



\*\*Pré-condições:\*\*

\- A fórmula aplicável foi aprovada pelo responsável de negócio.

\- O conjunto de teste e o período de referência estão definidos.

\- Os registros válidos para o cálculo foram identificados.

\- Os valores e a regra de inclusão dos registros estão documentados.



\*\*Dados fictícios de entrada:\*\*

|Registro|Valor|
|-|-|
|A|R$ 100,00|
|B|R$ 200,00|
|C|R$ 150,00|
|\*\*Total esperado\*\*|\*\*R$ 450,00\*\*|



\*\*Procedimento:\*\*

1\. Consultar os registros do conjunto de teste.

2\. Confirmar quais registros devem compor o cálculo.

3\. Aplicar a fórmula aprovada.

4\. Comparar o total calculado com o valor esperado.

5\. Registrar o resultado obtido e a evidência correspondente.



\*\*Resultado esperado:\*\* o total calculado é de R$ 450,00 para os três registros válidos do conjunto de teste.

\*\*Critério de aceite:\*\* o valor calculado corresponde a R$ 450,00, respeitando os critérios de inclusão e a fórmula previamente aprovados.

\*\*Evidência prevista:\*\* memória de cálculo, consulta executada ou relatório de validação que permita reproduzir o resultado.

\*\*Status:\*\* A executar.



#### CT02 — Tratamento de registros duplicados

\*\*Objetivo:\*\* verificar se registros que representam o mesmo evento de negócio são tratados conforme a chave de identificação e a regra aprovada.

\*\*Requisitos relacionados:\*\* RF01 e RF02.

\*\*Regra relacionada:\*\* RN04 — Tratamento de duplicidades.



\*\*Pré-condições:\*\*

\- A granularidade do indicador está definida.

\- A chave de negócio e os critérios de identificação de duplicidade foram aprovados.

\- O conjunto de teste contém registros identificados como duplicados e, quando aplicável, registros semelhantes que representam eventos distintos.



\*\*Procedimento:\*\*

1\. Consultar os registros do conjunto de teste.

2\. Aplicar os critérios aprovados de identificação de duplicidade.

3\. Verificar quais registros representam o mesmo evento e quais representam eventos legítimos distintos.

4\. Recalcular o indicador conforme a regra definida.

5\. Registrar os registros identificados e o resultado obtido.



\*\*Resultado esperado:\*\* os registros classificados como duplicados conforme a regra aprovada não provocam contagem indevida; eventos distintos são preservados.

\*\*Critério de aceite:\*\* o resultado respeita a granularidade e a chave de negócio aprovadas.

\*\*Evidência prevista:\*\* relação dos registros avaliados, identificação dos duplicados e memória do cálculo.

\*\*Status:\*\* A executar.



#### CT03 — Tratamento de cancelamentos e reversões

\*\*Objetivo:\*\* verificar se cancelamentos, estornos ou reversões são considerados de acordo com as regras de negócio aprovadas.

\*\*Requisitos relacionados:\*\* RF01 e RF02.

\*\*Regras relacionadas:\*\* RN03 e RN09.



\*\*Pré-condições:\*\*

\- O tratamento aplicável a cada tipo de evento está documentado.

\- Os dados de teste contêm exemplos representativos dos eventos previstos.



\*\*Procedimento:\*\*

1\. Identificar os registros de cancelamento, estorno ou reversão.

2\. Consultar a regra aplicável a cada situação.

3\. Recalcular o indicador conforme a regra aprovada.

4\. Comparar o resultado com o valor esperado.

5\. Registrar eventuais diferenças.



\*\*Resultado esperado:\*\* cada evento recebe o tratamento definido para seu tipo, sem exclusões ou inclusões baseadas em suposições.

\*\*Critério de aceite:\*\* o resultado está de acordo com as regras aprovadas para os eventos testados.

\*\*Evidência prevista:\*\* registros de entrada, regra aplicada, cálculo e resultado da comparação.

\*\*Status:\*\* A executar.



#### CT04 — Respeito ao período de referência

\*\*Objetivo:\*\* verificar se os registros são incluídos no indicador conforme a data de referência e o período definidos.

\*\*Requisitos relacionados:\*\* RF01 e RF02.

\*\*Regras relacionadas:\*\* RN02 e RN06.



\*\*Pré-condições:\*\*

\- A data de referência do indicador está definida.

\- Os limites do período de análise estão documentados.

\- O conjunto de teste contém registros em datas internas e externas ao período.



\*\*Procedimento:\*\*

1\. Identificar a data de referência aplicável a cada registro.

2\. Definir o período de consulta.

3\. Executar o cálculo para o período selecionado.

4\. Verificar a inclusão dos registros dentro do período e o tratamento dos registros externos.

5\. Comparar o resultado com o esperado.



\*\*Resultado esperado:\*\* os registros são considerados conforme a data de referência e os limites do período aprovados.

\*\*Critério de aceite:\*\* nenhum registro é incluído ou excluído em desacordo com a regra temporal definida.

\*\*Evidência prevista:\*\* parâmetros da consulta, registros avaliados e memória de cálculo.

\*\*Status:\*\* A executar.



#### CT05 — Rastreabilidade do indicador até a origem

\*\*Objetivo:\*\* verificar se é possível identificar os registros de origem que contribuíram para o valor consolidado.

\*\*Requisito relacionado:\*\* RF03 — Rastreabilidade dos registros.

\*\*Regra relacionada:\*\* RN07 — Rastreabilidade até a origem.



\*\*Pré-condições:\*\*

\- O conjunto de teste está identificado.

\- Os registros possuem identificadores que permitem relacionar a origem ao resultado.

\- A granularidade e o nível de detalhamento esperado estão definidos.



\*\*Procedimento:\*\*

1\. Selecionar um valor do indicador.

2\. Consultar os registros que contribuíram para esse valor.

3\. Relacionar os registros às respectivas fontes.

4\. Reproduzir o cálculo a partir dos registros identificados.

5\. Registrar eventuais lacunas de rastreabilidade.



\*\*Resultado esperado:\*\* os registros de origem pertinentes são localizados e relacionados ao valor analisado, respeitando o nível de detalhe definido.

\*\*Critério de aceite:\*\* o valor pode ser reconciliado com os registros identificados, ou as limitações de rastreabilidade são explicitamente registradas.

\*\*Evidência prevista:\*\* relação dos registros, identificação das fontes e memória de cálculo.

\*\*Status:\*\* A executar.



#### CT06 — Identificação de falha ou atraso de atualização

\*\*Objetivo:\*\* verificar se a solução identifica ou sinaliza dados que não atendem ao critério de atualização definido.

\*\*Requisitos relacionados:\*\* RF02 e RF06.

\*\*Regras relacionadas:\*\* RN05 e RN08.



\*\*Pré-condições:\*\*

\- A frequência ou o prazo esperado de atualização está definido.

\- Existe um critério para identificar dados desatualizados.

\- O conjunto de teste contém uma situação de atualização dentro do prazo e outra fora do limite estabelecido.



\*\*Procedimento:\*\*

1\. Consultar a data ou o horário de atualização disponível.

2\. Comparar a atualização observada com o limite aprovado.

3\. Verificar a sinalização da condição de atraso.

4\. Registrar o resultado e a evidência.



\*\*Resultado esperado:\*\* a condição que ultrapassa o limite definido é identificada conforme o critério aprovado.

\*\*Critério de aceite:\*\* a sinalização corresponde aos parâmetros de atualização definidos e não classifica como desatualizados dados que atendam ao critério.

\*\*Evidência prevista:\*\* registro da atualização, parâmetro de referência e resultado da verificação.

\*\*Status:\*\* A executar.



## 4\. Registro de execução dos testes

O registro abaixo deverá ser preenchido somente após a execução de cada caso.

|ID|Dados utilizados|Resultado esperado|Resultado obtido|Evidência|Status|
|-|-|-|-|-|-|
|CT01|Conjunto fictício A, B e C|R$ 450,00|Não executado|A registrar|A executar|
|CT02|A definir|Conforme regra de duplicidade aprovada|Não executado|A registrar|A executar|
|CT03|A definir|Conforme regra de cancelamentos e reversões aprovada|Não executado|A registrar|A executar|
|CT04|A definir|Conforme período de referência aprovado|Não executado|A registrar|A executar|
|CT05|A definir|Registros de origem identificáveis|Não executado|A registrar|A executar|
|CT06|A definir|Condição de atualização identificada conforme critério|Não executado|A registrar|A executar|



## 5\. Critérios de gestão dos resultados

Cada teste deverá receber um status coerente com a execução:



\- \*\*A executar:\*\* teste documentado, ainda não executado.

\- \*\*Aprovado:\*\* resultado obtido atende ao critério de aceite, com evidência registrada.

\- \*\*Reprovado:\*\* resultado obtido não atende ao critério de aceite.

\- \*\*Bloqueado:\*\* não foi possível executar o teste por falta de dados, ambiente, regra aprovada ou outra dependência identificada.

\- \*\*Não aplicável:\*\* cenário não se aplica ao escopo, mediante justificativa documentada e aprovação pertinente.



Quando houver reprovação, registrar a diferença observada, as evidências, o impacto, o responsável pelo encaminhamento e a necessidade de correção ou revisão do requisito.

Após a correção, o teste deverá ser reexecutado e, quando necessário, deverão ser avaliados testes de regressão para verificar possíveis impactos em outras regras ou resultados.



## 6\. Critérios gerais de conclusão

A validação será considerada concluída para o escopo definido quando:



\- Os testes aplicáveis tiverem sido executados.

\- Os resultados obtidos estiverem registrados e comparados com os critérios de aceite.

\- As evidências forem suficientes para reproduzir ou verificar os resultados.

\- As reprovações e os bloqueios estiverem documentados e tratados conforme os critérios aprovados.

\- As limitações e os riscos remanescentes estiverem registrados.

\- Os responsáveis de negócio tiverem avaliado os resultados e as condições de aceite.

A documentação do plano, por si só, não comprova que os requisitos foram atendidos ou que o indicador está correto.



## 7\. Limitações e próximos passos

Os testes descritos são propostas para um caso simulado. Os dados, as regras e os critérios deverão ser confirmados antes da execução.

O próximo passo é revisar os cenários com os requisitos e as regras de negócio, completar os dados de teste e preparar o registro de execução. Somente após a execução deverão ser documentados os resultados obtidos, as evidências e as conclusões de validação.



