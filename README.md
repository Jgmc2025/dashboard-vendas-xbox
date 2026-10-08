# 🎮 Dashboard de Vendas · Xbox Game Pass Subscriptions (Excel)

Dashboard interativo em Excel que transforma a base bruta de assinaturas do Xbox Game Pass em indicadores e gráficos para análise de desempenho de vendas.

## 📁 Conteúdo
- `dashboard_xbox_game_pass.xlsx` – arquivo final com o dashboard.
- `README.md` – este documento.

## 🗂️ Dados utilizados
Base oficial do desafio (`base.xlsx`): **295 assinaturas** iniciadas entre **01/01/2024 e 16/12/2024**.

| Coluna | Descrição |
|---|---|
| Subscriber ID / Name | Identificação do assinante |
| Plan | Core (R$ 5), Standard (R$ 10) ou Ultimate (R$ 15) |
| Start Date | Data de início |
| Auto Renewal | Renovação automática (Yes/No) |
| Subscription Type | Monthly, Quarterly ou Annual |
| EA Play Season Pass (+ Price) | Adicional EA Play (R$ 30) |
| Minecraft Season Pass (+ Price) | Adicional Minecraft (R$ 20) |
| Coupon Value | Desconto aplicado |
| Total Value | Plano + EA Play + Minecraft − Cupom |

## 📊 Estrutura do arquivo
| Aba | Função |
|---|---|
| **Assets** | Paleta de cores e logos do projeto |
| **Bases** | Base de dados (tabela `Tabela1`) + coluna auxiliar `Month` |
| **Cálculos** | Perguntas de negócio respondidas com fórmulas |
| **Dashboard** | Visualização final com filtros, KPIs e gráficos |

## ❓ Perguntas de negócio respondidas
1. Qual o faturamento total de planos anuais? → **R$ 1.754**
2. Faturamento de planos anuais por auto renovação → **R$ 1.537** (com) / **R$ 217** (sem)
3. Total de vendas do EA Play Season Pass → **R$ 2.940**
4. Total de vendas do Minecraft Season Pass → **R$ 3.880**
5. Como evolui a receita mês a mês?
6. Qual plano gera mais receita? (Ultimate: R$ 5.388)
7. Qual periodicidade vende mais? (Monthly: R$ 3.571)
8. Do que é composta a receita? (mensalidade, EA Play, Minecraft e cupons)
9. Quantos assinantes têm auto renovação?

> Valores sem filtros aplicados. Receita total: **R$ 7.633** · Ticket médio: **R$ 25,87**.
> Validação: com o filtro *Monthly*, o dashboard reproduz o gabarito do desafio (R$ 3.571 / EA Play R$ 1.350 / Minecraft R$ 1.800).

## 🎛️ Dashboard
- **KPIs:** Receita Total, Assinantes, Ticket Médio, EA Play, Minecraft e Cupons.
- **Gráficos:** receita por mês, por plano, por tipo de assinatura, composição da receita e assinantes por auto renovação.
- **Filtros (listas suspensas):** Tipo de assinatura, Plano e Auto renovação.
- **Planos anuais:** faixa fixa respondendo as perguntas 1 e 2.

## 🔁 Como reproduzir
1. Abra `dashboard_xbox_game_pass.xlsx` no Excel.
2. Para usar outra base, cole os dados na aba **Bases** (colunas A–M, mesmos cabeçalhos).
3. Se houver mais linhas, estenda a tabela e os intervalos `Bases!$X$2:$X$296` nas fórmulas da aba **Cálculos**.
4. Volte ao **Dashboard**; os valores e gráficos atualizam sozinhos.

## 🛠️ Recursos utilizados
`SUMIFS`, `COUNTIFS`, `MIN/MAX`, Tabela do Excel, Validação de Dados, gráficos nativos e a paleta Xbox do template.
