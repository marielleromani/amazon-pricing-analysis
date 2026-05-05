# Amazon Pricing Analysis: Desconto como Alavanca ou Armadilha?

## Contexto

Descontos são uma das estratégias mais usadas para impulsionar vendas.
Mas nem sempre mais desconto significa mais valor.

Esse projeto explora como diferentes níveis de desconto se relacionam
com a percepção do cliente, usando avaliações (ratings) como proxy.

## Problema

Descontos aumentam conversão no curto prazo, mas podem:

- reduzir margem
- atrair clientes menos qualificados
- impactar negativamente a percepção de valor do produto

A pergunta é simples: até que ponto o desconto ajuda — e quando começa a prejudicar?

## Hipótese

Descontos muito altos (acima de 70%) podem estar associados a pior avaliação média dos produtos.

## 📈 Visualizações

![Distribuição de Preços e Descontos](fig1_distribuicao.png)

![Top Categorias por Volume e Desconto](fig2_categorias.png)

![Matriz Estratégica: Ticket × Satisfação](fig7_matriz.png)

![Avaliação por Faixa de Desconto](fig8_ponto_otimo.png)

## Análise

A análise considera:

- distribuição de descontos no catálogo (551k produtos, 142 categorias)
- relação entre faixa de desconto e avaliação média
- segmentação estratégica por perfil de categoria

Os dados foram organizados em faixas de desconto para observar padrões de comportamento.

## Insight Principal

Existe uma tendência clara: quanto maior o desconto, pior a avaliação média do produto.

Produtos com descontos extremos (acima de ~70%) apresentam, de forma consistente,
avaliações mais baixas.

## Business Decision

Desconto nem sempre é alavanca.

Se o ganho incremental não compensar a perda de margem e o impacto na percepção
do cliente, ele passa a ser destruição de valor.

Na prática, isso sugere:

- evitar descontos extremos como estratégia padrão
- testar elasticidade de preço por categoria
- priorizar margem em vez de volume em determinados cenários

## Limitações

Essa análise é um ponto de partida. Em um cenário real, seria necessário validar:

- margem por produto
- quanto das vendas é realmente incremental
- impacto no comportamento do cliente ao longo do tempo (retenção, dependência de desconto)

## Próximos Passos

- rodar testes A/B para medir impacto real de desconto
- segmentar por categoria e tipo de produto
- incorporar métricas financeiras (margem, CAC, LTV)

## Estrutura do Projeto

| Arquivo | Descrição |
|---|---|
| `amazon_pricing_analysis.ipynb` | Análise exploratória completa |
| `fig1` a `fig8` | Gráficos e visualizações |

## Conclusão

Nem todo crescimento é ganho real.

Em alguns casos, parar de dar desconto pode ser a melhor decisão de negócio.

## 🔗 Links

[📝 Artigo completo no Substack](https://marielleromani.substack.com/p/desconto-como-alavanca-ou-armadilha)  
[📦 Dataset no Kaggle](https://www.kaggle.com/datasets/lokeshparab/amazon-products-dataset)

---

*Análise desenvolvida por Marielle Romani | Python · Pandas · Matplotlib · Seaborn*
