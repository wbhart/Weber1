<style>
  h1, h2, h3, h4, h5, h6 {
    text-align: center;
  }
</style>
<script type="text/javascript">
  MathJax = {
    tex: {
      inlineMath: [ ['$', '$'], ['\\(', '\\)'] ], // Support both $...$ and \(...\) for inline math
      displayMath: [ ['$$', '$$'], ['\\[', '\\]'] ] // Support $$...$$ and \[...\] for display math
    }
  };
</script>
<script type="text/javascript" async
  src="https://cdnjs.cloudflare.com/ajax/libs/mathjax/3.2.2/es5/tex-mml-chtml.js">
</script>

# First Section 

## General Group Theory

### §1. Definition of Groups

In the first volume, we became familiar with the concept of a group through permutations and made important algebraic applications of it. Our next task must now be to read this concept, which is extremely important in all of modern mathematics, in its most general form and to learn the governing laws that apply. We place the following definition at the forefront:

A system $P$ of things (elements) of any kind becomes a group when the following prerequisites are fulfilled:

1. There is a rule given by which from a first and a second element of the system, a completely determined third element of the same system is derived.

One writes symbolically, when $a$ is the first, $b$ the second, $c$ the third element:

$$
ab = c, \quad c = ab
$$

and calls $c$ composed of $a$ and $b$ and $a$ and $b$ the components of $c$.

In this composition, the commutative law is not generally assumed, i.e., $ab$ can be different from $ba$, however

2. the associative law is assumed,

i.e., if $a$, $b$, $c$ are any three elements from $P$, then:

$$
(ab)c = a(bc)
$$
and from this follows, by the method of complete induction, that one always arrives at the same result when, in any sequence of elements from $P$ of finite number, $a$, $b$, $c$, $d$ ..., one first composes two neighboring elements, then again two neighboring ones, and so on, until the whole sequence is reduced to one element, which is denoted by $abcd$ .... So for example:

$$
abcd = (ab)cd = [(ab)c]d = (ab)(cd) \\
= a(bc)d = [a(bc)]d = a[(bc)d] \\
= ab(cd) = (ab)(cd) = a[b(cd)]
$$

3. It is assumed that if $ab = ab\textrm'$ or $ab = a\textrm'b$, then necessarily in the first case $b = b\textrm'$, in the second case $a = a\textrm'$ must hold.

If $P$ encompasses a finite number of elements, then the group is called finite and the number of its elements is its order.

For finite groups, from 1., 2., 3. follows the conclusion:

4. When of the three elements $a$, $b$, $c$ from $P$ any two are given, then one can determine the third in one and only one way so that

$$
ab = c
$$

holds.

Namely, if $a$, $b$ are the given elements, then statement 4. coincides with 1. But if $a$ and $c$ are given, then let the second component $b$ in the composition $ab$ run through the whole system $P$, whose order $= n$. Then according to 1. and 3., $ab$ yields completely different elements of $P$, and since their number $= n$, all elements of $P$, thus also $c$, must occur among them. Similarly one concludes when $b$ and $c$ are given, by letting $a$ run through the whole system $P$.

For infinite groups, this can no longer be concluded in such a way. For infinite groups, therefore, property 4. is additionally included as a requirement in the concept definition.

In the permutation groups considered in the first volume, one will easily recognize the characteristics of the general group concept.

We now draw some completely general conclusions from this definition.

According to 4., for every given $b$ there exists an element $e$ in $P$ that satisfies the condition

$$
eb = b
$$

and this $e$ is independent of $b$; because from (1) follows for every $c$

$$
ebc = bc
$$

and $bc$ can mean any element in $P$ according to 4. Similarly, there exists an element $e\textrm'$ that satisfies for every $b$ the condition

$$
be' = b
$$

This element $e\textrm'$ is not different from $e$; because if we set $b = e\textrm'$ in (1) and $b = e$ in (2), it follows

$$
ee' = e, \quad ee' = e'
$$

therefore
$$
e = e'
$$

This element $e$ changes nothing when it is composed with any elements from $P$, and is called the unity of the group.

In many cases, it can be straightforwardly denoted by "1" without misunderstanding.

For every element $a$ there exists, according to 4., a specific element $a^{-1}$ that satisfies the condition

$$
a^{-1}a = e
$$

From (3), (1), and (2) follows

$$
a^{-1}aa^{-1} = ea^{-1} = a^{-1} = a^{-1}e
$$

and consequently, according to 3.,

$$
aa^{-1} = e
$$

The two elements $a$, $a^{-1}$ are called opposite or reciprocal to each other.

In special cases, for the composition of the elements of a group $P$, the commutative law can also hold, i.e., for any two elements $a$, $b$ of the group it can be

$$
ab = ba
$$

5. Groups that have this property are called commutative groups or also Abelian groups.

When the elements of two groups

$$
a, b, c, d \ldots
$$

and

$$
a', b', c', d' \ldots
$$

correspond to each other mutually and uniquely in such a way that whenever $ab = c$ is true, also $a\textrm'b\textrm' = c\textrm'$ holds, then the groups are called isomorphic, and the evident theorem holds that two groups isomorphic to a third group are isomorphic to each other. Accordingly, one can combine all mutually isomorphic groups into one class of groups, which itself is again a group whose elements are the generic concepts that one obtains when combining the corresponding elements of the individual isomorphic groups into a general concept. The individual mutually isomorphic groups are then to be understood as different representatives of a generic concept.

The properties of groups that can come into consideration are of different kinds. They can either adhere to particular groups and be derived from the nature of the elements from which the group is composed, or also from the nature of the composition law. Or they can adhere to the groups as such and must then be derivable solely from the definition of the group concept. The latter properties are common to all isomorphic groups and can be designated as invariant properties of the group. If a comparison is permitted, one could be reminded of the difference between metric and projective properties in geometry.

To the first kind of properties, which are derived from the particular nature of the elements, belong for example in permutation groups the properties of transitivity and intransitivity, of primitivity and imprimitivity; to the invariant properties belong exchangeability or non\-exchangeability, the order, the divisors and their index, the normal divisors. With these invariant properties, for which it is irrelevant from which representative of a class of isomorphic groups they are derived, we shall first concern ourselves.

## §2. The Divisors of Finite Groups

As we have already seen in the first volume, it is a particularly important question whether a part of the elements of a group itself forms a group again. For this, it is necessary and sufficient that any two elements of this part yield under composition an element belonging to the same part. This smaller group is then called a divisor or factor of the whole group. The unity element "1" forms in every group by itself a group, thus is a divisor in every group.

We restrict ourselves now, as almost always in what follows, to finite groups, and want to assume that

$$
P = 1, a_1, a_2 \ldots a_{n-1}
$$

is a group of order $n$ with elements $a_0 = 1$, $a_1$, $a_2$ ... $a_{n-1}$ and

$$
Q = 1, a_1, a_2 \ldots a_{v-1}
$$

is a divisor of $P$ of order $v$. Every such divisor $Q$ must have the basic properties of a group and thus certainly contains the unity element "1" and with each of its elements $a_1$ also the opposite $a_1^{-1}$. If $v < n$, then we call $Q$ a proper divisor of $P$. If then $b$ is an element of $P$ not contained in $Q$, then the elements

$$
Q_1 = b, a_1b, a_2b \ldots a_{v-1}b
$$

are all different from each other (§1, 3.) and all not contained in $Q$; because if, for example, $a_ib$ were contained in $Q$, then also, since $Q$ is a group, $a_i^{-1}a_ib = b$ would have to be contained in $Q$, contrary to the assumption.

If with $Q$ and $Q_1$ the whole group $P$ is not yet exhausted, then we take one of the still remaining elements, which we can denote with $c$, and form

$$
Q_2 = c, a_1c, a_2c \ldots a_{v-1}c
$$

and convince ourselves easily that the elements of $Q_2$ are all different not only from each other, but also from the elements of $Q$ and $Q_1$ are different. Because if, for example, $a_1c = a_2b$, it would follow that $c = a_1^{-1}a_2b$ would have to be; but $a_1^{-1}a_2$ is contained in $Q$, thus identical with one of the elements $1$, $a_1$, $a_2$ ... $a_{v-1}$, and thus $c$ would be against the assumption contained in $Q_1$. We continue in this way, forming the systems $Q$, $Q_1$, $Q_2$ ... $Q_{\mu-1}$, of which the last

$$
Q_{\mu-1} = g, a_1g, a_2g \ldots a_{v-1}g
$$

may be. Then $P$ must be exhausted by the systems $Q$, $Q_1$, $Q_2$ ... $Q_{\mu-1}$, and it follows, since these systems contain all different elements,

$$
n = v\mu
$$

or the theorem:

1. The order of a group is divisible by the order of each of its divisors. The quotient $\mu = n : v$ shall be called the index of the divisor $Q$.

The systems $Q_1$, $Q_2$ ... $Q_{\mu-1}$ we call, as in the special case of permutation groups, the cosets belonging to $Q$ and denote them by

$$
Q_1 = Qb, \quad Q_2 = Qc \ldots Q_{\mu-1} = Qg
$$

so that we can also symbolically write

$$
P = Q + Qb + Qc + \cdots + Qg
$$

Sometimes we will also denote the whole system $Q$, $Q_1$ ... $Q_{\mu-1}$ ($Q$ itself included) as a system of cosets, and thus call the representation (1) the decomposition of $P$ into a system of cosets.

From the way the cosets are formed, it also follows that, if $b$, $c$ are any two elements from $P$, the two systems $Qb$ and $Qc$ are either completely identical or contain no common element. For if $a_1b = a_2c$, where $a_1$, $a_2$ are two elements from $Q$, then it is also true for every other element $a$ from $Q$:

$$
aa_1b = aa_2c
$$

and when $a$ runs through the whole group $Q$, then, as already noted in §1, each of the two $aa_1$ and $aa_2$ also runs through the whole group $Q$; therefore $Qb$ and $Qc$ are identical.

As in Vol. I, §154, 2. we can also decompose $P$ in the following way into cosets:

$$
P = Q + b^{-1}Q + c^{-1}Q + \cdots + g^{-1}Q
$$
The cosets do not have the characteristics of a group. Because for two elements from $Q_1$ to yield under composition again an element from $Q_1$, something like

$$
a_1b \cdot a_2b = a_3b
$$

would have to hold, thus $a_1ba_2 = a_3$, $b = a_1^{-1}a_3a_2^{-1}$ would have to be. Thus $b$ would be contained in $Q$ contrary to the assumption.

The term coset is therefore only to be understood figuratively.

Two divisors $Q$, $Q\textrm'$ of $P$ always have the element 1 in common. They can however also have other elements in common, and these common elements form a group, which we want to denote with $R$. Because if the elements $a$ and $b$ belong to both $Q$ and $Q\textrm'$, then due to the group character of $Q$ and $Q\textrm'$ the same holds for the composition $ab$; thus $R$ is a group. We call this common group the greatest common divisor of $Q$ and $Q\textrm'$ or also, with a geometric analogy, the intersection of $Q$ and $Q\textrm'$. Similarly, it follows that the elements that are common to any number of divisors of $P$ form a group, which we likewise denote as the greatest common divisor or the intersection of all these groups.

In every group we can form divisors according to the following procedure.

A divisor is always the unity element by itself.

If we denote the repeated composition of an element with itself through powers (with $a^0$ the unity element), then the sequence of elements

$$
1, a, a^2, a^3 \ldots
$$

which all belong to the group $P$, cannot contain all different elements. If thus the first element that recurs for the second time is

$$
a^µ = a^{µ+α}
$$

then it follows that $a^α = 1$ must be, and that $α$ is the smallest positive number that satisfies this condition. It is then, if $m = qα$ is any multiple of $α$, $a^m = 1$ and conversely: whenever $a^m = 1$, $m$ must be divisible by $α$; because otherwise one could set $m = qα + α\textrm'$, where $α\textrm'$ is positive and smaller than $α$, and it would be $a^{α\textrm'} = 1$, contrary to the assumption, that $α$ is the smallest positive exponent for which $a^α = 1$. It is always and only then

$$
a^µ = a^{µ'}
$$

when $µ \equiv µ\textrm'$ (mod $α$), and herein the exponents can also be negative, where $a^{-r}$ means the $r$th power of the element $a^{-1}$ or the element opposite to $a^r$.

The sequence

$$
A = 1, a, a^2 \ldots a^{α-1}
$$

then contains $α$ different elements of $P$, whereby all powers of $a$ are represented. The elements $A$ clearly form a group of order $α$, because the exponents simply add under composition. This group is a divisor of $P$ and thus $α$ is a divisor of $n$.

Thus we have for every element $a^α = 1$.

The group $A$ is called the period of the element $a$ and $α$ is also called the order of the element.

## §3. Normal Divisors of a Group

If $P$ is a group as above and $Q$ a divisor of $P$, further $b$ is an element of $P$ not contained in $Q$, then the coset $Qb$ is not a group. However, the system $b^{-1}Qb$, or written out in full

$$
1, b^{-1}a_1b, \quad b^{-1}a_2b \ldots b^{-1}a_{v-1}b
$$

certainly forms a group, because

$$
b^{-1}a_1b \cdot b^{-1}a_2b = b^{-1}a_1a_2b
$$

is true, and this group is isomorphic with $Q$. The group $b^{-1}Qb$ is called the group transformed by $b$. If $b$ itself belongs to $Q$, then $b^{-1}Qb$ is identical with $Q$. If one takes for $b$ the different elements of $P$, one obtains a whole series of such groups, which we call the divisors conjugate to $Q$ of $P$ or also briefly conjugate groups.

It can happen that all conjugate divisors are identical with each other. We have already seen in the permutation groups that this case is of particular importance, and thus now introduce generally the following definition:

If $Q$ is a divisor of $P$ that is identical with all of its conjugate divisors, then $Q$ is called a normal divisor of $P$.

The unit element formed by Element 1 is a normal divisor of every group. We also obtain a normal divisor in the largest common divisor $R$ of all divisors conjugate with any divisor $Q$ of $P$.

For it has already been proved above that $R$, as the intersection of several divisors of $P$, is a group.

If now
$$
Q, Q', Q'' \ldots
$$
are the divisors of $P$ conjugate to $Q$ and $b$ is any element of $P$, then the system of groups
$$
b^{-1}Qb, b^{-1}Q'b, b^{-1}Q''b \ldots
$$
is not different from system (1). But if $R$ is the intersection of groups (1), then $b^{-1}Rb$ is the intersection of (2), and consequently $R$ is identical with $b^{-1}Rb$, i.e., $R$ is a normal divisor of $P$.

If $N$ is a normal divisor of any group $P$ and $b$ is any element in $P$, then
$$
b^{-1}Nb = N \text{ or } Nb = bN
$$

If $P$ is of degree $n$, $N$ of degree $v$ and of index $\mu$, thus $n = \mu v$, then we can choose the $\mu$ elements $1, b_1, \ldots b_{\mu-1}$ so that the decomposition of $P$ into cosets yields
$$
P = N + Nb_1 + \cdots + Nb_{\mu\-1}
= N + b_1N + b_2N + \cdots + b_{\mu\-1}N
$$
Thus we have
$$
N, N_1 = Nb_1 = b_1N, N_2 = Nb_2 = b_2N \ldots,
N_{\mu\-1} = Nb_{\mu\-1} = b_{\mu\-1}N
$$
as the system of cosets.

If $a$ is any element in $N$, then $Na$ is identical with $N$, thus $Nab$ is also identical with $Nb$, and since every element $c$ of $P$ occurs in $N$ or in one of its cosets, thus is contained in the form $ab_k$, $Nc$ must coincide with one of the systems (4).

We mention also the following theorem, whose correctness follows immediately from the isomorphism of transformed groups:

If $Q$ is a divisor of $P$, $R$ a divisor of $Q$, then if $Q\textrm'$ and $R\textrm'$ are transformed from $Q$ and $R$ by the same element of $P$, $R\textrm'$ is also a divisor of $Q\textrm'$, and if $R$ is a normal divisor of $Q$, then $R\textrm'$ is also a normal divisor of $Q\textrm'$.

Composition of Parts

If $A$ and $B$ are any two series of elements from a group $P$ (groups or not), then by the symbolic product $AB$ we will understand the totality of all elements that one obtains when multiplying each element $a$ of $A$ with each element $b$ of $B$ according to the composition rule valid in $P$ to form $ab$. We will call this type of combination of $A$ and $B$ to $AB$ the composition of parts (of $P$).

We distinguish here between a part and a divisor of $P$, so that a divisor should always be a group, which is not necessary for a part.

One can similarly compose three or more parts $A$, $B$, $C \ldots$ of $P$, and the associative law applies to the composition of parts, as follows immediately from the fact that this law holds in $P$. Accordingly, the meaning of a composite $ABC \ldots$ is uniquely determined.

In the composition $AB$, any of the parts $A$, $B$ can also consist of a single element, and then the notation $AB$ coincides with the notation used above for cosets.

For the composition of parts, the following theorems hold:

1. The necessary and sufficient condition for a part $A$ of $P$ to be a group is contained in the equation

$$
AA = A
$$

For this equation says nothing other than that when $a$ and $a\textrm'$ are contained in $A$, $aa\textrm'$ also belongs to $A$, thus that $A$ is a group.

2. Through the two equations

$$
AA = A,
AB = BA
$$

where $A$ is a specific part, $B$ can be any part of $P$, it is stated that $A$ is a normal divisor of $P$.

For according to (2), $A$ is a divisor of $P$ and according to (3) for each element $b$ of $P$
$$
b^{-1}Ab = A
$$
i.e., $A$ is a normal divisor.

3. If $A$ and $B$ are two divisors of $P$ (groups), then one of the two equations

$$
AB = A, BA = A
$$

is the necessary and sufficient condition for $B$ to be a divisor of $A$.

For if $B$ is a group and a divisor of group $A$, and if $a$ is in $A$, $b$ in $B$ and thus also in $A$ contained, then $ab$ is also contained in $A$. $A$ thus contains every element of $AB$.

If, however, secondly $B$ as a group also contains the element 1, then $AB$ also contains every element of $A$, and thus $AB$ is identical with $A$.

Similarly, one sees that $BA$ is identical with $A$. Conversely, it follows from each of equations (4), since $A$ as a group contains the unit element, that every element of $B$ is contained in $A$, thus $B$ is a divisor of $A$.

4. In the composition of parts, the system of cosets to a normal divisor of $P$ itself forms a group, in which the normal divisor $N$ forms the unit element, and

$$
Nb, Nb^{-1}
$$

are inverse elements.

For if $N$ is a normal divisor of $P$ and
$$
N, N_1 = Nb_1, N_2 = Nb_2, \ldots
$$
is the system of cosets, then
$$
N_hN_k = Nb_hNb_k.
$$
Due to the property of normal divisors, $N$ is commutable with any $b$, thus $b_hN = Nb_h$, and consequently
$$
N_hN_k = N\!b_hb_k.
$$

Because $b_hb_k$ is contained in $P$, $Nb_hb_k$ is identical with one of the cosets (5), and since $NN = N$ can be set (according to 1.), it follows, when we set $Nb_hb_k = N_i$,
$$
N_hN_k = N_i.
$$

With this, property §. 1, 1. of groups for the composition of cosets is proven. That also §. 1, 2., namely the associative law holds, we have already emphasized. Thus it remains to prove §. 1, 3., namely that when
$$
N_hN_i = N_kN_l
$$
is set, and $N_h = N_k$ is true, also $N_i = N_l$, and when $N_i = N_l$ is true, also $N_h = N_k$ must be true.

According to representation (5) we can however write (7) in the double way:
$$
Nb_hb_i = Nb_kb_l\\
b_hb_iN = b_kb_lN.
$$

If now $N_i = N_l$, so we can also assume $b_i = b_l$, and obtain from (8) through composition with $b_i^{-1}$
$$
Nb_h = Nb_k;
$$
and when $Nb_h = Nb_k$ is true, we take $b_h = b_k$ and obtain from (8) through composition with $b_h^{-1}$
$$
b_iN = b_lN,
$$
thus also $N_i = N_l$.

With this it is thus proven that the system of cosets through the composition of parts forms a group, in which the normal divisor $N$ is the unit element, follows immediately from 1., because accordingly
$$
NN_k = NNb_k = N_k
$$
is true. And because $Nb_kNb_k^{-1} = Nb_kb_k^{-1} = N$ is true, $Nb_k$ and $Nb_k^{-1}$ are inverse elements.

The group of magnitudes $N_i$, whose existence is thus hereby proven, we call the group of cosets or the complementary group to $N$ with respect to $P$. We denote it following Hölder with $P/N$. The degree of the complementary group is equal to the index of group $N$.

We mention at the conclusion of these considerations another theorem about normal divisors.

5. If $N$ is a divisor of $P$, $N\textrm'$ a divisor of $N$ and simultaneously a normal divisor of $P$, then $N\textrm'$ is also a normal divisor of $N$.

This is self\-evident, because for every element $b$ of $P$, $b^{-1}N\textrm'b = N\textrm'$ is true, and because every element of $N$ is also an element of $P$.

However, one must not conclude conversely that, when $N$ is a normal divisor of $P$, $N\textrm'$ a normal divisor of $N$, $N\textrm'$ must also be a normal divisor of $P$.

Multi\-stage Isomorphism

If as above $N$ is a normal divisor of $P$ of degree $v$ and index $\mu$, thus $n = \mu v$, then the complementary group $P/N$ to $P$ is of degree $\mu$. We want to denote this or an isomorphic group with $Q$ and denote its elements, which correspond to the cosets $N$, $Nb_1$, $Nb_2 \ldots$, with $A$, $B$, $C \ldots$. To each of these elements correspond $v$ elements of group $P$, namely
  to element $A$ the elements $a$, $a_1 \ldots a_{v-1}$
  to element $B$ the elements $b$, $b_1 \ldots b_{v-1}$
  $\ldots \ldots \ldots \ldots \ldots \ldots$

This correspondence is such that each composite element $ab$ corresponds to the composite element $AB$. For the elements $A$ and $B$ correspond to the cosets $Na$ and $Nb$, and it is, because $N$ is a normal divisor,
$$
NaNb = Nab
$$

Thus here with the composition of $A$, $B \ldots$ on one side and $a$, $b \ldots$ on the other side the same law applies as with isomorphic groups (§. 1), only with the difference that to each element $A$ not just one element $a$, but several correspond. This fact gives rise to extend the concept of isomorphism, as happens through the following definition:

One calls a group $P$ with elements $a$, $b$, $c \ldots$ (multi\-stage) isomorphic with a group $Q$ with elements $A$, $B$, $C \ldots$ when both groups can be related to each other such that to each of the elements $A$, $B$, $C \ldots$ one or more of the elements $a$, $b$, $c \ldots$ correspond, and specifically such that each element of $Q$ corresponds to one and only one of the elements of $P$, and when $a$ and $b$ correspond to $A$ and $B$, $ab$ corresponds to element $AB$.

It lets itself first prove that to each of the elements $A$, $B$, $C \ldots$ an equal number of elements $a$, $b$, $c \ldots$ corresponds and that thus the degree of $Q$ is a divisor of the degree of $P$. For let $A$ be the unit element in $Q$, to which the elements $a$, $a_1 \ldots a_{v-1}$ in $P$ may correspond. These latter elements must then form a group of degree $v$ that we want to denote with $N$ because according to the definition of isomorphism the element $aa_1$ must correspond to element $AA = A$. If then $b$ is an element of $P$ corresponding to element $B$, then again all elements $Nb$ must correspond to the same element $B$ from $Q$. For each $a$ must correspond to element $AB = B$. If $b_1$, $b$ are two elements corresponding to element $B$, then $b_1b^{-1} = a$ corresponds to element $A$, and thus is in $N$ contained, thus $b_1 = ab$ in $Nb$ contained. Through $Nb$ thus all elements that correspond to element $B$ are exhausted, and to each element of $Q$ correspond $v$ elements of $P$. The isomorphism is called $v$\-stage. Each element $b^{-1}ab$ corresponds however likewise to the unit element $A$ and thus is $b^{-1}Nb = N$, i.e. $N$ is normal divisor of $P$, and $Q$ is one\-stage isomorphic with $P/N$.

We see thus that there is no other multi\-stage isomorphism than that between the complementary group of a normal divisor and the total group. One could however expand the concept of isomorphism further such that one calls two groups that are $\mu$- and $v$\-stage isomorphic to a third group, $\mu$-$v$\-stage isomorphic to each other. By far the most important is the one\-stage isomorphism, which we therefore denote simply as isomorphism, while a multi\-stage isomorphism should always be made recognizable through an addition.

Composition Series and Jordan\textrm's Theorem

A group $P$ is called simple when it has no normal divisor besides itself and unity; composite, when other normal divisors are present.

A normal divisor that has no other normal divisor above itself, which thus is not part of another proper normal divisor of $P$, is called a greatest normal divisor of $P$. If $P_1$ is a greatest normal divisor of $P$, $P_2$ of $P_1$, $P_3$ a greatest normal divisor of $P_2$ and so on, then the series of groups
$$
P, P_1, P_2, P_3 \ldots 1,
$$
which necessarily ends with the group 1 formed from the unit element alone, is called a composition series of group $P$.

We want to denote the degrees of groups (1) with $n$, $n_1$, $n_2$, $n_3 \ldots 1$, and the quotients $n : n_1$, $n_1 : n_2$, $n_2 : n_3 \ldots$, thus the indices of $P_1$ with respect to $P$, $P_2$ with respect to $P_1$ and so on with $v_1$, $v_2$, $v_3 \ldots$ The series of all these numbers
$$
v_1, v_2, v_3 \ldots
$$
we call the index series of group $P$.

The greatest normal divisors $P_1$, $P_2$, $P_3 \ldots$ can for a given group $P$ in general be selected in several different ways, and accordingly the degree numbers $n_1$, $n_2$, $n_3 \ldots$ and the indices $v_1$, $v_2$, $v_3 \ldots$ can also be different.

But the following beautiful and important theorem by C. Jordan holds:

1. However a group P\textrm's composition series may be chosen, the index series is always the same, disregarding the arrangement.

The proof rests on the consideration of complementary groups introduced in the previous paragraph.

Let Q and Q_1 be normal divisors of P and simultaneously Q_1 a divisor (thus according to §4, 5. a normal divisor) of Q.

Then the following theorem holds:

1. The group Q/Q_1 is a normal divisor of the group P/Q_1, and the index of Q/Q_1 with respect to P/Q_1 equals the index of Q with respect to P.

To recognize its correctness, one only needs to consider more precisely the formation method of the individual groups.

Let n, q, q_1 be the orders of P, Q, Q_1 and

$$
n = v q, q = v_1 q_1, n = \mu q_1, \mu = v v_1
$$

One decomposes Q into cosets in that one sets, when $b_1, b_2 \ldots b_{v_1-1}$ are suitably chosen elements in Q,

$$
Q = Q_1 + Q_1b_1 + ... Q_1b_{v_1-1}
$$

The elements of the group Q/Q_1 are

$$
Q_1, Q_1b_1, ... Q_1b_{v_1-1}
$$

When we decompose P into cosets with respect to Q_1, certainly the elements (5) appear among them, and consequently Q/Q_1 is a divisor of P/Q_1.

It remains to be proven that this divisor is a normal divisor.

Let us denote with a any element of P, then all elements of P/Q_1 are in the form Q_1a, and we thus only need to show that, when b is any element in Q, every element

$$
Q_1 a^{-1}Q_1 b Q_1 a
$$

in Q/Q_1, i.e. in the form Q_1b, is contained.

This follows immediately from

$$
Q_1 a^{-1}Q_1 b Q_1 a = Q_1 a^{-1}b a
$$

because along with b, a⁻¹ba also appears in Q (since Q is a normal divisor of P). And that the determination of indices is correct is shown by the counting. Because the orders of P/Q_1 and Q/Q_1 are vv_1 and v_1, thus the index v.

Additionally, the following theorem holds:

2. If Q_1 is a normal divisor of P of order q_1, and the group P/Q_1 itself has a divisor M of order m, then P has a divisor Q of order q = mq_1. Simultaneously, Q_1 is a normal divisor of Q and M = Q/Q_1. If M is a normal divisor of P/Q_1, then Q is also a normal divisor of P.

Let μ be the index of Q_1 with respect to P, and let P be decomposed into cosets:

$$
P = Q_1 + Q_1e_1 + Q_1e_2 ... + Q_1e_{μ-1}
$$

so that e_1, e_2 ... e_{μ-1} are suitably chosen elements in P and

$$
Q_1, Q_1e_1, Q_1e_2 ... Q_1e_{μ-1}
$$

are the elements of P/Q_1. When now a divisor M is contained in the group P/Q_1, this must consist of a portion of the elements (9), perhaps of

$$
Q_1, Q_1b_1, Q_1b_2 ... Q_1b_{n\-1}
$$

and when this system should form a group, then for any two elements $b_{h}, b_{k}$ the product

$$
Q_1b_{h}Q_1b_{k} = Q_1b_{h}b_{k}
$$

must be contained again in (10), thus $= Q_1b_{n}$. When therefore the system 1, b_1, b_2 ... b_{n-1} is designated with B, then according to the method of composition of parts, the relation (11) can be written as:

$$
Q_1BQ_1B = Q_1B
$$

and thus it states according to §4, 1., that the elements contained in

$$
Q = Q_1B
$$

form a group of P that contains the group Q_1 as a divisor and is itself a divisor of P. That Q_1 is a normal divisor of Q follows from §4, 5., since Q_1 as normal divisor of P is presupposed, and from the representation (10) of group M it follows that M = Q/Q_1.

It remains to be shown that when M is a normal divisor of P/Q_1, then Q is also a normal divisor of P. This follows thus:
If e is any element in P and $Q_1b_{k}$ an element in M, then from the assumption that M is a normal divisor of P/Q_1 follows:
$$
Q_1e^{-1}Q_1b_{k}Q_1e = Q_1b_{h}
$$

which we can also express through the formula

$$
Q_1e^{-1}Q_1BQ_1e = Q_1B
$$

according to the composition of parts. Since now Q_1 is a normal divisor of P, Q_1 can be interchanged with each of the other factors, so that from (14) follows:

$$
e^{-1}Q_1Be = Q_1B
$$

or

$$
e^{-1}Qe = Q
$$

whereby it is expressed that Q is a normal divisor of P.

From Theorems 1. and 2. follows the corollary:

3. A normal divisor Q of P is a greatest normal divisor if and only if the complementary group P/Q is simple.

When Q and Q\textrm' are two normal divisors of P, then the symbolic product QQ\textrm' is also a normal divisor.

Because it is, since Q is a normal divisor

$$
QQ' = Q'Q
$$

thus

$$
QQ'QQ' = QQQ'Q' = QQ'
$$

and this is according to §4, 1. the characteristic that QQ\textrm' is a group. That it is a normal divisor of P follows then according to §4, 2. from

$$
QQ'B = QB Q' = BQQ'
$$

when B is any part of P.

If now Q is a greatest normal divisor of P, and Q\textrm' different from Q, then QQ\textrm' is a normal divisor of P, that contains both Q and Q\textrm' and is thus different from Q. Consequently, since there exists no normal divisor of P besides P itself,

$$
QQ' = P
$$

and similarly must also

$$
Q'Q = P
$$
be true. These theorems hold when just one of the two groups Q, Q\textrm' is a greatest normal divisor of P. We now assume that they both have this property, and understand by R the greatest common divisor of Q and Q\textrm'. This group R is then a normal divisor of P as well as of Q and Q\textrm'. Because if a is any element in P, and e in Q as well as in Q\textrm', then $a^{-1}ea$ is in Q and in Q\textrm', thus also contained in R. Thus a⁻¹Ra = R, and R is a normal divisor of P and therefore a normal divisor of Q and of Q\textrm' (§4, 5.). To decompose Q into cosets of R, we choose a suitable system of elements 1, b_1, b_2, b_3 ... in Q, so that R, Rb_1, Rb_2, Rb_3 ... all become different from each other and set

$$
Q = R + Rb_1 + Rb_2 + Rb_3 + ...
$$

which we can also, when we

$$
B = 1, b_1, b_2, b_3 ...
$$

set, briefly denote with

$$
Q = RB
$$

Now according to (13) Q\textrm'Q = P, thus also

$$
P = Q'RB = Q'B
$$

or

$$
P = Q' + Q'b_1 + Q'b_2 + Q'b_3 ...
$$

The cosets

$$
Q', Q'b_1, Q'b_2, Q'b_3 ...
$$

are however all different from each other. Because if perhaps

$$
Q'b_2 = Q'b_1
$$

it would follow, since Q\textrm' contains the unity, that there exists an element e in Q\textrm' such that

$$
b_2 = eb_1
$$

would be true. This element e is however equal to b_2b_1⁻¹, and thus, since the b are contained in Q, likewise in Q and thus also in R contained. But then Rb_2 = Rb_1 would also be true, which contradicts the assumption.

From this we can form the elements of the group complementary to R with respect to Q and of the group complementary to Q\textrm' with respect to P. We obtain these two groups

$$
Q/R = R, Rb_1, Rb_2, Rb_3 ...
$$

$$
P/Q' = Q', Q'b_1, Q'b_2, Q'b_3 ...
$$

From this one easily recognizes that these groups are not only of the same order, but that they are isomorphic. Because simultaneously

$$
Rb_1Rb_2 = Rb_1b_2
$$

and

$$
Q'b_1Q'b_2 = Q'b_1b_2
$$

Similarly, one can also conclude that the two groups Q\textrm'/R, P/Q are isomorphic.

The groups P/Q and P/Q\textrm' are, since Q, Q\textrm' are greatest normal divisors, according to 3) simple, and consequently the isomorphic groups Q\textrm'/R and Q/R are also simple, and thus we have the theorem:

4. If Q and Q\textrm' are two different greatest normal divisors of P and R is the intersection of Q and Q\textrm', then R is a greatest normal divisor of both Q and Q\textrm', and the index of R with respect to Q equals the index of Q\textrm' with respect to P.

With this we have gained the foundation to very simply prove the theorem about the constancy of the index series.

For better overview, we write the different composition series to be compared in such a way that we write the index of each member with respect to the preceding member under the member.

Accordingly, any two given composition series of P with their corresponding indices may be the following:

$$
P, Q, Q_1, Q_2, Q_3 ...
$$

$$
v, v_1, v_2, v_3 ...
$$

$$
P, Q', Q'_1, Q'_2, Q'_3 ...
$$

$$
v', v'_1, v'_2, v'_3 ...
$$

Let now R be the intersection of Q and Q\textrm', and μ and μ\textrm' be the indices of R with respect to Q and Q\textrm'. Due to the isomorphism of the groups P/Q and Q\textrm'/R, we have μ\textrm' = v, and for the corresponding reason μ = v\textrm'. We form a composition series of R with its corresponding index series

$$
R, R_1, R_2, R_3 ...
$$

$$
μ_1, μ_2, μ_3 ...
$$

and since R is now a greatest normal divisor of Q and of Q\textrm', we can form from this two new composition series of P, namely

$$
P, Q, R, R_1, R_2, R_3 ...
$$

$$
v, v', μ_1, μ_2, μ_3 ...
$$

$$
P, Q', R, R_1, R_2, R_3 ...
$$

$$
v', v, μ_1, μ_2, μ_3 ...
$$

The two composition series (26) and (27) of P thus have the same index series.

If we now assume that the theorem to be proven has already been proven correct for groups whose order ≦ ½n (where n denotes the order of P), then it follows that all index series of Q, whose order is indeed a proper divisor of n and thus at most = ½n, agree with each other, thus the series

$$
v_1, μ_1, μ_2, μ_3 ...
$$

$$
v'_1, v'_2, v'_3, v'_4 ...
$$

agree, disregarding the arrangement. Similarly, the index series of Q\textrm'

$$
v, μ_1, μ_2, μ_3 ...
$$

$$
v_1, v'_2, v'_3, v'_4 ...
$$

agree. Thus the two index series of P also agree

$$
v, v_1, v_2, v_3, v_4 ...
$$

$$
v', v'_1, v'_2, v'_3, v'_4 ...
$$

with each other, since the first agrees with v, v\textrm', μ_1, μ_2, μ_3 ..., the second with v\textrm', v, μ_1, μ_2, μ_3 ... .

For groups of order 2, which have only the one normal divisor 1, the theorem is evident, and thus it is proven generally through complete induction.

If in two composition series of P, which we now want to represent with their index series as

$$
P, P_1, P_2, P_3 ... P_{u-1}, 1
$$

$$
j_1, j_2, j_3 ... j_{u-1}, j_u
$$

$$
P, P'_1, P'_2, P'_3 ... P'_{s-1}, 1
$$

$$
j'_1, j'_2, j'_3 ... j'_{s-1}, j'_s
$$

a common member $P_r = P\textrm'_s$ occurs, then the theorem about the constancy of the index series also holds for the group $P_r = P\textrm'_s$, and from this it follows first that $s = r$ must be true, and that the index series $j_{r+1}, j_{r+2} ... j_u$ and $j\textrm'_{r+1},j\textrm'_{r+2} ... j\textrm'_u$, must agree, disregarding the ordering. Consequently, the preceding parts of the index series

$$
j_1, j_2 ... j_r \text{ and } j'_1, j'_2 ... j'_r
$$

must also agree.

§. 7.
Further Theorems about Composition Series.

Many theorems hold for composition series, of which we will here derive the most important ones.

II. If $P_r$ is any normal divisor of P, then there exists a composition series of P in which $P_r$ occurs.

If $P_r$ is a greatest normal divisor of P, then we can set P_r = P_1 and continue the composition series arbitrarily from there. If however $P_r$ is not a greatest normal divisor of P, then we search for a greatest normal divisor P_1, which we denote with P_1. Then $P_r$ is a normal divisor of P_1. If it is a greatest one, then we set P_r = P_2 and continue the composition series arbitrarily. If however $P_r$ is still not a greatest normal divisor of P_1, then we search for a greatest normal divisor of P_1 that contains $P_r$ and continue in this way, until we finally reach $P_r$, which must occur after a finite number of steps. When we then append a composition series of $P_r$, we have a composition series of P in which $P_r$ occurs, as the theorem requires.

In a composition series of a group P, by definition, each member is a normal divisor of each preceding one. The first member P_1 and the last member 1 are simultaneously normal divisors of P itself. For the intermediate P_2, P_3, ..., this will generally not be the case. In the composition series there are thus certain distinguished members, which are simultaneously normal divisors of P itself (they play a special role). From this we derive in the following still another important theorem.

Suppose Q is a member of a composition series of P that is simultaneously a normal divisor of P, while the following member $Q_1$ is not a normal divisor of $P$. Then among the groups $a^{-1} Q_1 a$ conjugate to $P$, there exist several different ones, which we want to denote as:
$$
Q_1, Q'_1, Q''_1, Q'''_1 \ldots
$$

The greatest common divisor $R$ of all these groups is again a normal divisor of $P$.

Now all the groups (1) are greatest normal divisors of $Q$, as follows from the final theorem of §3, since $Q_1, Q\textrm'_1$ are isomorphic with $a^{-1} Q a, a^{-1} Q_1 a$, while $Q$ as a normal divisor of $P$ with $a^{-1} Q a$ is identical. We can therefore allow each of the groups (1) with the same index $v$ to follow in the composition series for $Q$.

If now $Q_2$ is the greatest common divisor of $Q_1, Q\textrm'_1$ (thus $Q_1$ different), then according to §6, 4., $Q_2$ is a greatest normal divisor of $Q_1$ and $Q\textrm'_1$, whose index is likewise $v$. Thus we can continue the composition series of $Q$ in both of the following ways:

$$
Q, Q_1, Q_2, \quad Q\; Q'_1\; Q_2\\
\;\;\quad v\quad v\quad\quad\quad v \quad v
$$

We now want to generalize the law expressed here and prove it by complete induction.

When $Q_2$ is not yet equal to $R$, we add to $Q_1, Q\textrm'_1$ a third group $Q\textrm'\textrm'_1$ from the series (1) so that the intersection $Q_3$ of $Q_2, Q\textrm'_1, Q\textrm'\textrm'_1$ becomes a proper divisor of $Q_2$, and continue in this way until we reach the greatest common divisor $R$ of all groups (1).

Let therefore:

$Q_2$ be the intersection of $Q_1, Q\textrm'_1$
$Q_3$ be the intersection of $Q_1, Q\textrm'_1, Q\textrm'\textrm'_1$
$\ldots$
$Q_r$ be the intersection of $Q_1, Q\textrm'_1, Q\textrm'\textrm'_1 \ldots Q_1^{(r-1)}$

and the arrangement of the groups $Q_1, Q\textrm'_1 \ldots Q_1^{(r-1)}$ be chosen such that of the groups $Q_1, Q_2 \ldots Q_r$ each is a proper divisor of the preceding one. This arrangement can be continued as long as $Q_r$ is not equal to $R$.

We want to prove that we can choose the composition series of $P$ such that 
$$
Q, Q_1, Q_2 \ldots R,\\\quad v \quad v \quad v
$$
therein occurs, and that the indices in this part of the series are all equal to $v$. 

The claim is correct for $r = 2$, and we prove it generally by complete induction, under the assumption that it has already been proven for $r$.

If $Q_r$ is not equal to $R$, then we choose $Q_1^{(r)}$ so that $Q_{r+1}$ is the intersection of $Q_1, Q\textrm'_1 \ldots Q_1^{(r-1)}, Q_1^{(r)}$, and furthermore denote the intersection of $Q_r, Q\textrm'_1 \ldots Q_1^{(r-1)}, Q_1^{(r)}$ with $Q\textrm'_r$. Then $Q\textrm'_r$ is different from $Q_r$, and $Q_{r+1}$ is the intersection of $Q_r$ and $Q\textrm'_r$. Now according to assumption (4) we have two corresponding pieces of the composition series with the constant index sequence $v$

$$
Q, Q_1 \ldots Q_{r\-1} Q_r,\\
Q, Q_1 \ldots Q_{r\-1} Q'_r;
$$

for the second of these series is formed exactly like the first according to prescription (3), only that $Q_1^{(r)}$ has taken the place of $Q_1^{(r-1)}$. According to theorem §6, 2., therefore $Q_{r+1}$ is a greatest normal divisor of both $Q_r$ and $Q\textrm'_r$, and both with index $v$, and thus follows what was to be proven, that the composition series can be continued as:

$$
Q, Q_1 \ldots Q_{r-1}, Q_r, Q_{r+1},
$$

and that the newly added index is likewise $v$.

We can continue this until we reach the group $R$ and obtain a piece of the composition series

$$
Q, Q_1, Q_2 \ldots R,\\
\quad v \quad v \quad v
$$

whose last member $R$ is again a normal divisor of $P$ and in which all indices agree.

If we continue the composition series from $R$, the index can change; it can however from there on be kept equal again until one reaches another normal divisor of $P$.

Thus the following theorem is proved:

III. One can arrange the composition series of $P$ with its index series

$$
P, P_1, P_2, P_3 \ldots\\
j_1, j_2, j_3 \ldots
$$

in such a way that whenever a change occurs in the index series, thus $j_{r+1}$ is different from $j_r$, $P_r$ is a normal divisor of $P$.

§8.
Metacyclic Groups.

In §176 of the first volume, we defined metacyclic groups for permutation groups and learned about their significance for solving equations. However, the concept is independent of the special significance of the group elements, and we therefore now define generally:

A group whose index series consists entirely of prime numbers shall be called a metacyclic group.

For these groups, there holds an important theorem for applications to algebra, which is however independent of these applications and which we therefore derive here. The theorem states:

IV. A metacyclic group has a commutative normal divisor different from the unit group.

If $P$ is a metacyclic group and

$$
P, P_1, P_2 \ldots P_{n-1}, 1\\
\quad j_1, j_2 \ldots j_{n-1}, j_n
$$

is the composition series, whose index series $j_1, j_2 \ldots$ consists entirely of prime numbers, then $P_{n-1}$ is in any case a commutative group; for if $\pi$ is any element different from 1 from $P_{n-1}$, then the powers

$$
1, \pi, \pi^2 \ldots \pi^{j_n-1}
$$

(because $j_n$ is a prime number) are all different from each other and thus make up the whole group $P_{n-1}$; the cyclic group (2) is however certainly commutative, because for any two exponents $h$, $k$

$$
\pi^h\pi^k = \pi^k\pi^h = \pi^{h+k}
$$

holds. At the same time, according to the definition of the composition series, $P_{n-1}$ is a normal divisor of $P_{n-2}$.

We therefore now assume that we have a commutative normal divisor $Q_r$ different from the unit of any group $P$ of series (1) and furthermore assume that when there are several divisors of $P_r$ of the nature of $Q_r$, that one of possibly lowest degree is taken for $Q_r$.

When we then demonstrate how one can derive from $Q_r$ a commutative normal divisor $Q_{r-1}$ of $P_{r-1}$ that also contains $Q_r$, we can continue this process until we have arrived at a commutative normal divisor $Q$ of $P$ itself, as our theorem requires.

If we choose any element $\gamma$ from $P_{r-1}$ which is not contained in $P_r$, then since $P_r$ is a normal divisor of $P_{r-1}$, we have

$$
\gamma P_r = P_r \gamma,
$$

and if therefore $h$ is the lowest exponent for which $\gamma^h$ is contained in $P_r$, then $h$ is greater than 1 and

$$
\gamma^h P_r = P_r \gamma^h,
$$

and the elements contained in the system of subgroups

$$
P_r, \gamma P_r, \gamma^2 P_r, \ldots \gamma^{h-1} P_r
$$

which are all different from each other, form a group whose degree, if the degree of $P_r$ is denoted by $p_r$, equals $hp_r$. This group (5) is also a divisor of $P_{r-1}$ and consequently $hp_r$ must be a divisor of $p_{r-1} = j_r p_r$, and $h$ is a divisor of $j_r$. But since $j_r$ is a prime number, $h$ must equal $j_r$, and through (5) the whole group $P_{r-1}$ is exhausted:

$$
P_{r\-1} = P_r + \gamma P_r + \gamma^2 P_r + \cdots + \gamma^{j_r\-1} P_r
$$

We now consider the system of transformed groups

$$
\gamma^{-1} Q_r \gamma,
$$

where $\gamma$ runs through all elements of $P_{r-1}$.

These groups are all isomorphic with each other and are thus commutative just like $Q_r$. They are all contained in $P_r$, and are, since $\gamma^{-1} P_r \gamma = P_r$, according to the final theorem of §3 normal divisors of $P_r$.

If all groups (7) are identical with each other, then $Q_r$ is a normal divisor of $P_{r-1}$, and we achieve our purpose of determining $Q_{r-1}$ simply by taking $Q_r$ itself, or, if there should still exist a commutative normal divisor of lower degree than $Q_r$ of $P_{r-1}$, by taking this latter for $Q_{r-1}$.

In the other case, we want to denote the groups (7) that are different from each other by

$$
Q_r, Q'_r, Q''_r \ldots
$$

and derive from them a group

$$
R = (Q_r, Q'_r, Q''_r \ldots)
$$

which shall be defined as the smallest group that contains each of the groups (8) as a divisor, and which we can denote as the smallest common multiple of the groups $Q_r, Q\textrm'_r, Q\textrm'\textrm'_r \ldots$

That there exists one and only one such group $R$, and that every group that is divisible by all $Q_r, Q\textrm'_r, Q\textrm'\textrm'_r \ldots$ must also be divisible by $R$, is easy to see. For firstly there exist finite groups, e.g. the group $P_r$, that contain all groups (8) as divisors, and secondly, when two groups $R$, $R\textrm'$ contain all these groups, the same applies to their intersection $R$ and $R\textrm'$. If therefore $R\textrm'$ is of possibly lowest degree, this intersection must be identical with $R$, and $R$ is thus a divisor of $R\textrm'$. If $R\textrm'$ is also of possibly lowest degree, then $R\textrm'$ is not different from $R$.

For this group $R$ we now prove:
a) that it is a normal divisor of $P_{r-1}$,
b) that it is a commutative group.

When we have proven both of these, we have reached our goal; for then we can, if there does not exist a commutative normal divisor of lower degree of $P_{r-1}$, choose $R$ itself for $Q_{r-1}$.

The first is immediately clear. For if $\gamma$ denotes any element from $P_{r-1}$, then

$$
\gamma^{-1} R \gamma = (\gamma^{-1} Q_r \gamma, \gamma^{-1} Q'_r \gamma, \gamma^{-1} Q''_r \gamma \ldots)
$$

is the smallest common multiple of the groups

$$
\gamma^{-1} Q_r \gamma, \gamma^{-1} Q'_r \gamma, \gamma^{-1} Q''_r \gamma \ldots
$$

These groups however are according to definition (7) in their totality not different from the groups

$$
Q_r, Q'_r, Q''_r \ldots
$$

and consequently

$$
\gamma^{\-1} R \gamma = R,
$$

i.e. $R$ is a normal divisor of $P_{r-1}$.

However, to prove that $R$ is a commutative group, we must first present two auxiliary considerations.

1) It is to be proven that any two of the groups $Q_r, Q\textrm'_r, Q\textrm'\textrm'_r \ldots$ have no common divisor besides the unit group.

We need only prove for this that $Q_r, Q\textrm'_r$ have this property. For if we have

$$
Q'_r = \gamma'^{-1} Q_r \gamma', \quad Q''_r = \gamma''^{-1} Q_r \gamma''
$$

with greatest common divisor $T$, then $Q_r$ and $Q\textrm'\textrm'_r = \gamma\textrm' Q\textrm'_r \gamma\textrm'^{-1}$ have the greatest common divisor $\gamma\textrm' T \gamma\textrm'^{-1}$.

Let us therefore assume that $T$ is the greatest common divisor of $Q_r$ and $Q\textrm'_r$; then $T$ is certainly a commutative group, since $Q_r$, $Q\textrm'_r$ are such. $T$ is also a normal divisor of $P_r$. For $Q_r$ and $Q\textrm'_r$ are such divisors; and if therefore $\pi$ is an element from $T$ and $\tau$ an element from $P_r$, then $\tau^{-1}\pi\tau$ is contained in both $Q_r$ and $Q\textrm'_r$, thus also in $T$. Consequently $\tau^{-1} T \tau = T$.

Now we have however assumed that $Q_r$ is a commutative normal divisor of $P_r$ above the unit of possibly lowest degree; furthermore $Q_r$ and $Q\textrm'_r$ were different from each other. Thus $T$ can only be the unit group itself, q.e.d.

2) To form the group $R$, we can proceed by taking the elements from $Q_r, Q\textrm'_r, Q\textrm'\textrm'_r \ldots$ in any order and composing them with each other repeatedly as long as new elements arise. For all compositions formed thus make up a group $C$ that is contained in $R$ because it contains the individual elements of $Q_r, Q\textrm'_r, Q\textrm'\textrm'_r \ldots$ On the other hand, the groups $Q_r, Q\textrm'_r, Q\textrm'\textrm'_r \ldots$ are also contained in $C$, and consequently $R$ is contained in $C$ and $C$ is identical with $R$.

To therefore prove finally that $R$ is a commutative group, it remains only to show us that if $\alpha, \beta$ are any two elements from $Q_r, Q\textrm'_r, Q\textrm'\textrm'_r \ldots$, the interchangeability

$$
\alpha \beta = \beta \alpha
$$

exists.

If now $\alpha, \beta$ both belong to the same group $Q_r$, then (10) follows from our assumption that $Q_r$ is commutative; and likewise if both occur in one of the other groups $Q\textrm'_r, Q\textrm'\textrm'_r \ldots$

But if $\alpha$ and $\beta$ are contained in two different groups, say in $Q_r$ and $Q\textrm'_r$, then we conclude as follows: Because $\beta$ is contained in $P_r$ and $Q_r$ is a normal divisor of $P_r$, therefore also

$$
\beta^{-1} \alpha \beta = \alpha'
$$

is contained in $Q_r$. From this follows:

$$
\beta \alpha' \beta^{-1} = \alpha'',
$$

and because $\alpha$ is contained in $P_r$ and $Q\textrm'_r$ is a normal divisor of $P_r$, $\alpha\textrm'\textrm'$ is also contained in $Q\textrm'_r$. But from (12) follows

$$
\alpha' \alpha^{-1} = \beta^{-1} \alpha'' = \delta,
$$

and consequently the element $\delta$ is contained in both $Q_r$ and $Q\textrm'_r$. According to what was proven under 1), it can therefore only be the unit element, i.e.

$$
\alpha' = \alpha, \quad \alpha'' = \beta,
$$

and consequently it follows from (11) that $\alpha \beta = \beta \alpha$ must hold, as was to be proven.
