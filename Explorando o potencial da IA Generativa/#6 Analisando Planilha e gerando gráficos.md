# Mão na massa: analisando planilha e gerando gráficos

Utilizando o Google AI Studio ou o ChatGPT 4o, faça upload da planilha e peça para que o modelo analise que tipos de dados ela contém.

Depois, peça para o modelo calcular a média aritmética das notas de cada um dos alunos.

Você pode também pedir que o modelo gere um gráfico, como o de dispersão das médias dos estudantes, por exemplo.  
Se não for possível, você pode pedir as instruções para gerar esse gráfico no Excel ou Google Sheets.

---

# Resolução da atividade:
Inicialmente ao importar o arquivo para o ChatGPT e Google AI Studio ocorreu erro básico: o arquivo usa vírgula (`,`) como separador decimal e também como delimitador de coluna, o que confunde o Excel e o Pandas.

- O Excel lê tudo como uma única coluna (A).  
- O Pandas entende parcialmente, mas gera colunas quebradas e linhas extras.

Foi solicitado para o ChatGPT realizar a correção. Posteriormente o ChatGPT e Google AI Studio realizaram as seguintes análises:

### 1. Análises de desempenho individual
- Calcular a média de cada aluno → preencher a coluna “Nota final”.
- Identificar o melhor e o pior aluno com base na média.  
- Classificar alunos por desempenho (ranking).  
- Ver quais alunos ficaram abaixo de uma média mínima (ex: 6.0).  

### 2. Análises gerais da turma 
- Média geral da turma (por prova e no total).  
- Distribuição das notas — ver se as provas estão fáceis ou difíceis.  
- Desvio padrão / variabilidade das notas por prova (ver consistência).  
- Provas com melhor e pior desempenho médio.

## **ChatGPT:**

### Top 5 alunos (ranking por média)
| Posição | Aluno                 | Média Final |
| -------- | --------------------- | ------------ |
| 1 | Marcelo Barbosa | **7,80** |
| 2 | Maria Eduarda Farias | **7,68** |
| 3 | Bruna Oliveira | **7,25** |
| 4 | Lucas Gabriel Ribeiro | **7,05** |
| 5 | Leticia Costa | **7,02** |

**Melhor aluno:** Marcelo Barbosa — média **7,8**  

---

### Alunos abaixo da média mínima (6,0)
| Aluno                 | Nota Final |
| --------------------- | ---------- |
| Mariana Pereira       | 4,28       |
| Ana Paula Oliveira    | 3,92       |
| Natália Guimarães     | 4,75       |
| João Vitor Ferreira   | 4,92       |
| Rodrigo Almeida       | 5,98       |
| Marcos Vinicius Lima  | 5,72       |
| Carla Cristina Castro | 3,05       |

**Pior aluno:** Carla Cristina Castro — média **3,05**

---

### Médias gerais da turma
| Prova   | Média |
| -------- | ------ |
| Prova 1 | **6,44** |
| Prova 2 | **4,71** |
| Prova 3 | **6,59** |
| Prova 4 | **6,03** |

**Média geral da turma (todas as provas): 6,01**

---

### Desvio padrão (variabilidade das notas)
| Prova   | Desvio Padrão |
| -------- | ------------- |
| Prova 1 | 2,5 |
| Prova 2 | 2,9 |
| Prova 3 | 2,1 |
| Prova 4 | 2,8 |

- **Prova 3** foi a mais equilibrada (menor desvio, notas mais consistentes).  
- **Prova 2** foi a mais difícil, com menor média (4,71) e maior dispersão entre alunos.  
- A média geral (**6,01**) indica desempenho mediano da turma.  
- A **Prova 3** teve o melhor desempenho médio e consistência.  
### Resumo final

- **Melhor desempenho médio:** Prova 3 (Média: **6,59**)  
- **Pior desempenho médio:** Prova 2 (Média: **4,71**)  

- A turma apresentou **nível de desempenho razoável**, mas com **dificuldades específicas na Prova 2**.

## **Google AI Studio:**

### Média de cada aluno (Nota Final)

| Aluno | Prova 1 | Prova 2 | Prova 3 | Prova 4 | Nota Final |
|--------|----------|----------|----------|----------|-------------|
| Marcelo Barbosa | 6.5 | 8.3 | 9.2 | 7.2 | **7.8** |
| Rafaela Santos | 8.3 | 4.5 | 7.5 | 4.5 | **6.2** |
| Ronaldo Santos | 7.0 | 2.1 | 8.9 | 8.9 | **6.72** |
| Lucas Gabriel Ribeiro | 5.9 | 9.8 | 6.4 | 6.1 | **7.05** |
| Luana da Silva | 9.2 | 5.6 | 3.1 | 9.8 | **6.92** |
| Mariana Pereira | 4.7 | 1.2 | 5.8 | 5.4 | **4.28** |
| Maria Eduarda Farias | 8.8 | 7.7 | 4.2 | 10 | **7.68** |
| Fernando Henrique Silva | 6.1 | 6.9 | 9.7 | 2.3 | **6.25** |
| Pedro Henrique Souza | 7.2 | 3.4 | 8.0 | 6.7 | **6.32** |
| Ana Paula Oliveira | 0 | 0.5 | 7.2 | 8.0 | **3.92** |
| Natália Guimarães | 5.5 | 4.8 | 5.1 | 3.6 | **4.75** |
| João Vitor Ferreira | 8.0 | 8.9 | 2.8 | 0 | **4.92** |
| Rodrigo Almeida | 7.9 | 2.2 | 6.9 | 6.9 | **5.98** |
| Gustavo Carvalho | 6.4 | 9.1 | 7.6 | 4.3 | **6.85** |
| Leticia Costa | 9.9 | 1.0 | 9.4 | 7.8 | **7.02** |
| Aline da Rocha | 8.5 | 7.2 | 5.7 | 5.0 | **6.6** |
| Marcos Vinicius Lima | 6.8 | 3.3 | 4.5 | 8.3 | **5.72** |
| Carla Cristina Castro | 0 | 6.0 | 5.1 | 1.1 | **3.05** |
| Isabela da Costa | 5.2 | 5.1 | 6.3 | 9.1 | **6.42** |
| Bruna Oliveira | 9.0 | 2.5 | 9.9 | 7.6 | **7.25** |

**Melhor aluno:** Marcelo Barbosa (Média: **7.8**)  
**Pior aluno:** Carla Cristina Castro (Média: **3.05**)

---

### 2. Classificação por Desempenho (Ranking)

1. Marcelo Barbosa (7.8)  
2. Maria Eduarda Farias (7.68)  
3. Bruna Oliveira (7.25)  
4. Lucas Gabriel Ribeiro (7.05)  
5. Leticia Costa (7.02)  
6. Luana da Silva (6.92)  
7. Gustavo Carvalho (6.85)  
8. Ronaldo Santos (6.72)  
9. Aline da Rocha (6.6)  
10. Isabela da Costa (6.42)  
11. Pedro Henrique Souza (6.32)  
12. Fernando Henrique Silva (6.25)  
13. Rafaela Santos (6.2)  
14. Rodrigo Almeida (5.98)  
15. Marcos Vinicius Lima (5.72)  
16. João Vitor Ferreira (4.92)  
17. Natália Guimarães (4.75)  
18. Mariana Pereira (4.28)  
19. Ana Paula Oliveira (3.92)  
20. Carla Cristina Castro (3.05)

---

### 3. Alunos Abaixo da Média Mínima (6.0)

**Abaixo de 6.0:**  
- Mariana Pereira (4.28)  
- Ana Paula Oliveira (3.92)  
- Natália Guimarães (4.75)  
- João Vitor Ferreira (4.92)  
- Rodrigo Almeida (5.98)  
- Marcos Vinicius Lima (5.72)  
- Carla Cristina Castro (3.05)

**Observação:**  
Rafaela Santos (6.2) ficou no limite superior e é considerada acima da média mínima.

---

### 4. Análises Gerais da Turma

### Média Geral por Prova
| Prova | Média |
|--------|--------|
| Prova 1 | **6.44** |
| Prova 2 | **4.71** |
| Prova 3 | **6.59** |
| Prova 4 | **6.03** |

**Média geral da turma (notas finais):** **6.01**

---

### Distribuição e Observações

- **Prova 1** e **Prova 3** apresentaram as maiores médias (6.44 e 6.59).  
- **Prova 2** foi a mais difícil, com média 4.71.  
- **Prova 4** teve desempenho intermediário (6.03).  

- A média geral (6.01) indica desempenho mediano da turma.

---

### Desvio Padrão / Variabilidade das Notas

| Prova | Desvio Padrão | Observação |
|--------|----------------|-------------|
| Prova 1 | ~2.5 | Variabilidade moderada |
| Prova 2 | ~2.9 | Alta variabilidade |
| Prova 3 | ~2.1 | Mais consistente |
| Prova 4 | ~2.8 | Alta variabilidade |
---

### Resumo

- **Melhor desempenho médio:** Prova 3 (Média: **6.59**)  
- **Pior desempenho médio:** Prova 2 (Média: **4.71**)  
- **Conclusão:** A turma apresenta desempenho razoável, com dificuldades específicas na Prova 2. A Prova 3 foi a mais equilibrada e consistente em termos de notas.

---
