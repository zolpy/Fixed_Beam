<!-- Simulação de abas usando detalhes -->
<details open>
<summary>🇧🇷 Português</summary>

# 📊 Viga Fixa - Dataset de Deflexão para Diferentes Materiais

Este repositório contém a base de dados `viga_fixa_12plus_materiais_dataset.csv`, utilizada em estudos de modelagem estrutural e aprendizado de máquina. A base representa simulações da deflexão de uma viga engastada (viga fixa em uma extremidade) sujeita a carregamento concentrado, considerando diferentes materiais.

## 📁 Arquivo

* **Nome do arquivo:** `viga_fixa_12plus_materiais_dataset.csv`
* **Registros:** 663 linhas (exemplo completo)
* **Materiais:** 13 diferentes tipos, variando propriedades como módulo de elasticidade, densidade, razão de Poisson e limite de escoamento.

## 📐 Estrutura dos Dados

| Coluna                 | Descrição                                                    |
| ---------------------- | ------------------------------------------------------------ |
| `Material`             | Nome do material (ex: Aço\_Carbono, Alumínio, Concreto etc.) |
| `E_Pa`                 | Módulo de Elasticidade (Young) em Pascal                     |
| `Densidade_kg_m3`      | Densidade do material em kg/m³                               |
| `Poisson_ratio`        | Coeficiente de Poisson                                       |
| `Limite_Escoamento_Pa` | Limite de escoamento do material em Pascal                   |
| `x_m`                  | Posição ao longo da viga em metros                           |
| `y_deflexao_mm`        | Deflexão vertical local em milímetros                        |

## 🧪 Aplicações

Este dataset foi criado para treinar modelos de aprendizado de máquina (como Random Forest) que possam prever curvas de deformação estruturais ponto a ponto, com foco em acelerar análises paramétricas e otimizações estruturais.

### Exemplos de uso:

* Modelagem preditiva de comportamento estrutural
* Geração de modelos *surrogate* (substitutos)
* Estudos comparativos entre materiais
* Validação de soluções analíticas (como a teoria de Euler-Bernoulli)

## 📘 Referência Analítica

As deflexões foram calculadas com base na teoria de Euler-Bernoulli para vigas com peso próprio e carga concentrada na extremidade, com:

* Comprimento da viga: **2.0 m**
* Posição de cálculo da deflexão: 51 pontos ao longo do comprimento
* Consideração do peso próprio do material

## 📌 Observações

* Os dados são sintéticos, gerados numericamente a partir da solução analítica.
* As propriedades dos materiais foram escolhidas para cobrir uma ampla faixa de comportamento elástico.

## 📄 Licença

Este dataset pode ser utilizado livremente para fins acadêmicos e de pesquisa. Para outros usos, consulte os termos da licença incluída neste repositório.


</details>

<details>
<summary>🇺🇸 English</summary>

# 📊 Fixed Beam – Deflection Dataset for Various Materials

This repository contains the dataset `viga_fixa_12plus_materiais_dataset.csv`, designed for structural modeling and machine learning applications. The data represent simulations of the vertical deflection of a cantilever beam (fixed at one end) under a concentrated load, considering various material properties.

## 📁 Dataset Overview

* **Filename:** `viga_fixa_12plus_materiais_dataset.csv`
* **Total Records:** 663
* **Materials:** 13 distinct materials with varying mechanical and physical properties, including Young’s modulus, density, Poisson’s ratio, and yield stress.

## 📐 Data Structure

| Column                 | Description                                                    |
| ---------------------- | -------------------------------------------------------------- |
| `Material`             | Name of the material (e.g., Carbon\_Steel, Aluminum, Concrete) |
| `E_Pa`                 | Young’s modulus in Pascals (Pa)                                |
| `Densidade_kg_m3`      | Material density in kilograms per cubic meter (kg/m³)          |
| `Poisson_ratio`        | Poisson’s ratio                                                |
| `Limite_Escoamento_Pa` | Yield stress in Pascals (Pa)                                   |
| `x_m`                  | Position along the beam (in meters)                            |
| `y_deflexao_mm`        | Local vertical deflection at position `x_m` (in millimeters)   |

## 🧪 Purpose and Applications

This dataset was developed to support the training of machine learning models—such as Random Forests—that aim to predict full structural deflection curves point-by-point. The goal is to facilitate faster parametric analyses and optimizations in structural engineering contexts.

### Potential Applications:

* Predictive modeling of structural behavior
* Surrogate model (meta-model) development
* Comparative studies of material performance
* Validation of analytical beam theories (e.g., Euler-Bernoulli)

## 🧾 Analytical Background

Deflection values were computed using the classical Euler-Bernoulli beam theory, accounting for both self-weight and a concentrated load at the free end. Key modeling assumptions include:

* **Beam Length:** 2.0 meters
* **Deflection Computed At:** 51 equally spaced points along the beam span
* **Material Properties:** Selected to span a representative range of elastic behaviors

## 📌 Notes

* All data are synthetic, numerically generated using closed-form analytical solutions.
* Material names and values reflect realistic engineering use cases, making the dataset suitable for educational, research, and prototyping purposes.

## 📄 License

This dataset is freely available for academic and research use. For commercial or other purposes, please refer to the license terms provided in this repository.

</details>


