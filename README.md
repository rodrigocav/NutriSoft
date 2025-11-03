# 🍎 NutriSoft – Software de Cálculo Nutricional  

**NutriSoft** é um aplicativo desktop desenvolvido em **Java (NetBeans + Swing)**, criado para auxiliar **nutricionistas** em cálculos rotineiros de **avaliação corporal e recomendações nutricionais**.  

🧑‍🎓 Projeto acadêmico desenvolvido no **curso Senac EAD (2022)**.

---

## 📋 Funcionalidades

### ✅ Cálculo de IMC (Índice de Massa Corporal)
- Fórmula: `IMC = Peso / Altura²`
- Exibe automaticamente a **interpretação** do resultado:
  - *Magreza* — IMC < 18,5  
  - *Normal* — 18,5 ≤ IMC < 24,9  
  - *Sobrepeso* — 25 ≤ IMC < 29,9  
  - *Obesidade* — 30 ≤ IMC < 39,9  
  - *Obesidade grave* — IMC ≥ 40  

---

### ✅ Cálculo de Gasto Calórico Basal e Total
Baseado em fórmulas específicas para **homens** e **mulheres**:

- **Homem:**  
  `CalBasal = 66 + (13,8 × Peso) + (5 × Altura) – (6,8 × Idade)`
- **Mulher:**  
  `CalBasal = 655 + (9,6 × Peso) + (1,9 × Altura) – (4,7 × Idade)`

💪 O **gasto calórico total** é calculado conforme o **nível de atividade física**:

| Nível de Atividade | Fator | Fórmula |
|--------------------|--------|----------|
| Sedentário | 1.2 | CalBasal × 1.2 |
| Leve (1–3 dias/semana) | 1.375 | CalBasal × 1.375 |
| Moderado (3–5 dias/semana) | 1.55 | CalBasal × 1.55 |
| Ativo (5–6 dias/semana) | 1.725 | CalBasal × 1.725 |
| Extremamente ativo (diário) | 1.9 | CalBasal × 1.9 |

---

### ✅ Recomendações Nutricionais
Com base no **gasto calórico total**, o programa calcula automaticamente as recomendações diárias:

- **Carboidratos:** `Calorias × 0,5 / 4`  
- **Proteínas:** `Calorias × 0,25 / 4`  
- **Gorduras:** `Calorias × 0,25 / 9`  

Os resultados são exibidos em **gramas (g)**, de forma clara e intuitiva.

---

## 🧠 Validações e Usabilidade

- 🚫 **Campos obrigatórios:** o sistema exige o preenchimento completo antes dos cálculos.  
- ⚠️ **Entradas inválidas:** o programa trata erros (como letras em vez de números) com **mensagens amigáveis**, sem travar.  
- 🪟 **Interface intuitiva:** cada cálculo é aberto em uma nova janela sobre a tela principal.  

---

## 🖥️ Telas do Sistema

1. **Tela Inicial:** acesso rápido às funcionalidades.  
2. **Tela IMC:** entrada de peso e altura com resultado imediato.  
3. **Tela Gasto Calórico:** coleta dados e calcula o gasto energético.  
4. **Tela Recomendações:** gera valores ideais de macronutrientes.  

> *(As telas foram desenvolvidas com o construtor visual do NetBeans – Swing GUI Builder.)*

---

## 🛠️ Tecnologias Utilizadas

- ☕ **Java SE 8+**  
- 🧩 **NetBeans IDE**  
- 🪟 **Swing (Interface Gráfica Desktop)**  
- 🧮 **Lógica de Programação e Validação de Dados**

---

## 🚀 Como Executar o Projeto

1. Abra o projeto no **NetBeans**.  
2. Execute a classe principal (`Main.java` ou `TelaInicial.java`).  
3. A tela inicial será exibida com as opções de cálculo.  

> 💡 Certifique-se de ter o **JDK 8 ou superior** instalado no seu computador.

---

## 🧮 Fórmulas Utilizadas

| Cálculo | Fórmula |
|----------|----------|
| **IMC** | Peso / (Altura²) |
| **CalBasal (Homem)** | 66 + (13,8 × Peso) + (5 × Altura) – (6,8 × Idade) |
| **CalBasal (Mulher)** | 655 + (9,6 × Peso) + (1,9 × Altura) – (4,7 × Idade) |
| **Carboidratos** | Calorias × 0,5 / 4 |
| **Proteínas** | Calorias × 0,25 / 4 |
| **Gorduras** | Calorias × 0,25 / 9 |

---

## 👨‍💻 Autor

Desenvolvido por **[Seu Nome Aqui]**  
📚 Projeto acadêmico – **Senac EAD (2022)**  

---

## 🏷️ Licença

Este projeto é de uso **educacional e não comercial**.  
Sinta-se à vontade para **estudar, modificar e melhorar**. 🙌  

---

### ⭐ Dica

Se gostou deste projeto, deixe uma **estrela (★)** no repositório para apoiar! 😄
