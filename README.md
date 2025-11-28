📊 Análise de Performance de E-commerce: Receita & Logística

Este repositório contém o código fonte, relatório e materiais de apresentação do projeto final de Análise de Dados, focado em diagnosticar a saúde financeira e operacional de um e-commerce brasileiro.

👥 Equipe de Dados

Embarque Digital (3º Período)

Joyce Cristine

Albean Santiago

🎯 Objetivo do Projeto

A direção solicitou respostas confiáveis (com tratamento estatístico) sobre receita, margens, frete, prazos de entrega e comportamento do cliente. O objetivo foi produzir um pipeline reprodutível que vai da ingestão de dados até a inferência estatística.

KPIs Analisados

Financeiro: Receita, Ticket Médio, Share de Frete.

Logística: Lead Time (Prazo de Entrega), Taxa de Atraso, Performance por UF.

Cliente: Taxa de Conversão de Pagamentos, Comportamento Regional (SP vs RJ).

🛠️ Tecnologias Utilizadas

O projeto foi desenvolvido inteiramente em Python, utilizando as seguintes bibliotecas para manipulação e estatística:

pandas: Limpeza e manipulação de DataFrames.

numpy: Cálculos numéricos e geração de dados sintéticos.

seaborn & matplotlib: Visualização de dados (EDA).

scipy.stats: Testes de hipótese (T-test, Shapiro-Wilk, Levene).

statsmodels: Intervalos de confiança para proporções.

📂 Estrutura do Repositório

📁 /
├── analise_ecommerce.py    # Script principal (Gera dados, analisa e plota)
├── Relatorio_Analitico.md  # Relatório técnico detalhado para a diretoria
├── Apresentacao.md         # Roteiro para apresentação (Canvas/PPT)
├── GRAFICOS.png            # Painel visual gerado pelo script
└── README.md               # Documentação do projeto


🚀 Como Executar

Pré-requisitos

Certifique-se de ter o Python instalado. Recomenda-se o uso de um ambiente virtual (venv).

Clone o repositório:

git clone [https://github.com/seu-usuario/nome-do-repo.git](https://github.com/seu-usuario/nome-do-repo.git)
cd nome-do-repo


Instale as dependências:

pip install pandas numpy seaborn matplotlib scipy statsmodels


Execute a análise:

python analise_ecommerce.py


O script irá gerar os dados simulados, exibir os gráficos na tela e imprimir o Sumário Executivo no terminal.

📉 Principais Insights (Spoiler)

A análise revelou um cenário de alta conversão financeira, mas com gargalos logísticos graves:

Alerta Crítico: A taxa de atraso global é de ~48%. Quase metade dos pedidos não chega na data prometida.

Ineficiência do "Same-Day": A modalidade expressa não apresentou vantagem estatística de pontualidade sobre o frete padrão.

Saúde Financeira: O Ticket Médio é sólido (R$ 1.021,92) e a conversão de pagamentos é excelente (89%).

Regionalização: Estatisticamente, clientes de SP e RJ possuem o mesmo comportamento de gasto (p-value > 0.05), permitindo estratégias de marketing unificadas.

📋 Metodologia (Pipeline)

Geração de Dados: Simulação de 1.000 pedidos com ruídos realistas (nulos, duplicatas).

Limpeza: Deduplicação e tratamento de pedidos em trânsito.

Feature Engineering: Cálculo de Lead Time e flags de atraso.

EDA: Análise visual de distribuições e correlações.

Inferência: Aplicação de ICs (95%) e Testes de Hipótese para validar conclusões.

Made with 💜 by Joyce & Albean.
