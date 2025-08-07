# 💰 Calculadora de Imposto de Renda - C#

Este projeto em C# calcula o imposto de renda devido com base em faixas salariais progressivas, similar ao modelo aplicado no Brasil.

## 📋 Descrição

O programa solicita o valor do salário e aplica as alíquotas de forma progressiva, de acordo com a tabela:

| Faixa salarial (R$)         | Alíquota  | Observação                                      |
|-----------------------------|-----------|-------------------------------------------------|
| Até 2000,00                 | 0%        | Isento                                          |
| De 2000,01 até 3000,00      | 8%        | Apenas sobre o valor que exceder R$ 2000,00     |
| De 3000,01 até 4500,00      | 18%       | Apenas sobre o valor que exceder R$ 3000,00     |
| Acima de 4500,00            | 28%       | Apenas sobre o valor que exceder R$ 4500,00     |

## 🧠 Lógica aplicada

- **Leitura de dados** com `Console.ReadLine()`
- **Conversão numérica** com `double.Parse()` e `CultureInfo.InvariantCulture`
- **Estruturas condicionais** para aplicar a alíquota correta
- **Cálculo progressivo**: cada faixa é tributada separadamente

## ▶️ Exemplo de uso

**Entrada:**
Digite o valor do salario: R$5000.00

**Saída:**
R$ 490.00

Explicação:
- 8% de R$ 1000,00 = R$ 80,00
- 18% de R$ 1500,00 = R$ 270,00
- 28% de R$ 500,00 = R$ 140,00
- **Total**: R$ 490,00

## 🛠️ Tecnologias utilizadas

- C#
- .NET SDK
- Console Application
