# 🎮 Dashboard de Vendas Xbox (Excel)

Dashboard interativo de vendas feito em Excel, transformando dados brutos em indicadores e gráficos para apoiar decisões.

## 📁 Conteúdo
- `dashboard_vendas_xbox.xlsx` – arquivo final com o dashboard.
- `README.md` – este documento.

## 📊 Estrutura do arquivo
| Aba | Função |
|---|---|
| **Dashboard** | KPIs, filtros e gráficos |
| **Base** | Dados brutos de vendas (tabela `tbVendas`) |
| **Calc** | Tabelas auxiliares (SUMIFS) que alimentam KPIs e gráficos |

### Indicadores (KPIs)
Receita, Lucro, Margem, Pedidos, Unidades e Ticket Médio.

### Gráficos
- Receita e Lucro por mês (linha)
- Receita por categoria (colunas)
- Receita por região (colunas)
- Top 5 produtos (barras)
- Receita por vendedor (barras)

### Filtros
Listas suspensas (células amarelas) de **Ano**, **Região** e **Categoria**. Todos os KPIs e gráficos respondem a elas.

## 🗂️ Dados utilizados
Colunas da aba `Base`: Data, Pedido, Produto, Categoria, Região, Vendedor, Quantidade, Preço Unitário, Custo Unitário, e as colunas calculadas Receita, Custo Total, Lucro, Ano e Mês.

> ⚠️ **Importante:** a base oficial do desafio (`base.xlsx`) não pôde ser baixada no ambiente em que este projeto foi gerado. Por isso, o arquivo contém **720 pedidos simulados** (2024–2025, produtos Xbox: consoles, acessórios, jogos e assinaturas). Os valores não representam vendas reais.

## 🔁 Como reproduzir / usar sua própria base
1. Abra `dashboard_vendas_xbox.xlsx` e vá à aba **Base**.
2. Cole seus dados nas colunas A–I (mantendo os cabeçalhos). Se tiver mais linhas, arraste as fórmulas J–N para baixo e redimensione a tabela `tbVendas`.
3. Se houver mais linhas que o intervalo atual, ajuste os intervalos nas fórmulas da aba **Calc** (ou use *Localizar e Substituir* no final do intervalo).
4. Se seus produtos, regiões ou vendedores forem diferentes, edite os nomes nas tabelas da aba **Calc** (colunas E, H, K, R) e as listas dos filtros (Dados › Validação de Dados).
5. Volte ao **Dashboard**: tudo se atualiza automaticamente (Fórmulas › Calcular Agora, se necessário).

## 🛠️ Recursos do Excel utilizados
`SUMIFS`, `COUNTIFS`, `INDEX/MATCH`, `LARGE`, Tabelas do Excel, Validação de Dados, gráficos nativos.

## 📜 Licença
Uso livre para fins educacionais.
