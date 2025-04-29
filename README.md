# Análise Preditiva: Boxplot e Histograma

## Descrição

Este projeto demonstra a aplicação de **Análise Preditiva** usando dados simulados de salários, com a criação de **Boxplot** e **Histograma** para visualização das distribuições de dados.

- **Boxplot**: Utilizado para identificar a dispersão dos salários, mostrar a mediana e os possíveis **outliers**.
- **Histograma**: Mostra a distribuição de frequências dos salários em intervalos definidos.

O código foi implementado em **R**, utilizando pacotes padrão para análise estatística e visualização gráfica.

## Objetivo

O objetivo deste projeto é realizar uma análise básica de um conjunto de dados, destacando:
- A mediana, quartis e **outliers** (valores atípicos) com o **Boxplot**.
- A distribuição dos salários com o **Histograma**, que mostra em quais intervalos de salários a maioria dos dados se concentram.

## Como Rodar o Código

### Requisitos
- **R** (qualquer versão recente)
- Pacotes **base** (sem necessidade de instalação adicional)

### Passos para execução

1. Instale o **R** se ainda não tiver em seu sistema: [https://cran.r-project.org/](https://cran.r-project.org/)
   
# Simulação dos salários
set.seed(123)
salarios <- round(rnorm(40, mean = 5.28, sd = 2.62), 2)

# Boxplot
boxplot(salarios,
        main = "Boxplot dos Salários",
        ylab = "Salário (U$)",
        col = "lightblue",
        horizontal = TRUE)

# Histograma
hist(salarios,
     main = "Histograma dos Salários",
     xlab = "Salário (U$)",
     col = "lightgreen",
     border = "black")


---

**Resultados Esperados**:
- **Boxplot**: A caixa representará a distribuição dos dados, com a mediana e os quartis. Os bigodes irão mostrar os valores típicos e qualquer ponto fora deles será considerado um outlier.
- **Histograma**: As barras indicarão em quais faixas de salários a maioria dos dados se encontra.

---

