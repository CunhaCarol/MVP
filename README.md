# Wine Quality Analysis – Análise exploratória e modelagem preditiva com base no dataset Wine Quality

Este repositório apresenta um projeto de análise exploratória, processamento de dados e modelagem preditiva com base no dataset **Wine Quality – White**, da UCI Machine Learning Repository. Desenvolvido como MVP, o projeto investiga padrões químicos que influenciam a avaliação sensorial de vinhos brancos, testando hipóteses e construindo modelos de classificação com aprendizado de máquina.

---

## Sobre o dataset

- **Fonte:** [UCI Wine Quality Dataset](https://archive.ics.uci.edu/ml/datasets/wine+quality)
- **Tipo:** CSV separado por `;`
- **Amostras:** 4898 vinhos brancos
- **Atributos:** 11 variáveis físico-químicas + 1 nota sensorial (`quality`, de 0 a 10)

---

## Objetivos

- Explorar estatísticas descritivas e relações entre atributos físico-químicos
- Verificar se vinhos bons e ruins possuem perfis químicos distintos
- Criar *features* derivadas com base em conhecimento químico
- Construir modelos de classificação para prever qualidade sensorial
- Testar hipóteses orientadas por domínio e dados

---

## Hipóteses testadas

1. Existe correlação significativa entre teor alcoólico e açúcar residual?
2. É possível distinguir vinhos de diferentes níveis de qualidade com base em atributos físico-químicos?
3. Vinhos bons são mais facilmente identificáveis pelos modelos?

---

## Como executar

Você pode carregar o dataset diretamente via GitHub com:

```python
import pandas as pd

url = 'https://raw.githubusercontent.com/CunhaCarol/WINE/refs/heads/main/winequality-white.csv'
df = pd.read_csv(url, sep=';')  # O separador é ; porque o dataset original da UCI é assim
df.head()
