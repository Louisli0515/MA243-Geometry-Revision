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
