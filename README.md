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
