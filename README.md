# 📊 Análise Preditiva com Boxplot e Histograma em R

## 📌 Descrição do Projeto

Este projeto demonstra a aplicação de **Análise Preditiva** utilizando dados simulados de salários. A análise é feita por meio da geração de **Boxplot** e **Histograma**, ferramentas estatísticas visuais que ajudam a compreender a distribuição dos dados.

- **Boxplot**: utilizado para observar a dispersão, mediana, quartis e identificar possíveis **outliers** (valores atípicos).
- **Histograma**: utilizado para visualizar a **distribuição de frequência** dos salários, indicando onde os dados estão mais concentrados.

O projeto foi desenvolvido em **R**, utilizando apenas pacotes base, sem necessidade de instalação de bibliotecas adicionais.

---

## 🎯 Objetivo

O principal objetivo é apresentar uma análise descritiva simples e visual de um conjunto de dados simulados, com foco em:

- Identificação da **mediana**, **quartis** e **outliers** por meio do Boxplot.
- Análise da **distribuição de frequência** dos salários com o Histograma.
- Aplicação prática de conceitos estatísticos básicos utilizando R.

---

## 📦 Requisitos

- **R** (qualquer versão recente)
- **Pacotes base** do R (nenhuma instalação adicional necessária)

---

## ▶️ Como Executar

### 1. Instalação do R

Se ainda não possui o R instalado, acesse o site oficial:

🔗 [https://cran.r-project.org/](https://cran.r-project.org/)

### 2. Execução do Código

Abra o R ou o RStudio e execute os seguintes comandos:

```

# Simulação dos dados de salários
set.seed(123)
salarios <- round(rnorm(40, mean = 5.28, sd = 2.62), 2)

# Geração do Boxplot
boxplot(
  salarios,
  main = "Boxplot dos Salários",
  ylab = "Salário (U$)",
  col = "lightblue",
  horizontal = TRUE
)

# Geração do Histograma
hist(
  salarios,
  main = "Histograma dos Salários",
  xlab = "Salário (U$)",
  col = "lightgreen",
  border = "black"
)

