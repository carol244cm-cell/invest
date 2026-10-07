# 📊 Simulador de Investimento em Fundos Imobiliários (FIIs)

Esta ferramenta interativa em Excel foi desenvolvida para simular e projetar o acúmulo de património e o rendimento mensal de dividendos ao investir em Fundos Imobiliários (FIIs), permitindo uma tomada de decisão consciente alinhada ao perfil do investidor.

---

## ❓ As 5 Perguntas de Negócio que a Ferramenta Responde

A planilha foi desenhada no formato de aplicação e responde diretamente às seguintes perguntas:

1. **Quanto investir por mês?** — Definido na célula do aporte mensal (ex.: `R$ 230,00`).
2. **Por quantos anos?** — Prazo do investimento selecionado pelo utilizador (ex.: `5 anos`).
3. **Qual a taxa de rendimento mensal?** — Taxa esperada de rentabilidade mensal do fundo/carteira (ex.: `1,08% a.m.`).
4. **Quanto de património vai acumular?** — Calculado automaticamente no campo *Património Acumulado* (ex.: `R$ 19.268,69` em 5 anos).
5. **Quanto vai receber de dividendos por mês?** — Estimativa de rendimento mensal recorrente obtida com o património acumulado (ex.: `R$ 171,49/mês`).

---

## 📐 Como a Função VF e o PROCV Entram nos Cálculos

### 1. Função `VF` (Valor Futuro)
Calcula o montante total acumulado ao final do período com aportes mensais constantes.
* **Fórmula utilizada:**
  ```excel
  =VF(Taxa_Mensal; Qntd_anos * 12; Investimento_Mensal * -1)
