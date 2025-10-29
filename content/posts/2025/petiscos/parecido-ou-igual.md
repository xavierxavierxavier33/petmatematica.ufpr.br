+++
title = "Parecido ou igual? Equivalências Categóricas"
date = 2025-10-26T08:00:00-03:00
draft = false

tags = ["petiscos"]
eventos = []

showAuthor = true
autores = ["pedr.a"]
revisores = ["Juan Sebastián Herrera Carmona"]
+++

{{< katex >}}

Na matemática, ideias sobre o quão parecidas são duas estruturas nascem naturalmente no estudo: simetrias, isomorfismo ou equivalências entre objetos ou estruturas. Estudamos estas _"semelhanças"_ a nível de objetos - grupos isomorfos entre si, isometrias de uma figura -, mas também podemos estudá-las a nível categórico. Neste _Petisco_ entederemos como duas categorias são equivalentes e o que isto nos diz sobre seus objetos e morfismos.

Quando estudamos equivalências entre categorias, podemos entender duas noções: a de _isomorfismo_ entre categorias e de _equivalência_. A ideia de isomorfismo, à primeira vista, parece mais apropriada, no entanto, em certas ocasiões, pode ser muito restritiva, enquanto o conceito de equivalência é mais abrangente e adequado para estabelecer o conceito de semelhante ou de essencialmente igual.


Antes de começarmos, devemos relembrar alguns conceitos: uma categoria \\(\mathscr{C} \\) é uma quintupla \\(\mathscr{C} = (Ob_\mathscr{C}, Mor_\mathscr{C}, s, t, \circ) \\), onde \\(Ob_\mathscr{C}\\) e \\(Mor_\mathscr{C} \\) são os objetos e morfismos, respectivamente, da nossa categoria, \\(s,t \\) são as funções _source_ e _target_ que associarão um morfismo a sua saída e sua chegada respectivamente, e finalmente \\(\circ \\) é a composição usual de morfismos.
Um funtor entre duas categorias \\(\mathscr{C} \\) e \\(\mathscr{D} \\) nada mais é que um morfismo de categorias, poderíamos definir um funtor como uma aplicação \\(f: \mathscr{C} \rightarrow \mathscr{D} \\) entre as categorias que leva os objetos.. \\(Ob_{\mathscr{C}} \\) em \\(Ob_{\mathscr{D}} \\), os morfismos \\(Mor_{\mathscr{C}} \\) em \\(Mor_{\mathscr{D}} \\), e que preserva tanto a composição de morfismos quanto suas identidades.


Definiremos um _isomorfismo_ de \\(\mathscr{C} \\) para \\(\mathscr{D} \\) como um funtor \\(F: \mathscr{C} \rightarrow \mathscr{D} \\) para o qual existe um outro funtor \\(G: \mathscr{D} \rightarrow \mathscr{C} \\) tal que:

- \\(G \circ F = 1_{\mathscr{C}} \\);
- \\(F \circ G = 1_{\mathscr{D}} \\).

A partir dessas duas propriedades, podemos notar que este funtor é uma bijeção tanto a nível de objetos, quanto a nível de morfismos.

Exemplos de isomorfismos: a categoria de anéis _**Rng**_ é isomorfa a si mesma por um funtor que envia cada anél a seu anél oposto. Esta mesma categoria de anéis _**Rng**_ é isomorfa à categoria \\(\mathbb{Z} \\)-\\(Alg \\) (categoria de \\(\mathbb{Z} \\) álgebras).

Outra maneira de entender equivalências é por meio do estudo do _esqueleto_ de uma categoria. Diremos que uma categoria \\(\mathscr{C} \\) é _esqueletal_ quando objetos isomorfos desta categoria são idênticos; o esqueleto \\(\mathscr{D} \\) de uma categoria será a maior subcategoria esqueletal de \\(\mathscr{D} \\). 

O conceito de esqueleto é prevalente quando lidamos com equivalências, pois, além de sabermos que toda categoria tem um esqueleto, definimos que duas categorias são equivalentes quando seus _esqueletos são isomorfos_.

Vimos que duas categorias são equivalentes quando existe um isomorfismo entre seus esqueletos, podemos então notar que as ideias de isomorfismo e equivalência estão entrelaçadas, desta maneira, vamos estabelecer uma última definição que tome os requisitos necessários de um isomorfismo, e diretamente construa uma equivalência.

Definiremos uma equivalência entre \\(\mathscr{C} \\) e \\(\mathscr{D} \\) como um funtor \\(F:\mathscr{C} \rightarrow \mathscr{D} \\) que é:

- Fiel, ou seja, para todo \\(a,b\in Ob(\mathscr{C}) \\), existe \\(F_{(x,y)}:hom(x,y) \rightarrow hom(F(x), F(y))\\) injetivo;
- Pleno, isto é, \\(F_{(x,y)} \\) é sobrejetivo;
- Essencialmente sobrejetivo: para todo \\(B\in Ob(\mathscr{D}) \\) existe \\(A\in Ob(\mathscr{C}) \\) tal que \\(F(A) \cong B\\).

Esta noção de equivalência nos mostra uma correspodência entre a ideia de semelhança a nível de objetos (um morfismo bijetivo entre eles) e a nível categórico (bijeções entre esqueletos). 

Enfim, desta vez nos aprofundamos ainda mais na _Teoria de Categorias_, tentando entender quando duas estruturas são semelhantes e como a divisão entre ser parecido ou igual é borrada. Foi um prazer escrever-vos, seguiremos eventualmente com mais teoria de categorias e até a próxima!
