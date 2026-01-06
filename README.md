# Projeto Power BI: Ex-02

Este repositório contém o ficheiro de projeto do Power BI (`Ex-02.pbix`), desenvolvido para a análise de dados e visualização de indicadores chave de desempenho (KPIs).

## 📊 Visão Geral do Relatório

O objetivo deste painel é fornecer insights sobre **[Insira aqui o tema, ex: Vendas, Recursos Humanos, Financeiro]**, permitindo a análise de tendências e o apoio à tomada de decisão.

**Principais funcionalidades:**
* Navegação interativa entre páginas.
* Filtros dinâmicos por **[ex: Período, Região, Categoria]**.
* Análise comparativa (**[ex: Ano Atual vs Ano Anterior]**).

## 💾 Fontes de Dados

O relatório é alimentado pelas seguintes fontes:

* **Excel / CSV:** `[Nome do ficheiro.xlsx]` (Dados de transações).
* **Base de Dados:** `[SQL Server / Web / SharePoint]` (Tabelas de dimensão).
* **Tabelas Calculadas:** Tabelas auxiliares criadas em DAX (ex: Tabela dCalendario).

## 🗂 Estrutura do Modelo de Dados

O modelo de dados segue o esquema **Star Schema** (Estrela) para otimização de performance:

### Tabelas de Factos (f)
* `fVendas` (ou o nome da tua tabela principal): Contém os registos históricos e valores transacionais.

### Tabelas de Dimensão (d)
* `dProduto`: Cadastro e detalhes dos itens.
* `dCliente`: Segmentação e localização dos clientes.
* `dCalendario`: Datas para inteligência temporal (Time Intelligence).

## 📈 Principais Métricas (DAX)

As principais medidas calculadas incluem:

1.  **Total de Vendas:** Soma do valor faturado.
2.  **Ticket Médio:** `Total de Vendas / Contagem de Pedidos`.
3.  **Variação YoY (%):** Comparativo com o mesmo período do ano anterior.
4.  **Margem de Lucro:** `(Receita - Custo) / Receita`.

## 🛠 Pré-requisitos e Como Executar

Para visualizar ou editar este projeto, é necessário:

1.  Ter o **Microsoft Power BI Desktop** instalado.
2.  Fazer o download do ficheiro `Ex-02.pbix`.
3.  Ao abrir, caso os dados não carreguem, vá a **Transformar Dados > Definições da Fonte de Dados** e atualize o caminho para os ficheiros locais (se aplicável).

---
*Projeto desenvolvido no âmbito do exercício Ex-02.*
