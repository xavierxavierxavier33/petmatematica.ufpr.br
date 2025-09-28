+++
title = "Uma cota superior para Álgebras de dimensão finita"
date = 2025-09-28T08:00:00-03:00
draft = false

tags = ["petiscos"]
eventos = []

showAuthor = true
autores = ["feli.k"]
+++

{{< katex >}}

Uma _álgebra_ sobre um corpo \\(\mathbb{K}\\), ou uma \\(\mathbb{K}\\)-álgebra, é um espaço vetorial \\(A\\) sobre o corpo \\(\mathbb{K}\\) munido de um produto bilinear e associativo.

Em outras palavras, dados arbitrários \\(a\\) e \\(b\\) do espaço \\(A\\), exatamente nessa ordem, existe um elemento unicamente definido de \\(A\\) que chamamos de _elemento produto_, denotamos por \\(ab\\), em que as seguintes condições são satisfeitas:

- \\(a(b+c) = ab+ac \\);
- \\((b+c)a = ba+ca \\);
- \\((\alpha a)b = a(\alpha b) = \alpha (ab) \\);
- \\((ab)c = a(bc)\\),


em que \\(c\\) também é um elemento arbitrário de \\(A\\) e \\(\alpha\\) é um escalar arbitrário do corpo \\(\mathbb{K}\\).

Uma álgebra \\(A\\) é dita de _dimensão finita_ ou de _dimensão infinita_ se o \\(\mathbb{K}\\)-espaço vetorial \\(A\\) é de dimensão finita ou dimensão infinita, respectivamente. A dimensão de um espaço vetorial \\(A\\) é chamada de _dimensão da álgebra \\(A\\)_ e é denotada por \\([A:\mathbb{K}]\\).

Segue da bilinearidade do produto que, dada uma base \\(\left\{ a_i\right\}_{i=1}^n\\), o produto é unicamente determinado pelo produto dos vetores da base \\(b_{ij} = a_ia_j\\). De fato, dados \\(a,b \in A\\), existem coeficientes \\(\alpha_k \in \K\\) e \\(\beta_k \in \K\\), \\(k=1,2,\cdots,n\\), tais que \\(a = \sum_{i=1}^n \alpha_i a_i\\) e \\(b = \sum_{j=1}^n \beta_j a_j\\). Assim,

$$
\begin{align*}
	ab 
	&= \left( \sum_{i=1}^n \alpha_i a_i \right) \left( \sum_{j=1}^n \beta_j a_j \right)
	= \sum_{i=1}^n \left( \alpha_i a_i \sum_{j=1}^n \beta_j a_j \right)
	= \sum_{i=1}^n \sum_{j=1}^n \alpha_i a_i \beta_j a_j \nonumber \\\\
	&= \sum_{i=1}^n \sum_{j=1}^n \alpha_i \beta_j a_i a_j 
	= \sum_{i=1}^n \sum_{j=1}^n \alpha_i \beta_j b_{ij}
\end{align*}
$$

Decompondo os vetores \\(b_{ij}\\) com respeito a base, temos que existem constantes \\(\gamma_{ij}^k \in \K\\), \\(k=1,2,\cdots,n\\), tais que \\(b_{ij} = \sum_{k=1}^n \gamma_{ij}^k a_k\\), para \\(i,j=1,2,\cdots,n\\). Esses elementos são chamados de _constantes estruturais_ de \\(A\\). Dessa forma,

$$
\begin{align*}
	ab 
	&= \sum_{i=1}^n \sum_{j=1}^n \alpha_i \beta_j b_{ij} 
	= \sum_{i=1}^n \sum_{j=1}^n \alpha_i \beta_j \sum_{k=1}^n \gamma_{ij}^k a_k
	= \sum_{i=1}^n \sum_{j=1}^n \sum_{k=1}^n \alpha_i \beta_j \gamma_{ij}^k a_k \\\\
	&= \sum_{k=1}^n \sum_{i=1}^n \sum_{j=1}^n  \alpha_i \beta_j \gamma_{ij}^k a_k
	= \sum_{k=1}^n \left( \sum_{i=1}^n \sum_{j=1}^n  \alpha_i \beta_j \gamma_{ij}^k \right) a_k
\end{align*}
$$

Como a operação é unicamente definida pelo produto dos vetores da base e há no máximo a escolha de \\(n^3\\) constantes \\(\gamma_{ij}^k\\), \\(i,j,k=1,2,\cdots,n\\), temos que existem no máximo \\(n^3\\) produtos em um \\(\mathbb{K}\\)-espaço vetorial de dimensão \\(n\\). 

Note que \\(n^3\\) é apenas uma cota superior. A escolha dos vetores \\(b_{ij}\\), e logo das constantes \\(\gamma_{ij}^k\\), não pode ser arbitrária. Elas devem ser escolhidas de tal forma que cumpram os axiomas da álgebra.