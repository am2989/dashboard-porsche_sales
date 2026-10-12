# Porsche Sales Intelligence Dashboard

Dashboard interativo desenvolvido no âmbito do desafio da DIO para análise de vendas Porsche através de HTML, CSS e JavaScript.

A solução transforma uma base de dados de vendas numa dashboard visual e interativa, permitindo explorar indicadores, gráficos e filtros sem depender do Excel ou de qualquer ferramenta externa.

## Dashboard Publicada

🔗 Dashboard: https://am2989.github.io/dashboard-porsche_sales/

🔗 Repositório: https://github.com/am2989/dashboard-porsche_sales

---

# Objetivo do Projeto

O objetivo deste projeto foi transformar uma planilha de vendas Porsche numa dashboard web interativa que permitisse responder a perguntas reais de negócio através de visualizações de dados simples e intuitivas.

Toda a aplicação está contida num único ficheiro HTML, sem dependências externas e pronta para publicação no GitHub Pages.

---

# Perguntas de Negócio Escolhidas

## 1. Quais são os modelos Porsche mais vendidos?

### Porquê?

Esta análise permite identificar quais os modelos com maior procura no mercado, ajudando equipas comerciais e de marketing a compreender tendências de consumo.

### Visualização Utilizada

- Gráfico "Modelos mais vendidos"

---

## 2. Em que cidades existe maior concentração de vendas?

### Porquê?

Permite identificar os mercados mais relevantes e as regiões onde existe maior procura pelos veículos da marca.

### Visualização Utilizada

- Gráfico "Vendas por cidade"
- Tabela resumo por cidade
- Ranking de modelos líderes por cidade

---

## 3. Quais são os métodos de pagamento preferidos pelos clientes?

### Porquê?

Ajuda a compreender o comportamento de compra dos clientes e pode apoiar decisões relacionadas com financiamento, crédito e processos financeiros.

### Visualização Utilizada

- Gráfico de distribuição dos métodos de pagamento

---

# Tratamento da Base de Dados

Antes da utilização da IA para gerar a dashboard, foi realizado o tratamento da base de dados disponibilizada no desafio:

- Utilização apenas dos campos sanitizados.
- Conversão dos campos numéricos para formato adequado.
- Validação dos campos de preço e ano.
- Remoção de dependências de fórmulas da folha de cálculo.
- Preservação dos registos com datas inválidas para análises gerais.
- Exclusão dessas datas em análises temporais.

Após o tratamento, os dados foram incorporados diretamente no HTML através de uma estrutura JavaScript.

---

# Prompt Utilizado

O prompt inicial utilizado para gerar a dashboard foi semelhante ao seguinte:

> Cria uma dashboard em HTML único para análise de vendas Porsche.
>
> A dashboard deve conter:
>
> - Filtros por modelo, cidade, ano e método de pagamento;
> - Indicadores de total de vendas e receita;
> - Gráfico dos modelos mais vendidos;
> - Gráfico das vendas por cidade;
> - Gráfico da distribuição por métodos de pagamento;
> - Layout moderno inspirado em dashboards executivas;
> - Design responsivo para computador e dispositivos móveis;
> - Utilização exclusiva de HTML, CSS e JavaScript.

---

# Evolução do Prompt

Ao longo do desenvolvimento foram feitos vários refinamentos:

### Versão Inicial

- Apenas KPIs e gráficos básicos.

### Melhorias Adicionadas

- Ranking dos modelos mais populares por cidade.
- Insights automáticos baseados nos filtros ativos.
- Tabela resumida por cidade.
- Melhor responsividade para dispositivos móveis.
- Modo de edição do conteúdo textual.
- Melhor organização visual inspirada em dashboards empresariais.

---

# Funcionalidades Implementadas

## Filtros

- Modelo Porsche
- Ano do modelo
- Cidade
- Método de pagamento

## Indicadores (KPIs)

- Total de vendas
- Receita total
- Modelo líder
- Ano dominante

## Visualizações

- Top 8 modelos mais vendidos
- Top 8 cidades com mais vendas
- Distribuição por model year
- Distribuição por método de pagamento
- Ranking de líderes por cidade
- Tabela resumo por cidade

## Extras

- Insights automáticos
- Interface responsiva
- Canvas editável
- Armazenamento local das alterações (localStorage)

---

# Tecnologias Utilizadas

- HTML5
- CSS3
- JavaScript (Vanilla JS)
- SVG para gráficos
- GitHub Pages para publicação

---

# Estrutura do Projeto

```text
dashboard-porsche_sales
│
├── index.html
└── README.md
```

---

# Como Executar

1. Clonar o repositório:

```bash
git clone https://github.com/am2989/dashboard-porsche_sales.git
```

2. Abrir o ficheiro:

```text
index.html
```

em qualquer navegador moderno.

---

# Evidências do Projeto

Sugere-se incluir:

- Captura de ecrã da dashboard.
- Captura de ecrã com filtros aplicados.
- Captura de ecrã da publicação no GitHub Pages.

Estas evidências ajudam a demonstrar o correto funcionamento da solução.

---

# Conclusão

Este projeto demonstra como uma folha de cálculo pode ser transformada numa dashboard web interativa através de IA generativa, HTML, CSS e JavaScript.

A dashboard permite responder rapidamente a questões de negócio relacionadas com procura por modelos, distribuição geográfica das vendas e preferências de pagamento, disponibilizando uma alternativa mais flexível e visual do que uma análise tradicional em Excel.

---

## Autor

**Alda Benta**

Projeto desenvolvido para o desafio da DIO - Dashboard Porsche Sales.

Este projeto tem fins exclusivamente educativos e não possui qualquer afiliação oficial com a Porsche.

