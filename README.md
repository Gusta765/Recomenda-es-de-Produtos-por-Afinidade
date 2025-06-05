🚀 Sistema de Recomendação Baseado em Similaridade de Produtos
🔍 Visão Geral do Modelo
Este sistema de recomendação utiliza álgebra linear e similaridade vetorial para identificar produtos relacionados com base nos padrões de compra dos clientes. 
O núcleo matemático do modelo é o cálculo de similaridade cosseno entre vetores que representam o comportamento de compra de diferentes produtos.

<p align="center"> <img src="https://miro.medium.com/v2/resize:fit:1400/1*G5eDcA1vMpGg2s0gN4tX4g.gif" alt="Sistema de Recomendação" width="600"> </p>
📚 Fundamentação Matemática
1. Representação Vetorial de Produtos
Cada produto é representado como um vetor no espaço n-dimensional de clientes:

Produto_i = [qtd_cliente_1, qtd_cliente_2, ..., qtd_cliente_n]

Onde cada dimensão corresponde às quantidades compradas por um cliente único.

2. Matriz de Utilidade
Construímos uma matriz produto-cliente:

        Cliente1  Cliente2  ...  ClienteN
ProdA   [  qa1      qa2     ...    qaN    ]
ProdB   [  qb1      qb2     ...    qbN    ]
...
ProdZ   [  qz1      qz2     ...    qzN    ]

3. Similaridade Cosseno
A similaridade entre produtos A e B é calculada por:

                A • B
cos(θ) = -----------------
           ||A|| * ||B||

Onde:

A • B = produto escalar dos vetores

||A|| e ||B|| = normas Euclidianas

<p align="center"> <img src="https://www.researchgate.net/profile/Hans-Georg-Stark/publication/301874235/figure/fig1/AS:669956433379332@1536748952244/Illustration-of-the-cosine-similarity-principle.png" alt="Similaridade Cosseno" width="400"> </p>

📊 Resultado de Exemplo

Suponhamos que o cliente tenha adiquirido o produto 10 

Digite o ID do produto comprado: 10

Produtos recomendados para quem comprou o produto 10:
Produto  Similaridade
  11         72%
  13         64%
  50         62%

📈  Interpretação dos Resultados
72% de similaridade: Os padrões de compra dos produtos têm 72% de alinhamento vetorial

Recomendações significativas: Produtos frequentemente comprados pelos mesmos clientes

Complementaridade: Itens que podem ser substitutos ou complementares

📫 Contato
<p align="center"> <a href="https://www.linkedin.com/in/gustavo-barbosa-868976236/"> <img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn"> </a> <a href="mailto:gustavobarbosa7744@gmail.com"> <img src="https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white" alt="Email"> </a> <a href="https://github.com/seu-usuario"> <img src="https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white" alt="GitHub"> </a> </p>
