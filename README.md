# Porsche — Sales Intelligence

Dashboard interativo de vendas, desenvolvido no âmbito de um desafio da DIO. Transforma um conjunto de dados brutos de vendas Porsche em informação visual: indicadores, rankings e gráficos que se atualizam em tempo real conforme os filtros escolhidos.

Tudo corre num único ficheiro (`index.html`), sem instalações, sem servidor e sem dependências externas.

## Funcionalidades

- **Filtros combináveis** por modelo, *model year*, cidade e método de pagamento, com botão para limpar tudo.
- **4 indicadores (KPIs):** vendas registadas, valor total de vendas, modelo líder e *model year* dominante.
- **Gráficos em SVG:**
  - Modelos mais vendidos (Top 8)
  - Vendas por cidade (Top 8)
  - Distribuição por *model year*
  - Métodos de pagamento (gráfico em anel com legenda)
- **Leitura do mercado:** três insights gerados automaticamente a partir do recorte filtrado.
- **Modelos populares por cidade** e **tabela-resumo por cidade** (unidades, modelo líder e quota do líder).
- **Canvas editável:** o botão *Editar canvas* permite alterar os textos do dashboard diretamente; as alterações ficam guardadas no navegador (`localStorage`).
- **Responsivo:** adapta-se a ecrãs de computador, tablet e telemóvel.

## Dados utilizados

O dataset está embutido no próprio `index.html` (constante `DATA`) e foi sanitizado antes de ser usado.

| Campo | Descrição |
|---|---|
| `id` | Identificador do registo |
| `date` | Data da venda (pode estar vazia) |
| `model` | Modelo Porsche |
| `year` | *Model year* |
| `price` | Valor registado da venda |
| `mileage` | Quilometragem |
| `pay` | Método de pagamento |
| `city` / `state` | Cidade e estado |
| `status` | Estado da encomenda (ex.: Delivered, Pending, In Transit, Cancelled) |

**Resumo do conjunto:** 100 registos · 40 modelos · 7 *model years* · 79 cidades · 9 métodos de pagamento.

## Notas de qualidade dos dados

- **24 registos sem data válida:** são mantidos nas métricas de vendas e excluídos de qualquer análise temporal.
- **Moeda não especificada:** os valores são apresentados tal como constam no ficheiro, sem validação nem conversão de moeda.
- **Empates:** vários modelos têm o mesmo número de unidades (4); o "modelo líder" mostrado corresponde ao primeiro na ordenação, pelo que deve ser lido com essa ressalva.
- **Datas fora do esperado:** existem datas posteriores à data atual no conjunto, o que deve ser validado na origem dos dados.

## Como executar (reprodução)

1. Descarregue ou clone este repositório:
   ```bash
   git clone [https://github.com/am2989/dashboard-porsche_sales).git
   ```
2. Abra o ficheiro `index.html` num navegador (duplo clique chega).
3. Use os filtros no topo para explorar os dados.

### Publicar online com GitHub Pages (opcional)

1. No repositório, vá a **Settings → Pages**.
2. Em **Source**, escolha a branch `main` e a pasta `/ (root)`.
3. Guarde. Ao fim de alguns minutos o dashboard fica disponível em `https://github.com/am2989/dashboard-porsche_sales`.

## Para usar outros dados

Substitua o conteúdo da constante `DATA` no `index.html` por uma lista de objetos com os mesmos campos descritos acima. Os filtros, KPIs e gráficos adaptam-se automaticamente.

## Tecnologias

- HTML5, CSS3 e JavaScript (vanilla)
- Gráficos desenhados em SVG, sem bibliotecas externas

## Estrutura do repositório

```
.
├── index.html   # Dashboard completo (interface, dados e lógica)
└── README.md    # Este ficheiro
```

## Autoria

Desenvolvido por **Alda Benta** no âmbito de um desafio de dashboard de vendas da DIO.

> Interface demonstrativa para exploração do ficheiro fornecido. Projeto com fins formativos, sem qualquer ligação oficial à Porsche.
