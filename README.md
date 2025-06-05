
# 🔗 Sistema de Recomendação com Similaridade Cosseno  
### Recomendando produtos com base em vetores de comportamento de compra

<p align="center">
  <img src="https://miro.medium.com/v2/resize:fit:1400/1*G5eDcA1vMpGg2s0gN4tX4g.gif" width="600" alt="Recommender GIF"/>
</p>

---

## 📌 Descrição do Projeto

Este projeto implementa um sistema de recomendação de produtos baseado em **similaridade vetorial**. Utilizando conceitos de **álgebra linear** e **análise de padrões de compra**, a aplicação identifica produtos similares àqueles adquiridos por um cliente, com base na **similaridade cosseno** entre vetores de produtos.

---

## 🧠 Fundamentação Matemática

### 1. Representação Vetorial de Produtos  
Cada produto é representado por um vetor no espaço n-dimensional, onde cada dimensão corresponde a um cliente:

\[
Produto_i = [qtd_{cliente1},\ qtd_{cliente2},\ ..., qtd_{clienteN}]
\]

---

### 2. Matriz de Utilidade  
Construímos uma matriz produto-cliente, onde cada linha representa um produto e cada coluna, um cliente:

```
           Cliente1  Cliente2  ...  ClienteN
Produto1     2         0      ...     1
Produto2     0         3      ...     0
Produto3     1         1      ...     4
```

---

### 3. Similaridade Cosseno  

A **similaridade cosseno** mede o ângulo entre dois vetores, sem considerar magnitude, ideal para capturar padrões de comportamento:

\[
\cos(\theta) = \frac{A \cdot B}{\|A\| \times \|B\|}
\]

- \( A \cdot B \): Produto escalar  
- \( \|A\| \): Norma Euclidiana de A  
- \( \|B\| \): Norma Euclidiana de B


---

## ⚙️ Como Funciona

1. Carrega-se a base de dados com históricos de compras.
2. Gera-se a matriz de utilidade produto-cliente.
3. Calcula-se a matriz de similaridade usando `cosine_similarity`.
4. Ao receber um produto de entrada, são retornados os top produtos mais similares.

---

## 💡 Exemplo de Recomendação

```bash
Digite o ID do produto comprado: 10
```

**Saída:**
```
Produtos recomendados para quem comprou o produto 10:
Produto  Similaridade
  11         72%
  13         64%
  50         62%
```

---

## 📈 Interpretação dos Resultados

- **72% de similaridade**: O vetor do produto 11 tem 72% de alinhamento direcional com o produto 10.
- **Relevância estatística**: Produtos recomendados com base em comportamento coletivo.
- **Complementaridade ou Substituição**: Produtos que geralmente são comprados por perfis semelhantes.

---

## 📂 Tecnologias Utilizadas

- **Pandas** – Manipulação de dados
- **scikit-learn** – Cálculo de similaridade
- **Álgebra Linear** – Cálculo vetorial, norma, produto escalar
- **Python** – Linguagem principal

---

## 🧪 Teste você mesmo

Execute o script principal e insira o ID de um produto para receber recomendações com base em similaridade.

[Clique Aqui](https://github.com/Gusta765/Recomenda-es-de-Produtos-por-Afinidade/blob/main/Sistema_Recomenda%C3%A7%C3%A3o.ipynb)

---

## 📫 Contato

<p align="center">
  <a href="https://www.linkedin.com/in/gustavo-barbosa-868976236/">
    <img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn">
  </a>
  <a href="mailto:gustavobarbosa7744@gmail.com">
    <img src="https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white" alt="Email">
  </a>
  <a href="https://github.com/seu-usuario">
    <img src="https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white" alt="GitHub">
  </a>
</p>
