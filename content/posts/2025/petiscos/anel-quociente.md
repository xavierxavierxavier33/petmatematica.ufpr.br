+++
title = "Um anel quociente conveniente"
date = 2025-08-26T08:00:00-03:00
draft = false

tags = ["petiscos"]
eventos = []

showAuthor = true
autores = ["feli.k"]
+++

{{< katex >}}

Há muita desconfiança quando se fala em números complexos. Muito disse se deve à mística do nome imaginários. Esse nome confunde: parece sugerir que o que está sendo discutido não existe na realidade. Se já faço pouco números reais, imagine dos números imaginários.

Apesar do nome, quero te mostrar que esses números são bem concretos. A existência de um objeto cujo quadrado é negativo surge de forma natural na teoria de aneis e corpos. Estamos sempre nos perguntando quais propriedades um anel possui e, muitas vezes, as resposta aparecem ao analisar os polinômios com coefientes nesse anel. 

Considere um corpo \\(\mathbb{K} \\) munido das operações soma \\(+ \\) e produto \\(\cdot \\). Denotamos por \\(\mathbb{K}[x] \\) o anel de polinômios com coeficiente em \\(\mathbb{K} \\), isto é,

$$
p \in \mathbb{K}[x] \iff p(x) = a_0 + a_1 \cdot x + ... + a_n \cdot x^n =\sum_{i=0}^n a_i \cdot x^i \text{, onde } a_i \in \mathbb{K}, \forall i=1,2,...,n, \text{ para algum } n \in \N \text{.}
$$

Segue da teoria que, como \\(\mathbb{K} \\) é corpo, \\(\mathbb{K}[x] \\) é um domínio de ideais principais. Isto é, para todo ideal \\(I \subset \mathbb{K}[x] \\) existe um polinômio \\(f(x) \in I \\) tal que \\(\left<f(x)\right> = I \\).

Agora, considere \\(\mathbb{K} = \R \\), o elemento \\(f(x) = x^2 + 1 \in \R[x] \\) e o ideal \\(I \\) gerador por \\(f(x) \\):

$$
I = \left <f(x)\right> = \lbrace g(x) \in \R[x] \thickspace \vert \thickspace g(x) = f(x) \cdot h(x) \text{ para algum h(x) } \in \R[x] \rbrace
$$

Vejamos o que acontece no quociente \\(\frac{\R[x]}{\left<f(x)\right>} \\). Dado o elemento \\([x] \in \frac{\R[x]}{\left<f(x)\right>} \\) temos:

$$
    [x]^2 = [x^2] = [x^2 - f(x)] = [x^2 - (x^2 + 1)] = [x^2 - x^2 - 1] = [-1]
$$

Ou seja, no quociente existe um elemento tal que seu quadrado é \\(-1 \\). Esse elemento é a classe do polinômio identidade.

Além disso, como o grau de \\(f(x) \\) é dois, toda a classe admite um representante de grau no máximo 1. Em outras palavras, todos os elementos do quociente são da forma \\([ax+b] \\) para algum \\(a,b \in \R \\). É fácil ver, pelo isomorfismo 

$$
\phi: \frac{\R[x]}{\left<f(x)\right>} \to \mathbb{C} \text{, dado por } [x] \mapsto i \in \mathbb{C} \text{,}
$$

que

$$
\frac{\R[x]}{\left<x^2 + 1\right>} \cong \mathbb{C} \text{ e } \phi([a+bx]) = a+bi, \forall a,b \in \R
$$

O polinômio \\(f(x) = x^2 + 1 \\) pode parecer tirado da cartola, mas na verdade surge naturalmente como um polinômio irredutível de grau 2 em \\(\R[x] \\). Para mim, a construção dos reais a partir dos racionais é de longe mais imaginária do que esta apresentada.
