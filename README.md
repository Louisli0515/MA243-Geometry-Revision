# MA243-Geometry-Revision
My own revision on the module Geometry, mainly from example sheets and past papers

This repository will mainly focus on two parts, from support class sheets and past papers. For the support class I will create my own pdf, so no license issues should be addressed.





## Lecture notes

[MA243Notes.pdf](https://github.com/Louisli0515/MA243-Geometry-Revision/files/11215007/MA243Notes.pdf)

First thing first, feel free to download the 2022 version of lecture nots.

## Example sheets

### Week 1

[MA243_Geometry_week_1.pdf](https://github.com/Louisli0515/MA243-Geometry-Revision/files/11217035/MA243_Geometry_week_1.pdf)

In week 1's example sheets, there are some new definitions and old linear algebra knowledge to look at.

#### Metric

* A ***metric*** or ***distance***, $d$ on a set $X$ is a function $$d:X\times X\to[0,\infty)$$ such that it is 

(1) Non-degenerate: $$d(x,y) = 0\Leftrightarrow x = y,\,\forall x,y\in X.$$ (2) Symmetric: $$d(x,y) = d(y,x).$$ (3) Triangle Inquality: $$d(x,y)\leq d(x,z)+d(z,y).$$

#### Collinearity

* If $\mathbf{x},\mathbf{y},\mathbf{z}$ are ***distinct collinear points*** on a line $L\subset\mathbb{R}^{m}$, then for some $\lambda\in\mathbb{R}$ we have $$\mathbf{z} = \lambda_{1}\mathbf{x}+\lambda_{2}\mathbf{y},$$ where $\lambda_{1}+\lambda_{2} = 1$ and $\lambda_{2} = \lambda$.

#### Isometries and Euclidean space

* If $(X_{1},d_{1})$ and $(X_{2},d_{2})$ are ***metric spaces***, then a ***distance preserving map*** between $(X_{1},d_{1})$ and $(X_{2},d_{2})$ is a map $f:X_{1}\to X_{2}$ such that for any points $P,Q$ in $X_{1}$, we have $$d_{2}(f(P),f(Q)) = d_{1}(P,Q).$$
* An isometry is a ***bijective*** distance preserving map.
* If $f$ is an isometry, then $(X_{1},d_{1})$ and $(X_{2},d_{2})$ are said to be ***isometric***.
* A ***Euclidean space*** is a metric space which is ***isometric*** to $\mathbb{R}^{n}$, with the Euclidean metric, for some integer $n$. We use the notation $\mathbb{E}^{n}$ to denote the metric space $\mathbb{R}^{n}$ together with the Euclidean metric. If not specified otherwise, $\mathbb{R}^{n}$ is used to mean $\mathbb{E}^{n}$.

#### Affine maps

* A map $T:\mathbb{R}^{n}\to\mathbb{R}^{k}$ is ***affine*** as it is of the form $T(\mathbf{x}) = L(\mathbf{x}) + \mathbf{b}$ for all $\mathbf{x}\in\mathbb{R}^{n}$ for some ***linear map*** $L:\mathbb{R}^{n}\to\mathbb{R}^{k}$ and $\mathbf{b}\in\mathbb{R}^{k}$. Note that $\mathbf{b} = T(\mathbf{0}).$

#### Reflection and rotational matrix

* A reflection matrix has eigenvalues $\pm 1$, while a rotational matrix with an anti-clockwise rotation has eigenvalues $e^{\pm i\theta}$.
* A ***reflection matrix*** has determinant -1 while a ***rotation matrix*** has determinant 1.

#### Euclidian motion

* An Euclidian motion is a bijective map $T:\mathbb{E}^{n}\to\mathbb{E}^{n}$ that is an isometry.

#### Glide reflection

* We can assume that the glide $f$ is given by 

```math
\begin{pmatrix} x\\y \end{pmatrix} \to \begin{pmatrix} 1&0\\ 0&-1 \end{pmatrix} \begin{pmatrix} x\\ y\end{pmatrix} + \begin{pmatrix}  t\\ 0 \end{pmatrix},
```
where $t$ is non-zero.

### Week 2

[MA243_Geometry_week_2.pdf](https://github.com/Louisli0515/MA243-Geometry-Revision/files/11232734/MA243_Geometry_week_2.pdf)

In week 2's example sheets, note that there are some theorems to be revised.

#### Orthogonality

* Vectors $\mathbf{u},\mathbf{v}$ are ***orthogonal*** to each other if  their inner product is 0. 
* A basis of $\mathbb{R}^{n}$ is an ***orthogonal basis*** if it consists of normalised vectors which are mutually orthogonal.
* An orthogonal matrix is $A^{T} = A^{-1}$.

#### Orthogonal complement

* If $V$ is a vector space, with a subspace $W$, then the ***orthogonal complement*** of $W$ in $V$ is the vector subspace $$W^{\perp} = \set{\mathbf{v}\in V:\langle\mathbf{v},\mathbf{w}\rangle = 0,\forall \mathbf{w}\in W}.$$

#### Eigenvectors and eigenvalues

* If a matrix has no real eigenvalues, then it is not diagonalisable over the real numbers.
* Any real polynomial of odd degree has a real root.

#### Orthogonal matrices and Linear Isometry

* Let $L:\mathbb{R}^{n}\to\mathbb{R}^{n}$ be a linear map with matrix $A$ with respect to the standard basis. Then the following ***are equivalent***:
* $L$ is an isometry.
* $\left\|L(\mathbf{x})\right\| = \left\|\mathbf{x}\right\|$ for all $\mathbf{x}\in\mathbb{R}^{n}$, i.e. $L$ is ***norm preseving***.
* $\langle L(\mathbf{x}), L(\mathbf{y})\rangle = \langle \mathbf{x},\mathbf{y}\rangle.$, $\forall\mathbf{x},\mathbf{y}\in\mathbb{R}^{n}$, i.e. $L$ ***preserves the inner product***.
* The matrix $A$ is ***orthogonal***, i.e. $A^{T}A = I$.

#### Normal form Theorem

* Let $L:\mathbb{R}^{n}\to\mathbb{R}^{n}$ be a ***linear isometry*** and $A$ an ***orthogonal matrix*** such that $L(\mathbf{x}) = A\mathbf{x}$. Then there is an ***orthonormal basis*** of $\mathbb{R}^{n}$ with respect to which $L$ has the matrix of the form 

```math
\begin{bmatrix} I_{k} &  &  & &\\
 & -I_{m} &  & &\\
 &  & B_{1} & &\\
 &  &  & \ddots &\\
 &  &  &  & B_{l}\end{bmatrix},
```
where $I_{k}$ is the $k\times k$ identity matrix, and $B_{i}$ is the $2\times 2$ matrix representing a rotation of $\theta_{i}$ degrees counter clockwise about origin 

```math
B_{i} = \begin{bmatrix} \cos\theta_{i} & -\sin\theta_{i} \\
 \sin\theta_{i} & \cos\theta_{i}\end{bmatrix}.
```

#### Spectral theorem

* $A$ is normal if and only if it is unitarily diagonalisable. i.e. $A$ is normal if and only if there exists a unitary matrix $U$ such that $$A = UDU^* ,$$ where $D$ is a digaonal matrix, and $U$ is a unitary matrix, meaning its conjugate transpose $U*$ is also its inverse, that is, if $$U^* U = UU^* = UU^{-1} = I.$$

#### Euclidian geometry important theorems

* Let $T:\mathbb{R}^{2}\to\mathbb{R}^{2}$ be a Euclidian isometry. Then the image $T(C)$ of a circle $C$ of centre $x\in\mathbb{R}^{2}$ and radius $r > 0$ is a circle of centre $T(x)$ and radius $r$.
* Let $n\geq 1$ and $L:\mathbb{R}^{n}\to\mathbb{R}^{n}$ be a linear Euclidian isometry with a real eigenvalue $\lambda$, then $\lambda = \pm 1$.
* For every $n\geq 2$, every Euclidian line $L$ in $\mathbb{R}^{n}$ and point $P\in\mathbb{R}^{n}$ not belonging to $L$, there is a line $L'$ passing through $P$ such that $L\cap L' = \emptyset$.

### Week 3

[MA243_Geometry_week_3.pdf](https://github.com/Louisli0515/MA243-Geometry-Revision/files/11237714/MA243_Geometry_week_3.pdf)

In week 3's example sheet, we focus mainly on groups and hyperplanes.

#### Hyperplane

* A ***hyperplane*** of $\mathbb{R}^{n}$ is an affine subspace of dimension $n-1$, which has the form $$\Pi = V+\mathbf{b} = \set{\mathbf{b}+\mathbf{v}:\mathbf{v}\in V} = (\mathbb{R}\mathbf{v}_ n)^{\perp} + \mathbf{b} = \set{\mathbf{v}\in\mathbb{R}^{n}:\langle\mathbf{v},\mathbf{v}_ n\rangle = \beta}.$$

#### Reflection

* The reflection $\rho_{\Pi}$ in the hyperplane $\Pi$ exists and is ***unique***, and is given by $$\rho_{\Pi}:\mathbf{P}\to\mathbf{P}-2\langle\mathbf{P}-\mathbf{b},\mathbf{v}\rangle\mathbf{v},$$ where $\Pi = \mathbf{b}+(\mathbb{R}\mathbf{v})^{\perp}$ and $\left|\mathbf{v}\right| = 1$.
* If $R$ is a reflection and $T$ is any isometry, then $T^{-1}\circ R\circ T$ is also a reflection.
* If $\rho_{\Pi}$ is a reflection in the plane $\Pi$, then the conjugation of $\rho_{\Pi}$ by the reflection $T(\mathbf{x}) = \mathbf{x}+\mathbf{c}$, that is, the map $T^{-1}\circ\rho_{\Pi}\circ T$ is a reflection in $\Pi - \mathbf{c}$.
* A reflection $R$ has order 2, that is, $$R\circ R = \text{id}.$$

#### Review of Group Theory

* A ***homomorphism*** between two groups $G$ and $H$ is a map $$\phi:G\to H$$ such that $\phi(gh^{-1}) = \phi(g)\phi(h)^{-1}$ for all $g,h\in G$. i.e. $\phi$ preserves multiplication, inverse, identity.
* An ***Isomorphism*** is a ***group homomorphism*** which is a bijection.
* The group of ***automorphisms*** of a group $H$ is the group $$Aut(H) = \set{f:H\to H:f\ \text{is}\ \text{group}\ \text{isomorphism}},$$ with group law composition of functions. 

### Week 4

[MA243_Geometry_week_4.pdf](https://github.com/Louisli0515/MA243-Geometry-Revision/files/11239138/MA243_Geometry_week_4.pdf)

In week 4's example sheet, we enter the field of spherical geometry.

#### The sphere and the spherical metric

* The ***n-dimensional sphere*** of radius $r\geq 0$ is defined by $$S_{r}^{n} = \set{\mathbf{x}\in\mathbb{R}^{n+1}:\left|\mathbf{x}\right| = r},$$ where $S^{n} = S_{1}^{n},$ which has Euclidean norm 1.
* A spherical line or ***great circle*** is the intersection of $S_{r}^{n}$ with a ***2-dimensional vector subspace*** of $\mathbb{R}^{n+1}$, i.e. $$S^{2}\cap\Pi,$$ where $\Pi$ is some plane in $\mathbb{R}^{3}$ containing 0.

#### Antipodal

* If $\mathbf{P},\mathbf{Q}\in S_{r}^{n}$, then they are ***antipodal*** if $\mathbf{Q} = -\mathbf{P}$.
* If $\mathbf{P}$ and $\mathbf{Q}$ in $S_{r}^{n}$ are ***not antipodal***, then there is a unique great circle containing both of them.

#### Spherical Distance

* The ***spherical distance*** between two points $\mathbf{P},\mathbf{Q}\in S_{r}^{n}$ is the length of the ***shortest arc*** of a great circle joining them. We will show that this distance is a metric, called the ***spherical metric***, which we can also define by $$d_{S_{r}^{n}}(\mathbf{P},\mathbf{Q}) = r\arccos\left(\frac{\langle\mathbf{P},\mathbf{Q}\rangle}{r^{2}}\right).$$

#### Main formula of spherical trigonomtry
* Let $\alpha,\beta,\gamma$ be the ***side lengths*** of a spherical triangle with vertices $\mathbf{P},\mathbf{Q},\mathbf{R}\in S^{2}$ on the unit sphere, $$\alpha = d(\mathbf{Q},\mathbf{R}),\quad\beta = d(\mathbf{P},\mathbf{Q}),\quad\gamma = d(\mathbf{P},\mathbf{Q}),$$ where $d = d_{S^{2}}$ is the ***spherical metric***. Let $a$ be the ***spherical angle*** between arcs $\mathbf{P}\mathbf{Q}$ and $\mathbf{P}\mathbf{R}$. Then $$\cos\alpha = \cos\beta\cdot\cos\gamma + \sin\beta\cdot\sin\gamma\cdot\cos a.$$

#### Isometry in spherical geometry

* An isometry $T:S^{n}\to S^{N}$ preserves ***antipodal points***.
* An isometry $T:S^{n}\to S^{N}$ preserves ***great circles***.
* A ***bijective map*** $f:\mathbb{R}^{k}\to\mathbb{R}^{k}$, which ***preserves the standard inner product*** on $\mathbb{R}^{k}$ is a ***linear isometry*** of $\mathbb{R}^{k}$.
* If $L:\mathbb{R}^{n+1}\to\mathbb{R}^{n+1}$ is a linear isometry and since it is bijective, then $$L(A\cap B) = L(A)\cap L(B)$$ for general subsets $A,B$.

#### Area of spherical triangle

* The spherical triangle $\triangle$ with angles $\alpha,\beta,\gamma$ is $$\text{area}(\triangle) = \alpha+\beta+\gamma - \pi.$$

#### Important theorems in spherical geometry

* If $\mathcal{C}$ and $\mathcal{D}$ are two distinct great circles on $S^{2}$, then $\mathcal{C}\cap\mathcal{D} = \set{-P,P}$ for some $P\in S^{2}$.

### Week 5

[MA243_Geometry_week_5.pdf](https://github.com/Louisli0515/MA243-Geometry-Revision/files/11240922/MA243_Geometry_week_5.pdf)

In week 5's example sheet, we mainly focus on spherical geometry and hyperplane and Lorentz transformation.

#### Definition of hyperbolic metric

* The hyperbolic metric on $\mathcal{H}^{n}$ is defined as $$\mathcal{H}^{n} = \set{\mathbf{x}\in\mathbb{R}^{n+1}:\left\|\mathbf{x}\right\|_ {L} = i, x_{1} > 0}.$$


#### Definition for $\mathcal{H}^{n}$ is comparable to that for $S^{n}$

* We note the difference between these two: $$d_{S^{n}}(\mathbf{x},\mathbf{y}) = \cos^{-1}(\mathbf{x},\mathbf{y}) = \left(\frac{\langle\mathbf{x},\mathbf{y}\rangle}{|\mathbf{x}| |\mathbf{y}|}\right)\quad d_{\mathcal{H}^{n}}(\mathbf{x},\mathbf{y}) = \cosh^{-1}(\mathbf{x},\mathbf{y}) = \left(\frac{\langle\mathbf{x},\mathbf{y}\rangle_{L}}{|\mathbf{x}|_L|\mathbf{y}|_L}\right).$$

#### Terminology inspired by special relativity

There are several terminology including ***time,space and light like vectors***:

* A point $\mathbf{x}\in\mathbb{R}^{n}$ is ***space-like*** if $\left\|\mathbf{x}\right\|_{L}\in (0,\infty)$, i.e. if $\langle\mathbf{x},\mathbf{x}\rangle _{L}>0.$
* A point $\mathbf{x}\in\mathbb{R}^{n}$ is ***light-like*** if $\left|\mathbf{x}\right|_{L} = 0$, i.e. if $\langle\mathbf{x},\mathbf{x}\rangle _{L}=0.$
* A point $\mathbf{x}\in\mathbb{R}^{n}$ is ***time-like*** if $\left|\mathbf{x}\right|_{L}\in i(0,\infty)$, i.e. if $\langle\mathbf{x},\mathbf{x}\rangle _{L}<0.$
* A point $\mathbf{x}\in\mathbb{R}^{n}$ is ***positive*** if $x_{1} > 0.$
* A point $\mathbf{x}\in\mathbb{R}^{n}$ is ***negative*** if $x_{1} < 0.$
* A ***time-like*** or ***space-like*** vector $\mathbf{x}\in\mathbb{R}^{n}$ is ***positive*** if $x_{1} > 0$ and ***negative*** if $x_{1} < 0.$

#### Lorentz transformation

* A map $T:\mathbb{R}^{n}\to\mathbb{R}^{n}$ is a ***Lorentz transformation*** if it preserves the Lorentz inner product: $$\langle T(\mathbf{x}),T(\mathbf{y})\rangle_{L} = \langle\mathbf{x},\mathbf{y}\rangle_{L}\,\forall\mathbf{x},\mathbf{y}\in\mathbb{R}^{n}.$$
* We see that $T$ is ***positive*** if $\mathbf{x}$ is ***positive time-like*** if and only if $T(\mathbf{x})$ is ***positive time-like***.
* A Lorentz transformation is ***bijective***.

#### Lorentz orthogonal

* An $n\times n$ real matrix $A$ is ***Lorentz orthogonal*** if 
```math
A^{T}JA = J:= \begin{bmatrix} -1 & \mathbf{0} \\
 \mathbf{0} & I_{n-1} \end{bmatrix},
```

* The ***Lorentz group*** is the group of Lorentz orthogonal $(n+1)\times (n+1)$ matrices, denoted $$O(1,n) = \set{A\in M_{(n+1)\times(n+1)}|A^{T}JA = J}.$$
* The ***positive Lorentz group*** is the subgroup of $O(1,n)$ which maps ***positive time like vectors*** bijectively to ***positive time like vectors***. This is denoted $O^{+}(1,n)$.
* $O(1,n)$ and $O^{+}(1,n)$ are groups.
* A set of vectors $\mathbf{v}_ 1,...,\mathbf{v}_ n\in\mathbb{R}^{n}$ is ***Lorentz orthogonal*** if $\langle\mathbf{v}_ {i},\mathbf{v}_ {j}\rangle_{L} = 0$ for $i\ne j$. 
It is ***Lorentz orthonormal*** if 
* (1) $\langle\mathbf{v}_ {i},\mathbf{v}_ {j}\rangle_{L} = 0,$ if $i\ne j$.
* (2) $\langle\mathbf{v}_ {i},\mathbf{v}_ {j}\rangle_{L} = 1,$ if $2\leq i=j < n$.
* (3) $\langle\mathbf{v}_ {i},\mathbf{v}_ {j}\rangle_{L} = -1,$ if $i=j=1$.
* If $A\in O(1,n)$, then $A^{T}\in O(1,n).$

#### Lemma of Lorentz transformation

* The ***canonical basis*** $\mathbf{e}_ {1},...,\mathbf{e}_ {n}$ is ***Lorentz orthonormal***.
* If $\mathbf{v}_ {1},...,\mathbf{v}_ {n}$ are ***Lorentz orthonormal***, then they form a basis of $\mathbb{R}^{n}$.
* $\mathbf{v}_ {1},...,\mathbf{v}_ {n}$ is a Lorentz orthonormal basis if and only if $\langle\mathbf{v}_ {i},\mathbf{v}_ {j}\rangle_{L} = J_{i,j}$, the element in the ith row, jth column of $J$.
* A linear map $T:\mathbb{R}^{n}\to\mathbb{R}^{n}$, with matrix $A$ is a ***Lorentz transformation*** if and only if it maps the ***standard basis*** to a ***Lorentz orthonormal basis***.
* Let $A$ be a $n\times n$ matrix. THe following are equivalent: 
* (1) The map $T(\mathbf{x}) = A\mathbf{x}$ is a ***Lorentz transformation***.
* (2) $\left\|T(\mathbf{x})\right\|_ {L} = \left|\mathbf{x}\right|_ {L}$ for all $\mathbf{x}\in\mathbb{R}^{n}$.
* (3) $A$ is ***Lorentz orthogonal***.
* A map $T:\mathbb{R}^{n}\to\mathbb{R}^{n}$ is a Lorentz transformation if and only if 
* (1) The image of the canonical basis $T(\mathbf{e}_ {1}),...,T(\mathbf{e}_ {n})$ is ***Lorentz orthonormal***.
* (2) $T$ is ***linear***.
* There is a ***basis*** of $\mathbb{R}^{n+1}$ consisting of ***time-like*** vectors, which may be taken to be elements of $\mathcal{H}^{n}$.

#### Hyperbolic lines

* A 2-dimensional ***sub-vector*** space $V$ of $\mathbb{R}^{n+1}$ is called a ***Lorentz plane*** if it contains a ***time-like*** vector. A ***hyperbolic line*** is the intersection of $\mathcal{H}^{n}$ with any ***Lorentz plane***.

### Week 6

[MA243_Geometry_week_6.pdf](https://github.com/Louisli0515/MA243-Geometry-Revision/files/11244804/MA243_Geometry_week_6.pdf)

Week 6's example sheet is a recap of Lorentz geometry and isomorphism. Therefore all the lemmas and theorems are given above, there is only one to note.

#### Parameterisation of $\mathcal{H}^{2}$

* There is a ***paraterisation*** $f:\mathbb{R}^{2}\to\mathcal{H}^{2}$ where $$f:(t,\theta)\to(\cosh(t),\cos(\theta)\sinh(t),\sin(\theta)\sinh(t)),\quad t\in[0,\infty),\theta\in[0,2\pi),$$ where $\mathbb{R}^{2}$ is given with polar coordiantes, and $\mathcal{H}^{2}$ with the Cartesian coordinates of $\mathbb{R}^{3}$.

#### Area of hyperbolic triangle

* The area of a hyperbolic triangle $\triangle$ with angles $\alpha,\beta,\gamma$ is $$\text{area}(\triangle) = \pi-(\alpha+\beta+\gamma).$$

#### Main formula of hyperbolic trignometry

* For distinct points $\mathbf{x},\mathbf{y},\mathbf{z}$ in $\mathcal{H}^{n}$, let $$\alpha = d_{\mathcal{H}^{n}}(\mathbf{z},\mathbf{y}),\quad\beta = d_{\mathcal{H}^{n}}(\mathbf{x},\mathbf{z}),\quad\gamma = d_{\mathcal{H}^{n}}(\mathbf{x},\mathbf{y}),\quad a = \text{hyperbolic angle at x},$$ then $$\cosh\alpha = \cosh\beta\cdot\cosh\gamma - \sinh\beta\cdot\sinh\gamma\cdot\cos a.$$

#### Important theorms in hyperbolic geometry

* For every $n\geq 2$, every hyperbolic line $L$ in $\mathcal{H}^{n}$ and point $P\in\mathcal{H}^{n}$ not belonging to $L$, there is a hyperbolic line $L'$ passing through $P$ such that $L\cap L' = \emptyset$.

### Week 7

[MA243_Geometry_week_7.pdf](https://github.com/Louisli0515/MA243-Geometry-Revision/files/11299007/MA243_Geometry_week_7.pdf)


Week 7's example sheet leads us to Projective Geometry.

#### Equivalence relation

* Define an ***equivalence relation*** on $V^{*}$ by defining for $\mathbf{x},\mathbf{y}\in V$, $$\mathbf{x}\sim\mathbf{y}\Longleftrightarrow k\mathbf{x} = k\mathbf{y}.$$

#### Projective space

* The ***projective space of*** $V$ is the set of ***equivalence classes*** in $V^{*}$ under this relation: $$\mathbb{P}^{n}(k) = \mathbb{P}(V) = V^{ *}\setminus\sim.$$
* When $k = \mathbb{R}$, we write $\mathbb{P}^{n} = \mathbb{P}(\mathbb{R}^{n+1})$, and call this $n$-dimensional real projective space.

Alternative definition

* The projective space $\mathbb{P}^{n}$ is the set of lines through 0 in $\mathbb{R}^{n+1}$.

#### k-dimensional projective linear subspace

* If $V$ is a vector space $V$, with a $k+1$ dimensional vector subspace $W$, then the ***k-dimensional projective linear subspace*** $\mathbb{P}(W)$ of $\mathbb{P}(V)$ is the ***image under*** $\pi$ of $W$ in $\mathbb{P}(V)$, that is $$\mathbb{P}(W) = \set{\mathbf{x}\in\mathbb{P}(V):\mathbf{x}\subset W} = \pi(W).$$
* The dimension of $\mathbb{P}(W)$ is one less than the dimension of $W$.

#### Definition of point, line and plane in projective geometry

* Let $W$ be a ***subvector space*** of $V$. Then $$\mathbb{P}(W)$$ is a 
* ***point*** if $\dim(W) = 1$.
* ***line*** if $\dim(W) = 2$.
* ***plane*** if $\dim(W) = 3$.

#### Dimension formula for projective geometry

* For projective linear subspaces $E$ and $F$ of $\mathbb{P}(V)$, $$\dim(E\cap F) = \dim(E)+ \dim(F) - \dim\langle E,F\rangle,$$ with the convention $\dim(\emptyset) = -1$ and $\langle E,F\rangle$ is the linear subspace of $\mathbb{P}(V)$ spanned by $E$ and $F$.


#### Projective general linear group

* The ***projective general linear group*** of a vector space $V$ over a field $k$ is the group of all ***invertible linear maps*** from $T:V\to V$ up to ***scalar multiplication***, that is, we consider $T_{1}\sim T_{2}$ if there is some non-zero element $\lambda\in k$ with $T_{2} = \lambda T_{1}$. 
* We write PGL $(n)$ = PGL $(\mathbb{R}^{n})$. In this case, the elements of PGL $(n)$ are ***invertible matrices*** up to scalar multiplication, that is $$A\sim B\Longleftrightarrow  A = \lambda B$$ for some $\lambda\in\mathbb{R}^{*}.$

#### Projective transformation

* If $A$ is an invertible $(n+1)\times(n+1)$ matrix, then the map $$T_{A}:\mathbb{P}^{n}\to\mathbb{P}^{n},\quad \left[\mathbf{v}\right]\to\left[A\mathbf{v}\right]$$ is called a ***projective transformation***, or a ***projectivity*** or a ***projective linear map***.

#### Projective frame of reference

* A ***projective frame of reference*** for $\mathbb{P}^{n}$ is an ***ordered*** set of $n+2$ points, $P_{0}, P_{1},..., P_{n+1}\in\mathbb{P}^{n}$, any $n+1$ of which are ***linearly independent*** and so span $\mathbb{P}^{n}$.

#### Standard frame of reference

* The ***standard frame of reference*** for $\mathbb{P}^{n}$ is given by $[\mathbf{e}_ {1}],...,[\mathbf{e}_ {n+1}]$ together with $[\mathbf{e}_ {1} + ...+\mathbf{e}_ {n+1}]$, where $\mathbf{e}_{i}$ are the standard basis for $\mathbb{R}^{n+1}$.

#### Bijection between projective transformation and projective frames of reference

* There is a ***bijection*** between projective transformations of $\mathbb{P}^{n}$ and ***projective frames of references*** of $\mathbb{P}^{n}$, defined as follows: $$\phi: PGL(n+1)\to\set{\text{projective frames of reference}},\quad T\to\set{T([\mathbf{e}_ {1}]),...,T([\mathbf{e}_ {n+1}]), T([\mathbf{e}_ {1}+...+\mathbf{e}_ {n+1}])}.$$

### Week 8

This is the final example sheet as the remaining two focuses on assignments.

#### Perspectivity

* A ***perspectivity*** $f$ is a map between two ***distinct hyperplanes*** (linear subspaces of dimension $n-1$), $\Pi_{1}$ and $\Pi_{2}$ in $\mathbb{P}^{n}$, given by projection from a point $O\notin\Pi_{1}\cup\Pi_{2}$. That is , if $P\in\Pi_{1}$, then $f(P)\in\Pi_{2}$ is the point such that $0,P,f(P)$ all lie on the same line.

#### Projectivities between lines

* Two projectivities between lines coincide iff they coincide on a frame of reference, i.e. on three distinct points.

#### Cross ratio

* Let $P,Q,R,S$ be four ***distinct points on a line*** in $\mathbb{P}^{n}$. Choose an appropriate basis such that $P = (1:0)$ and $Q = (0:1)$. Since $\tilde{P}$ and $\tilde{Q}$ span the line that $R$ and $S$ lie on, and since $R,S\ne P$, there are $\lambda,\mu\in\mathbb{R}$ such that we can write with respect to this basis: $$R = (1:\lambda), S = (1:\mu).$$ Then the ***cross ratio*** is $$\set{P,Q;R,S} = \frac{\lambda}{\mu}.$$
* Here, $\tilde{P}$ is defined up to direction, not magnitude, and given by $$\tilde{P} = \text{any choice of non-zero}\mathbf{v}\in P.$$
* If $P,Q,R,S$ are points in $\mathbb{P}^{1}$, then they can be considered as lines in $\mathbb{R}^{2}$. Let $L$ be any line in $\mathbb{R}^{2}$ not through the origin. Let $\mathbf{p},\mathbf{q},\mathbf{r},\mathbf{s}$ be the vector coordinates of the intersections of $P,Q,R,S$ with $L$. Then $$\set{P,Q;R,S} = \left(\frac{\mathbf{p}-\mathbf{r}}{\mathbf{p}-\mathbf{s}}\right)\left(\frac{\mathbf{q}-\mathbf{s}}{\mathbf{q}-\mathbf{r}}\right),$$ where the ratios of vectors make sense because they all in the direction of $L$, and we define $\frac{\lambda\mathbf{v}}{\mathbf{v}} = \lambda.$

#### Definitions of triangle

* A ***triangle*** $\Delta PQR$ in $\mathbb{P}^{n}$ is a set of three distinct points, $P,Q,R\in\mathbb{P}^{n}$ and the "sides" of the triangle, which are three lines spanned by the three paris of points.
* Two triangles $\Delta PQR$ and $\Delta P'Q'R'$ in $\mathbb{P}^{n}$ are said to be ***in persepctive from a point*** $\mathcal{O}$ if the lines $\langle P,P'\rangle, \langle Q,Q'\rangle, \langle R,R'\rangle$ all ***intersect in a common point*** $\mathcal{O}$.
* Two triangles $\Delta PQR$ and $\Delta P'Q'R'$ with sides $p,q,r$ and $p',q',r'$ in $\mathbb{P}^{n}$ are said to be ***in perspective from a line*** $L$ if the points $p\cap p',q\cap q',r\cap r'$ all lie on a common line $L$.

#### Important theorems in projective geometry

* Any two distinct lines in $\mathbb{P}^{2}$ intersect at a point.
* Whenever $\mathbb{F}_ {q}$ is a field, (i.e. $q$ is a prime power), the projective plane $\mathbb{P}^{2}(\mathbb{F}_ {q})$ has $q^{2}+q+1$ points and $q^{2}+q+1$ lines. Each line contains $q+1$ points and each point is contained in $q+1$ lines.

#### Desargues' Theorem

* If $\Delta PQR$ and $\Delta P'Q'R'$ are two ***distinct triangles*** in $\mathbb{P}^{n}$ which are in ***perspective from a point, then they are also in perspective from a line***.

#### Pappu's Theorem

* Let $L,L'\subset\mathbb{P}^{2}$ be ***distinct projective lines***. Let $P,Q,R\in L\setminus L', P', Q', R'\in L'\setminus L$ be distinct points. Then  the intersection points $$A = \langle P,Q'\rangle\cap\langle P',Q\rangle,\quad B = \langle P,R'\rangle\cap\langle P',R\rangle,\quad C = \langle Q,R'\rangle\cap\langle Q', R\rangle$$ are colinear.
