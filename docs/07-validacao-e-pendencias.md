# 07\. Validação e pendências

## 1\. Objetivo

Definir os critérios necessários para avaliar a conformidade da solução proposta, acompanhar a execução das validações e registrar pendências, riscos e decisões que possam afetar a confiabilidade dos indicadores.

Este documento estabelece critérios de aceite e indicadores candidatos para um cenário simulado. Sua aplicação depende da confirmação dos requisitos, da aprovação das regras de negócio e da execução das verificações previstas.



## 2\. Critérios para aceite da solução

A solução poderá ser submetida à aprovação quando os seguintes critérios tiverem sido atendidos ou formalmente tratados conforme o processo de validação acordado.

|ID|Critério|Evidência esperada|Status|
|-|-|-|-|
|AC01|Regras de negócio aprovadas pelos responsáveis competentes|Regras documentadas com responsável e registro de aprovação|Pendente|
|AC02|Requisitos prioritários associados a testes verificáveis|Matriz de rastreabilidade atualizada|Pendente|
|AC03|Testes aplicáveis executados e resultados registrados|Registro de execução e evidências correspondentes|Pendente|
|AC04|Divergências investigadas, corrigidas ou justificadas|Registro da ocorrência, análise, decisão e tratamento|Pendente|
|AC05|Resultados comparados com uma referência aprovada, sob critérios equivalentes|Memória de cálculo, parâmetros da comparação e fonte de referência|Pendente|
|AC06|Riscos residuais e pendências documentados|Lista de pendências, impactos, responsáveis e encaminhamentos|Pendente|
|AC07|Validação dos usuários registrada|Registro de validação, ressalvas e decisões dos responsáveis|Pendente|
|AC08|Documentação atualizada conforme a solução efetivamente validada|Requisitos, regras, fluxos, matriz e testes revisados|Pendente|

\*\*Condição de aceite:\*\* a aprovação deverá considerar o conjunto de evidências, os critérios acordados e os riscos remanescentes. Pendências que afetem a integridade do indicador ou impeçam a comprovação de requisitos críticos deverão ser avaliadas antes da autorização de uso.

A conclusão documental não substitui a execução dos testes nem a aprovação dos responsáveis.



## 3\. Indicadores propostos para acompanhamento

Os indicadores abaixo são candidatos para avaliar a qualidade da validação e o comportamento das divergências. As definições, a periodicidade, a população analisada e as metas deverão ser acordadas antes de sua utilização.



|Indicador|Definição e método de cálculo|Cuidados de interpretação|
|-|-|-|
|Taxa de divergências|(Número de comparações válidas com divergência ÷ total de comparações válidas) × 100|Definir previamente o que caracteriza uma comparação válida e uma divergência, inclusive a tolerância aplicável, se houver|
|Cobertura de testes|(Número de requisitos que exigem validação e possuem testes executados ÷ total de requisitos que exigem validação no escopo) × 100|Ter um teste documentado não significa que o requisito foi testado; acompanhar separadamente os requisitos bloqueados|
|Taxa de aprovação dos testes|(Número de testes aprovados ÷ total de testes executados com resultado conclusivo) × 100|Informar separadamente testes bloqueados e não executados; documentar o tratamento dos testes reprovados|
|Tempo de investigação|Tempo decorrido entre o registro da divergência e a conclusão documentada da investigação|Definir início, término, unidade de medida e tratamento de ocorrências suspensas ou reabertas|
|Cobertura de rastreabilidade|(Número de valores amostrados cuja origem foi identificada conforme o critério definido ÷ total de valores válidos amostrados) × 100|Definir a amostragem, a granularidade e o nível de rastreabilidade exigido|



\### Regras de utilização dos indicadores

\- \*\*Definir a população:\*\* especificar quais relatórios, períodos, registros ou requisitos fazem parte de cada cálculo.

\- \*\*Estabelecer uma referência:\*\* determinar a fonte oficial ou o critério aprovado para comparação.

\- \*\*Padronizar a coleta:\*\* registrar a origem dos dados, a data da medição e os filtros aplicados.

\- \*\*Medir antes de definir metas:\*\* estabelecer uma linha de base com dados válidos e representativos.

\- \*\*Interpretar em contexto:\*\* uma taxa menor de divergências, isoladamente, não comprova qualidade se houver comparações insuficientes ou critérios inadequados.

Os indicadores são propostas conceituais. Não há valores medidos, metas aprovadas ou resultados operacionais disponíveis neste estudo.



## 4\. Pendências e plano de validação

|ID|Pendência|Próxima ação|Evidência para encerramento|Status|
|-|-|-|-|-|
|PEN01|Processo atual e fontes ainda não confirmados|Levantar o fluxo real com os envolvidos|Fluxo revisado e validado|Pendente|
|PEN02|Regras de negócio aguardam aprovação|Validar fórmulas, períodos, exceções e critérios de inclusão|Regras aprovadas e decisões registradas|Pendente|
|PEN03|Fonte de referência não definida|Identificar e obter aprovação da fonte ou do método de reconciliação|Referência documentada e aprovada|Pendente|
|PEN04|Dados de teste não preparados|Definir conjuntos de dados, cenários e resultados esperados|Dados identificados e casos de teste completos|Pendente|
|PEN05|Testes ainda não executados|Executar os testes previstos e registrar os resultados|Registro de execução e evidências|Pendente|
|PEN06|Linha de base e metas não estabelecidas|Definir método de medição e coletar dados adequados|Linha de base documentada e metas acordadas|Pendente|
|PEN07|Critérios de aceite aguardam validação|Revisar os critérios com os responsáveis de negócio|Critérios aprovados e responsabilidades identificadas|Pendente|
|PEN08|Viabilidade técnica não avaliada|Analisar fontes, integrações, acessos, controles e esforço necessário|Avaliação técnica documentada|Pendente|



## 5\. Gestão de riscos e decisões

Durante a validação, deverão ser registrados os riscos que possam comprometer a confiabilidade dos resultados, incluindo:



\- Ausência de fonte de referência aprovada.

\- Regras de negócio conflitantes ou não documentadas.

\- Dados incompletos, desatualizados ou sem rastreabilidade suficiente.

\- Testes sem cobertura de cenários relevantes.

\- Divergências sem responsável ou justificativa documentada.

\- Limitações técnicas que impeçam a execução de controles necessários.

Para cada risco ou pendência relevante, registrar a descrição, o impacto potencial, a prioridade, o responsável pelo encaminhamento, a ação prevista e o status.

A classificação de prioridade e a decisão de aceitar um risco devem ser realizadas pelos responsáveis competentes, e não presumidas na documentação.



## 6\. Condições para encerramento da validação

O ciclo de validação poderá ser encerrado para o escopo acordado quando:



1\. Os critérios de aceite aplicáveis tiverem sido avaliados com evidências.

2\. Os testes executados estiverem registrados e seus resultados forem verificáveis.

3\. As divergências relevantes estiverem corrigidas, justificadas ou formalmente encaminhadas.

4\. Os riscos residuais e as limitações estiverem documentados e avaliados.

5\. Os usuários e responsáveis de negócio tiverem registrado sua avaliação.

6\. A documentação refletir o estado real da solução e as decisões tomadas.

O encerramento deverá indicar claramente o escopo validado, as evidências consideradas, as limitações existentes e as pendências que permanecerem abertas.



## 7\. Limitações do estudo

O cenário é simulado e tem finalidade demonstrativa. Não houve, neste estudo, confirmação de causas reais, execução dos testes descritos, implantação de solução ou medição de melhoria operacional.

Os critérios, indicadores e ações apresentados constituem uma proposta de trabalho e deverão ser confirmados com base em requisitos aprovados e evidências verificáveis.

Nenhum ganho, redução de divergências ou melhoria de desempenho deverá ser declarado sem medição e evidência correspondentes.



