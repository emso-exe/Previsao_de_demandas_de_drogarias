# 🔎 Previsão de demandas de drogarias 🏪

A Rossmann é uma das maiores redes de drogarias da Europa, com sede na Alemanha e filiais em outros países europeus. Suas lojas oferecem uma ampla variedade de produtos, incluindo medicamentos, itens de higiene pessoal, cosméticos, alimentos, entre outros. Na plataforma [Kaggle](https://www.kaggle.com/competitions/rossmann-store-sales), a Rossmann disponibilizou um conjunto de dados para uma competição focada na previsão da demanda de vendas.

## 🚨 Contexto do problema

Atualmente, os gerentes de cada filial da Rossmann são responsáveis por prever suas vendas diárias com até seis semanas de antecedência. As vendas de cada loja são influenciadas por diversos fatores, como promoções, feriados, localização, entre outros, o que pode resultar em uma grande variação na precisão das previsões. A criação de um modelo preditivo de demandas de vendas para as próximos seis semanas ajudará os gerentes a focarem mais em seus clientes e funcionários.

## 💼 Demanda do negócio

- Construir novas variáveis;
- Desenvolver um modelo preditivo de demanda de vendas.

## 📃 Compreensão dos dados

Os dados disponíveis incluem três arquivos em formato _CSV_: _train.csv_/_test.csv_, que contêm dados históricos de vendas, e _store.csv_, que oferece informações suplementares sobre as lojas. Os dados de vendas cobrem o período de 31/12/2012 a 16/09/2015, e foram extraídos do portal [Kaggle - Rossmann Store Sales](https://www.kaggle.com/competitions/rossmann-store-sales). O conjunto de dados inclui informações detalhadas sobre faturamento, número de clientes diários, indicadores de funcionamento das lojas, promoções, concorrentes, entre outros fatores temporais.

## 📓 Dicionário de dados

**Arquivos: train.csv/test.csv**
| Variáveis | Descrição | Domínios |
|-----------|-----------|----------|
| **Store** | Um Id exclusivo para cada loja. | |
| Id | Um Id que representa um (Store, Date) duplicado dentro do conjunto de teste. | |
| DayOfWeek | |
| Date | |
| Sales | O faturamento de um determinado dia. | |
| Customers | O número de clientes em um determinado dia. | |
| Open | Um indicador para saber se a loja estava aberta. | 0 = fechada, 1 = aberta |
| Promo | Indica se uma loja está realizando uma promoção naquele dia. | |
| StateHoliday | Indica um feriado estadual. Normalmente, todas as lojas, com poucas exceções, fecham em feriados estaduais. Observe que todas as escolas fecham em feriados e fins de semana. | a = feriado público, b = feriado de Páscoa, c = Natal, 0 = Nenhum |
| SchoolHoliday | Indica se a loja foi afetada pelo fechamento de escolas públicas. | |

**Arquivo: store.csv**
| Variáveis | Descrição | Domínios |
|-----------|-----------|----------|
| **Store** | Um Id exclusivo para cada loja. | |
| StoreType | Classificação entre 4 modelos de loja diferentes. | a, b, c, d |
| Assortment | Descreve um nível de sortimento | a = básico, b = extra, c = estendido|
| CompetitionDistance | Distância em metros até a loja concorrente mais próxima | |
| CompetitionOpenSinceMonth | Fornece o mês aproximado em que o concorrente mais próximo foi aberto. | |
| CompetitionOpenSinceYear | Fornece o ano aproximado em que o concorrente mais próximo foi aberto. | |
| Promo2 | É uma promoção contínua e consecutiva para algumas lojas. | 0 = a loja não está participando, 1 = a loja está participando |
| Promo2SinceWeek | Descreve a semana do calendário em que a loja começou a participar da **Promo2**. | |
| Promo2SinceYear | Descreve o ano em que a loja começou a participar da **Promo2**. | |
| PromoInterval | Descreve os intervalos consecutivos em que o **Promo2** é iniciado, nomeando os meses em que a promoção é reiniciada. Por exemplo, _"Fev, Mai, Ago, Nov"_ significa que cada rodada começa em fevereiro, maio, agosto, novembro de qualquer ano para aquela loja | |

> fonte: [Rossmann Store Sales](https://www.kaggle.com/competitions/rossmann-store-sales)

## 💻 Tecnologias

- Python
  - Biblioteca GC
  - Biblioteca Pandas
  - Biblioteca GeoPandas
  - Biblioteca Matplotlib
  - Biblioteca Seaborn
  - Biblioteca MissingNo
  - Biblioteca Numpy
  - Biblioteca Warnings
  - Biblioteca Tabulate
  - Biblioteca TextWrap
  - Biblioteca Unidecode
- PySpark
  - Biblioteca OS
  - Biblioteca Time


## 💳 Créditos

- [Estênio Mariano](https://github.com/emso-exe)

## 🔖 Licença

Licença MIT (MIT). Por favor leia o [arquivo da licença](LICENSE.md) para mais informações.