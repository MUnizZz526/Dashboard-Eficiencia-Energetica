# 💡 Dashboard de Gestão de Eficiência Energética

Este projeto consiste em uma solução completa de análise de dados e gestão de eficiência energética, criada para rastrear e otimizar o consumo de energia (kWh) em um escritório. O foco está na identificação dos vilões sazonais (Ar Condicionado e Chuveiro) e no cálculo do potencial de economia.

## 📊 1. Dados e Estrutura

Os dados utilizados são **simulados** com base em um cenário realista de uma Pequena Agência de Marketing Digital no clima quente do Brasil. O dataset foi estruturado para refletir a correlação direta entre temperatura e consumo (picos de AC no Verão e picos de Chuveiro no Inverno).

O arquivo de dados principal, **`dados.csv`**, está localizado na pasta `/data`.

| Campo | Descrição |
| :--- | :--- |
| `REF` / `N.MÊS` | Rótulo do mês e ordem numérica para garantir a cronologia correta dos gráficos. |
| `ESTAÇÃO` | Categoria principal para filtros sazonais (Verão, Inverno, etc.). |
| `AR COND(kWh)` | Consumo detalhado de Ar Condicionado (pico no Verão). |
| `CHUVEIRO (kWh)` | Consumo detalhado do Chuveiro (pico no Inverno). |
| `PCs(kWh)` | Consumo de computadores (principal foco de otimização 24/7). |
| `TOTAL (kWh)` / `TOTAL EM R$` | Consumo consolidado e custo financeiro (Base: R$ 0,90/kWh). |

## 📈 2. Resultados Chave e Impacto Financeiro

A análise demonstrou que, ao implementar ações de eficiência específicas, o escritório pode alcançar uma economia substancial.

| Métrica | Ano sem Otimização (Real) | Ano Otimizado (Meta) | Ganho Financeiro |
| :--- | :---: | :---: | :---: |
| **Consumo Total Anual** | **10.070 kWh** | **8.159,75 kWh** | **1.910,25 kWh** |
| **Custo Total Anual** | **R$ 9.063,00** | **R$ 7.343,78** | **R$ 1.719,22** |
| **Redução Percentual** | N/A | **18,97%** | N/A |

### Distribuição dos Consumidores (Situação Real)

Os três maiores vilões do consumo anual são o foco da otimização:

1.  **Ar Condicionado:** 31,28%
2.  **PCs e Periféricos:** 30,83%
3.  **Chuveiro:** 27,81%

## 🎯 3. Foco nas Ações de Otimização

A estratégia para atingir a redução de **18,97%** é focada nas seguintes ações de custo zero/baixo:

| Área | Período de Ação | Dica de Otimização | Meta de Redução |
| :--- | :--- | :--- | :--- |
| **Ar Condicionado** | Verão (Pico) | Padronização do termostato para $\mathbf{23{}^\circ\text{C}}$ e uso de temporizadores para desligamento pós-expediente. | 15% |
| **PCs e Periféricos** | Ano Todo | Implementação de uma política rigorosa de desligamento total dos equipamentos (incluindo monitores) para combater o consumo fantasma. | 25% |
| **Chuveiro** | Inverno (Pico) | Instalação de redutores de vazão e conscientização sobre o tempo de banho para reduzir a demanda de aquecimento de água. | 20% |

## ⚙️ 4. Orientações de Execução

O arquivo **`dashboard_final.xlsx`** (localizado em `/docs`) contém toda a Dashboard interativa, gráficos e Tabelas Dinâmicas configuradas.

**Como utilizar a Dashboard:**

1.  Faça o download do arquivo `dashboard_final.xlsx`.
2.  Utilize os filtros de **Mês** e **Estação** (segmentadores) para ver como o consumo, o custo e o ranqueamento dos equipamentos mudam sazonalmente.
3.  A Dashboard está pronta para ser atualizada: insira novos dados de consumo nas abas de origem e clique em **Dados > Atualizar Tudo** para gerar novos insights.
