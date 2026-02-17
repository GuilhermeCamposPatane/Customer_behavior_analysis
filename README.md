🛍️ Análise do Comportamento de Compra dos Clientes
📌 Visão Geral do Projeto

Este projeto analisa o comportamento de compra dos clientes utilizando dados transacionais de 3.900 compras distribuídas em diversas categorias de produtos.

O principal objetivo é identificar insights sobre:

Padrões de gasto

Segmentação de clientes

Preferências de produtos

Comportamento de assinatura

Principais direcionadores de receita

A análise combina Python (EDA e Tratamento de Dados), PostgreSQL (Consultas de Negócio) e Power BI (Visualização em Dashboard) para gerar insights estratégicos.

📊 Resumo do Dataset

Linhas: 3.900

Colunas: 18

Valores Ausentes: 37 (na coluna de Avaliação)

🔎 Principais Variáveis

Demografia dos Clientes

Idade

Gênero

Localização

Status de Assinatura

Detalhes da Compra

Produto Comprado

Categoria

Valor da Compra

Estação

Tamanho

Cor

Comportamento de Compra

Desconto Aplicado

Código Promocional

Compras Anteriores

Frequência de Compras

Avaliação

Tipo de Envio

🐍 Análise Exploratória de Dados (Python)

A preparação e limpeza dos dados foram realizadas em Python.

✔ Carregamento dos Dados

Importação utilizando a biblioteca pandas

✔ Exploração Inicial

df.info() para verificar estrutura

df.describe() para estatísticas descritivas

✔ Tratamento de Dados Ausentes

Identificados 37 valores ausentes em review_rating

Substituição pela mediana da avaliação por categoria de produto

✔ Padronização de Colunas

Conversão dos nomes das colunas para snake_case

✔ Engenharia de Features

Criação da coluna age_group (agrupamento por faixa etária)

Criação da coluna purchase_frequency_days

Remoção da coluna redundante promo_code_used

✔ Integração com Banco de Dados

Conexão do Python com PostgreSQL

Carregamento do dataset tratado para análise em SQL

🗄️ Análise de Negócio (SQL – PostgreSQL)

Foram realizadas consultas estruturadas para responder perguntas estratégicas:

1️⃣ Receita por Gênero

Comparação da receita total gerada por clientes masculinos e femininos.

2️⃣ Clientes de Alto Gasto com Desconto

Identificação de clientes que utilizaram desconto e ainda assim gastaram acima da média.

3️⃣ Top 5 Produtos por Avaliação

Ranking dos produtos com maior média de avaliação.

4️⃣ Comparação por Tipo de Envio

Comparação do valor médio de compra entre:

Envio Padrão

Envio Expresso

5️⃣ Assinantes vs. Não Assinantes

Análise de:

Ticket médio

Receita total

Impacto da assinatura na receita

6️⃣ Produtos Dependentes de Desconto

Identificação dos produtos com maior percentual de vendas com desconto.

7️⃣ Segmentação de Clientes

Classificação dos clientes em:

🆕 Novos

🔁 Recorrentes

⭐ Fiéis

8️⃣ Top 3 Produtos por Categoria

Ranking dos produtos mais vendidos dentro de cada categoria.

9️⃣ Compradores Frequentes e Assinaturas

Análise da relação entre clientes com mais de 5 compras e probabilidade de assinatura.

🔟 Receita por Faixa Etária

Cálculo da contribuição de receita por grupo de idade.

📈 Dashboard (Power BI)

Foi desenvolvido um dashboard interativo no Power BI para visualizar:

Distribuição da receita

Segmentação de clientes

Performance de assinaturas

Produtos mais vendidos

Contribuição por faixa etária

Comportamento por tipo de envio

O dashboard permite exploração dinâmica dos dados para apoiar a tomada de decisão estratégica.

💡 Recomendações Estratégicas
🚀 Incentivar Assinaturas

Oferecer benefícios exclusivos para aumentar receita recorrente.

🎯 Programas de Fidelidade

Criar incentivos para transformar clientes recorrentes em clientes fiéis.

💰 Revisão da Política de Descontos

Equilibrar estratégias promocionais com controle de margem.

🏆 Posicionamento de Produtos

Destacar produtos mais bem avaliados e mais vendidos em campanhas.

📊 Marketing Direcionado

Focar esforços em:

Faixas etárias de maior receita

Usuários de envio expresso

Clientes fiéis

🛠️ Tecnologias Utilizadas

Python (Pandas, Limpeza e Engenharia de Dados)

PostgreSQL (Consultas e Análise de Negócio)

Power BI (Visualização e Dashboard Interativo)
