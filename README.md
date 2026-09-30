# 📈 Simulador de Controle de Investimentos em FIIs

Ferramenta desenvolvida em Excel para simulação e planejamento de investimentos em Fundos Imobiliários (FIIs) com base no perfil de risco do investidor.

---

## 🎯 Perguntas de Negócio Respondidas
* **Quanto investir por mês?** (Valor de entrada definido pelo usuário)
* **Por quantos anos?** (Prazo de acumulação)
* **Qual a taxa de rendimento mensal?** (Rendimento esperado da carteira)
* **Quanto de patrimônio vai acumular?** (Calculado via função `VF`)
* **Quanto vai receber de dividendos por mês?** (Estimativa com base no patrimônio acumulado)

---

## 🧮 Fórmulas e Intervalos Nomeados

### Fórmulas Utilizadas
* **`VF` (Valor Futuro):** Utilizada para calcular o montante final acumulado considerando os aportes mensais recorrentes, a taxa mensal e o prazo em anos.
* **`PROCV` com Chave Composta:** Utilizada na tabela de apoio para buscar o percentual exato alocado para cada **Tipo de FII** combinando o **Perfil do Investidor** e o tipo do fundo.

### Intervalos Nomeados
* `ganho_mensal`: Salário/Renda informada.
* `aporte_mensal`: Valor destinado ao investimento por mês.
* `taxa_mensal`: Taxa de rendimento estimada.
* `qtd_anos`: Período de acumulação em anos.

---

## 📊 Distribuição por Perfil de Investidor

| Perfil | Papel | Tijolo | Híbridos | FOFs | Desenvolvimento | Hotelarias |
| :--- | :---: | :---: | :---: | :---: | :---: | :---: |
| **Conservador** | 60% | 20% | 10% | 10% | 0% | 0% |
| **Moderado** | 40% | 30% | 10% | 10% | 5% | 5% |
| **Agressivo** | 50% | 10% | 5% | 5% | 20% | 10% |

---

## 🚀 Diferenciais e Melhorias
* **Design de Aplicação:** Remoção das linhas de grade e ocultação de elementos do Excel para um visual limpo.
* **Projeção Multicenários:** Tabela dinâmica de cenários simulando prazos de 2 a 30 anos.
* **Gráfico Dinâmico:** Visualização da distribuição dos FIIs atualizada conforme o perfil selecionado.
