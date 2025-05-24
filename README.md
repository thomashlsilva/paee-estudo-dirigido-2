# Estudo Dirigido 2 - Planejamento e Análise Estatística de Experimentos (PAEE)

Este repositório contém um Jupyter Notebook desenvolvido para a disciplina de **PAEE**, focado na aplicação de modelos estatísticos com ênfase em **ANOVA** e na validação do **Teorema Central do Limite (TCL)** através de simulações.

## 📘 Descrição

O notebook aborda os seguintes tópicos principais:

- Análise de Variância (ANOVA):
  - ANOVA a um fator
  - ANOVA a dois fatores
  - ANOVA com interação entre fatores
  - ANOVA com blocagem
  - Comparação de modelos usando Critério de Informação de Akaike (AIC)

- Estatística Não Paramétrica:
  - Geração de populações assimétricas
  - Verificação da normalidade com o Teste de Shapiro-Wilk
  - Validação empírica do Teorema Central do Limite (TCL)
  - Avaliação do comportamento do teste t sob distribuições não normais
  - Implementação de testes t pareados para amostras assimétricas

## 🛠️ Ferramentas e Pacotes

- Linguagem: **R v4.5**
- Ambiente: **Jupyter Notebook** com suporte ao kernel de R (`IRkernel`)
- Principais pacotes utilizados:
  - `ggplot2`
  - `ggpubr`
  - `tidyverse`
  - `broom`
  - `AICcmodavg`

## ▶️ Execução

### Requisitos:

1. Instale o kernel de R no Jupyter:

```r
install.packages("IRkernel")
IRkernel::installspec()
````

2. Instale os pacotes necessários:

```r
install.packages(c("ggplot2", "ggpubr", "tidyverse", "broom", "AICcmodavg"))
```

3. Execute o notebook no ambiente Jupyter.

### Leitura dos dados:

Os dados são lidos utilizando o comando:

```r
crop.data <- read.csv("caminho/para/seu/arquivo/crop.data.csv",
                      header = TRUE,
                      colClasses = c("factor", "factor", "factor", "numeric"))
```

> Substitua `"caminho/para/seu/arquivo"` pelo caminho onde está seu arquivo CSV.

## 📁 Arquivos

* `paee-estudo-dirigido-2.ipynb`: notebook com todas as análises e simulações do estudo dirigido 2.
* `crop.data.csv`: arquivo de dados utilizado nas análises.

## 🎯 Objetivos de Aprendizado

* Aplicar ANOVA em diferentes contextos experimentais.
* Compreender os efeitos de interação e blocagem.
* Validar empiricamente o Teorema Central do Limite (TCL).
* Analisar a robustez de testes paramétricos sob populações não normais.
* Realizar e interpretar testes t pareados.

## ✍️ Autor

Este notebook foi desenvolvido como parte das atividades da disciplina **Planejamento e Análise Estatística de Experimentos (PAEE)** do **CEFET-MG**, ministrada pelos professores **Elizabeth Fialho Wanner** e **Fabio Rocha da Silva**.
