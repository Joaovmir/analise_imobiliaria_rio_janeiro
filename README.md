# Análise Imobiliária no Rio de Janeiro 🏠📊🌎

[![Python](https://img.shields.io/badge/python-3.8%2B-blue.svg)](https://www.python.org/)

Este repositório apresenta uma análise exploratória e espacial do mercado imobiliário do Rio de Janeiro, integrando **dados de imóveis** e **informações geográficas de setores censitários**. O objetivo é revelar padrões, tendências de preços, distribuição espacial dos imóveis e insights relevantes para tomada de decisão.

---

## 🌟 Motivação

Compreender o mercado imobiliário de grandes cidades exige analisar variáveis econômicas, sociais e, principalmente, o **contexto geográfico** dos imóveis. Unir dados tabulares com informações espaciais permite descobrir regiões valorizadas, clusters de imóveis e oportunidades para compradores, investidores e gestores públicos.

---

## 🎯 Objetivos do Projeto

- Realizar uma **análise exploratória** dos dados de imóveis à venda no Rio de Janeiro.
- Integrar os dados de imóveis com **setores censitários** georreferenciados (shapefile).
- Gerar **visualizações espaciais** dos preços, densidade de ofertas e outros atributos.
- Identificar padrões geográficos, clusters de preços e desigualdades espaciais.
- Fornecer um **notebook interativo** para replicação, adaptação ou aprofundamento dos estudos.

---

## 🗂️ Etapas do Projeto

1. **Carregamento dos dados de imóveis** (arquivo `dados_imoveis.csv`)
2. **Download dos arquivos de setores sensitários**: [IBGE](https://www.ibge.gov.br/geociencias/downloads-geociencias.html?caminho=organizacao_do_territorio/malhas_territoriais/malhas_de_setores_censitarios__divisoes_intramunicipais/2021/Malha_de_setores_%28shp%29_por_UFs)
3. **Leitura dos arquivos de setores censitários** (pasta `rj_setores_censitarios/rj_setores_censitarios` com arquivos `.shx`, `.dbf`, `.prj`)
4. **Limpeza e pré-processamento** dos dados tabulares e espaciais
5. **Integração** dos imóveis com setores censitários via geolocalização
6. **Análise estatística** e visualização de variáveis-chave (preço, área, número de quartos, etc.)
7. **Visualização geográfica**: mapas de calor, clusters, distribuição dos imóveis por região
8. **Discussão dos resultados** e insights sobre o mercado imobiliário carioca

---

## 📚 Tecnologias Utilizadas

- [Python 3.8+](https://www.python.org/)
- [Pandas](https://pandas.pydata.org/)
- [Geopandas](https://geopandas.org/) — Leitura e manipulação de shapefiles
- [Matplotlib](https://matplotlib.org/) e [Seaborn](https://seaborn.pydata.org/) — Visualização
- [Shapely](https://shapely.readthedocs.io/) — Operações geométricas
- [PySAL](https://pysal.org/) ou [Folium](https://python-visualization.github.io/folium/) — (opcional) Mapas interativos e análise espacial

---

## ⚡ Como Rodar o Projeto

### 1. Clone o repositório

```bash
git clone https://github.com/Joaovmir/analise_imobiliaria_rio_janeiro.git
cd analise_imobiliaria_rio_janeiro
```

### 2. Instale as dependências

```bash
pip install pandas geopandas matplotlib seaborn shapely
# (adicione folium ou pysal se usar mapas interativos/clusterização espacial)
```

## 📁 Estrutura do Projeto

```
analise_imobiliaria_rio_janeiro/
├── analise_imobiliaria_rio_janeiro.ipynb
├── dados/
│   ├── dados_imoveis.csv
│   └── rj_setores_censitarios/
│       └── rj_setores_censitarios/
│           ├── 33SEE250GC_SIR.dbf
│           ├── 33SEE250GC_SIR.prj
│           ├── 33SEE250GC_SIR.shx
├── README.md
```

---

## 🔎 Interpretação e Expansões Possíveis

* Identificação de bairros e regiões mais valorizadas ou acessíveis
* Análise de densidade e concentração de imóveis à venda
* Mapas de clusters de preços e características dos imóveis
* Possibilidade de adaptar para aluguel ou outras cidades

---


