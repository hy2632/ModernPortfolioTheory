# Efficient-Frontier
[Wikipedia - Modern portfolio theory - Mathematical Model](https://en.wikipedia.org/wiki/Modern_portfolio_theory)

The analytical solution of efficient frontier. 

The class includes:
- Monte Carlo simulation of portfolios consisting of assets in the designated pool.
- Solve for the curve of the efficient frontier analytically (a constrained optimization problem) using lagrange multiplier. This solution did not take into consideration the constraint that all weights are greater than 0, a.k.a. it allows short and leverage.
  - ![](Misc/CodeCogsEqn.gif)
<!-- $$
\begin{bmatrix}2\Sigma &-R & -{\bf1}\\ R^T &0 & 0 \\ {\bf1}^T &0 &0 \end{bmatrix} 
* \begin{bmatrix}w\\\lambda_1\\\lambda_2\end{bmatrix} 
= \begin{bmatrix}0\\\mu \\ 1\end{bmatrix}
$$ -->

- (2021/1/30 Update) `optimizerSolver()` to solve for the efficient frontier using scipy optimizer. Due to the limit of the optimizer, this solution performs bad for low `mu` part.

- Plot the "Expected Annual Return - Portfolio Volatility" chart, with MC points and the analytical solutions.
![](Misc/Figure_1.png)
