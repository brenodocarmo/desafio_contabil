# 🧩 Desafio Técnico – Painel de Indicadores de Receitas

## 🎯 Objetivo
Construir uma **consulta SQL** que consolide dados de duas tabelas de homologação e gere um **painel de indicadores financeiros** baseado nas **receitas, deduções e tributos mensais**.

O resultado final deve permitir a visualização de **valores mensais, acumulados e médias**, além da criação de **indicadores e gráficos de desempenho**.

---

## 🧱 Etapa 1 – Consulta SQL Consolidada

Usando as duas tabelas fornecidas, montar uma consulta que apresente os seguintes campos:

| Campo | Descrição |
|--------|------------|
| `desc_analitica` | Nome da conta analítica (ex: Receita Operacional, ICMS, Devolução de Vendas etc.) |
| `janeiro` a `dezembro` | Valor consolidado por mês |
| `total_acumulado` | Soma de todos os meses |
| `media_mensal` | Média aritmética dos valores mensais |

### Requisitos técnicos
- Consolidar os dados por **descrição analítica** ou **conta contábil**.  
- Tratar valores nulos (meses sem movimento).  
- Calcular corretamente o **total acumulado** e a **média mensal**.  
- Apresentar o resultado em formato **tabelado (pivot)**, como no exemplo de referência.

---

## 📊 Etapa 2 – Cálculo dos Indicadores Financeiros

Com base no resultado da consulta, calcular os seguintes indicadores:

1. **Receita Bruta Total**  
   → Soma das receitas de venda antes das deduções.

2. **Receita Operacional Líquida (ROL)**  
   → Receita Bruta − Deduções de Receita.

3. **% Deduções sobre Receita Bruta**  
   → (Total de deduções / Receita Bruta) × 100.

4. **% Tributos sobre Receita Bruta**  
   → ((ICMS + PIS + COFINS) / Receita Bruta) × 100.

5. **Participação (%) de cada tipo de venda**  
   → (Venda de produtos, equipamentos e serviços / Receita Bruta) × 100.

6. **Crescimento mensal da Receita Total**  
   → Comparar a variação percentual mês a mês.

7. **Projeção Anual (estimada)**  
   → Média mensal × 12.

---

## 📈 Etapa 3 – Construção do Painel

Com os dados da consulta e os indicadores calculados, construir um **painel interativo** (em **Power BI**, **Excel** ou **Google Data Studio**) com os seguintes elementos:

### Painel 1 – Resumo Geral
- Receita total, receita líquida e médias mensais.  
- Indicadores de % de deduções e % de tributos.  
- Gráfico de linha com a evolução mensal da receita total.  

### Painel 2 – Composição da Receita
- Gráfico de pizza ou barras com a participação de cada tipo de venda.  
- Evolução mensal por categoria (produtos, equipamentos, serviços).  

### Painel 3 – Tributos e Deduções
- Gráfico de barras com a evolução mensal de ICMS, PIS e COFINS.  
- Percentual de devoluções em relação à receita.  

---

## 📁 Entrega Esperada

1. **Script SQL** utilizado para gerar o resultado.  
2. **Base de dados exportada** (planilha com o resultado consolidado).  
3. **Painel montado** (Power BI / Excel / Data Studio).  
4. **Resumo com principais insights e observações.**

---

## 💡 Dica
O layout da tabela deve seguir o exemplo mostrado (com colunas de janeiro a dezembro, total e média mensal).  
Capriche na apresentação visual do painel, destacando indicadores-chave de forma clara e intuitiva.

---

### ✅ Sugestão de Organização no Repositório
