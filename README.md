# ModernPortfolioTheory
[Wikipedia - Modern portfolio theory - Mathematical Model](https://en.wikipedia.org/wiki/Modern_portfolio_theory)
## Efficient Frontier
The analytical solution of efficient frontier. 

The class includes:
- Monte Carlo simulation of 30000 portfolios consisting of assets in the designated pool.
- Solve the curve of the efficient frontier (a constrained optimization problem) using lagrange multiplier.

  - ![](CodeCogsEqn.gif)

<!-- $$
\begin{bmatrix}2\Sigma &-R & -{\bf1}\\ R^T &0 & 0 \\ {\bf1}^T &0 &0 \end{bmatrix} 
* \begin{bmatrix}w\\\lambda_1\\\lambda_2\end{bmatrix} 
= \begin{bmatrix}0\\\mu \\ 1\end{bmatrix}
$$ -->

- Plot the "Expected Annual Return - Portfolio Volatility" chart, with MC points and the analytical solution.
![](Efficient%20Frontier.jpg)
