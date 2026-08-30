\# 📊 Miniguia de Estudos: Matemática Financeira Aplicada ao Financiamento Imobiliário (SAC vs. PRICE e CET)



> \*\*Autor:\*\* José Alexandre  

> \*\*Perfil:\*\* Contador (Graduação, Pós-graduado em Perícia Contábil e Controladoria), Assistente Administrativo e Especialista em Rotinas Fiscais e Contábeis.  

> \*\*Projeto:\*\* Desafio Prático DIO — Aprendizagem Ativa e Curadoria do Conhecimento com NotebookLM  



\---



\## 🎯 1. Contexto e Objetivos



\### Contexto

A aquisição da casa própria por meio de empréstimo/financiamento bancário de longo prazo é uma das decisões financeiras mais complexas para famílias e empresas. Compreender a mecânica por trás das tabelas de amortização, a incidência de juros compostos, a correção monetária e o impacto do Custo Efetivo Total (CET) é fundamental para a análise financeira rigorosa e a perícia contábil de contratos bancários.



\### Objetivos de Estudo

\- Comparar os métodos de amortização \*\*SAC (Sistema de Amortização Constante)\*\* e \*\*Tabela Price (Sistema Francês de Amortização)\*\* em cenários de crédito imobiliário de longo prazo.

\- Entender a composição do \*\*Custo Efetivo Total (CET)\*\*, incluindo taxa de juros nominal/efetiva, seguros obrigatórios (MIP e DFI) e tarifas administrativas.

\- Utilizar o \*\*NotebookLM\*\* como ferramenta de aprendizagem ativa para auditar fórmulas, analisar normativas do Banco Central do Brasil (BACEN) e apoiar simulações financeiras.



\---



\## 📚 2. Curadoria de Fontes



Para alimentar o caderno temático no NotebookLM, foram selecionadas 4 fontes oficiais e abertas (normativas do BACEN, cartilhas técnicas e literatura de matemática financeira):



1\. \*\*\[Resolução CMN nº 4.881/2020 (Banco Central do Brasil - BACEN)](https://www.bcb.gov.br/estabilidadefinanceira/exibenormativo?tipo=Resolu%C3%A7%C3%A3o%20CMN\&numero=4881)\*\*

&#x20;  - \*Descrição:\* Regulamentação oficial do Conselho Monetário Nacional sobre a obrigatoriedade, transparência e fórmula de cálculo do Custo Efetivo Total (CET).

2\. \*\*\[Cartilha de Habitação PF - CAIXA / BACEN (PDF)](https://www.caixa.gov.br/Downloads/habitacao-documentos-gerais/cartilha-habitacao-PF-construcao-conclusao-reforma-ampliacao-de-unidades-habitacionais.pdf)\*\*

&#x20;  - \*Descrição:\* Guia explicativo das regras do crédito habitacional, cobrindo exigências de enquadramento (SFH/SFI) e custos adicionais com seguros obrigatórios (MIP e DFI).

3\. \*\*\[Artigo Técnico: Price ou SAC, qual é melhor? - REMAT/IFRS (PDF)](https://periodicos.ifrs.edu.br/index.php/REMAT/article/download/7647/3964/36730)\*\*

&#x20;  - \*Descrição:\* Estudo acadêmico do Instituto Federal do Rio Grande do Sul que deduz as equações matemáticas das tabelas Price e SAC, analisando anatocismo e evolução do saldo devedor.

4\. \*\*\[Instrução Normativa BCB nº 83/2021 - Exemplo de Planilha de CET](https://www.bcb.gov.br/estabilidadefinanceira/exibenormativo?tipo=Instru%C3%A7%C3%A3o%20Normativa%20BCB\&numero=83)\*\*

&#x20;  - \*Descrição:\* Regulamento do BACEN que estabelece o formato padrão e a memória de cálculo para a demonstração do CET nas propostas de financiamento.



\---



\## 🧪 3. Engenharia de Prompts e "Cicatrizes" (Troubleshooting)



\### Testes de Prompts Efetuados no NotebookLM:



\#### Teste 1: Comparação Conceitual vs. Análise Analítica do Saldo Devedor

\- \*\*Prompt Inicial (Genérico):\*\* \*"Qual a diferença entre a Tabela Price e o Sistema SAC no financiamento da casa própria?"\*

&#x20; - \*\*Resultado:\*\* A IA apresentou apenas a diferença básica (Price tem parcelas fixas; SAC tem parcelas decrescentes), sem abordar a taxa de amortização e omitindo os seguros obrigatórios do CET.

\- \*\*Prompt Refinado (Técnico):\*\* \*"Com base nas fontes fornecidas, explique analiticamente por que o Sistema SAC amortiza o saldo devedor mais rapidamente nos primeiros 5 anos do que a Tabela Price para um mesmo valor financiado. Explique também como o Custo Efetivo Total (CET) difere da taxa nominal ao incluir as tarifas e seguros obrigatórios (MIP e DFI)."\*

&#x20; - \*\*Resultado:\*\* A resposta foi altamente precisa: detalhou que na Price as primeiras prestações são compostas majoritariamente por juros, enquanto no SAC a cota de amortização principal ($A = SD\_0 / n$) é constante desde a primeira parcela, reduzindo a base de cálculo dos juros futuros de forma acelerada.



\### Troubleshooting e Lições Aprendidas ("Cicatrizes")

\- \*\*Desafio Encontrado:\*\* O NotebookLM inicialmente tendeu a tratar a \*Taxa de Juros Nominal\* como equivalente ao \*Custo Efetivo Total (CET)\* ao responder sobre o custo real da operação para o mutuário.

\- \*\*Solução:\*\* Incluir a seguinte diretriz de calibração no prompt: \*"Diferencie estritamente a taxa de juros nominal contratada do CET, destacando que o CET engloba IOF, tarifas administrativas e prêmios de seguro habitacional vinculados ao contrato."\*



\---



\## 📖 4. Miniguia de Estudo (Entrega Final)



\### 4.1. Resumos Estruturados do Assunto



\#### A. Comparativo Metodológico: SAC vs. PRICE

| Característica | Sistema SAC | Tabela Price (Sistema Francês) |

| :--- | :--- | :--- |

| \*\*Prestação ($PMT$)\*\* | Decrescente ao longo do tempo. | Constante (em termos nominais). |

| \*\*Amortização ($A$)\*\* | \*\*Constante\*\* ($A = \\frac{SD\_0}{n}$). | Crescente a cada período. |

| \*\*Juros ($J$)\*\* | Decrescentes (calculados sobre o saldo devedor menor). | Decrescentes, mas representam a maior fração da parcela inicial. |

| \*\*Saldo Devedor ($SD$)\*\* | Redução linear e acelerada no início. | Redução lenta nos primeiros anos. |



\#### B. Composição do Custo Efetivo Total (CET)

O CET representa a porcentagem real paga pelo mutuário e é composto por:

1\. \*\*Taxa de Juros do Contrato:\*\* Taxa nominal/efetiva contratada.

2\. \*\*Seguro MIP (Morte e Invalidez Permanente):\*\* Reajustado conforme a faixa etária dos compradores.

3\. \*\*Seguro DFI (Danos Físicos ao Imóvel):\*\* Calculado percentualmente sobre o valor de avaliação do imóvel.

4\. \*\*Tarifa de Administração de Contrato:\*\* Taxa mensal cobrada pela instituição financeira para manutenção da operação.



\---



\### 4.2. Glossário de Conceitos Fundamentais



\- \*\*Amortização ($A$):\*\* Parcela do pagamento mensal destinada exclusivamente à redução do principal da dívida.

\- \*\*Saldo Devedor ($SD$):\*\* Valor remanescente da dívida sobre o qual incidem os juros do período.

\- \*\*CET (Custo Efetivo Total):\*\* Taxa percentual informada ao consumidor que resume todos os encargos, taxas, seguros e juros da operação.

\- \*\*MIP / DFI:\*\* Seguros obrigatórios exigidos em financiamentos habitacionais (MIP = Morte e Invalidez Permanente; DFI = Danos Físicos ao Imóvel).



\---



\### 4.3. Prompts Reutilizáveis para Revisorias e Perícias Futuras



1\. \*\*Simulação e Auditoria de Memória de Cálculo:\*\*

&#x20;  > \*"Atuando como um perito contador especialista em finanças, elabore uma memória de cálculo detalhada dos 12 primeiros meses para um financiamento habitacional com base nos dados das fontes anexadas, comparando lado a lado os métodos SAC e Price."\*

2\. \*\*Análise Crítica de CET x Taxa Nominal:\*\*

&#x20;  > \*"Com base nas diretrizes do Banco Central, explique como identificar se um contrato bancário possui cobranças desalinhadas analisando a diferença percentual entre a Taxa Nominal Contratada e o CET final exibido na proposta."\*

