# Density matrix

## Pure state

A **pure state** is a vector in the Hilbert space of the quantum system we are interested in
$$
| \psi \rangle \in \mathscr{H}
$$

## Mixed state

A **mixed state** is a state which has a classical probability distribution in different pure state. Notice that a mixed state is different from a quantum superposition. 

## Density matrix

For a **finite-dimensional** function space, the most general density operator is of the form
$$
\rho = \sum_j p_j | \psi_j \rangle \langle \psi_j |
$$
where the coefficients $p_j$ are non-negative and add up to one, and $| \psi_j \rangle \langle \psi_j |$ is an outer product written in bra-ket notation. This represents a mixed state, with probability $p_j$ that the system is in the pure state $| \psi_j \rangle$. 

For pure state, a density operator or density matrix is a projection
$$
\rho = |\psi \rangle \langle \psi |
$$
which means $\rho^2 = \rho$.

### Example: qubit

All qubit states $\omega$ may be represented as $2 \times 2$ matrices
$$
\begin{gather}
\rho = \frac{1}{2}
\begin{pmatrix}
1 + x_3 & x_1 - i x_2 \\
x_1 + i x_2 & 1 - x_3
\end{pmatrix} , \quad \underline{x} \in \mathbb{R}^3\\
\rho \ge 0 , \quad \operatorname{tr}(\rho) = 1
\end{gather}
$$

#### Exercise 

Show $\rho \ge 0 \Leftrightarrow |\underline{x}| \le 1$. Thus $\underline{x} = (x_1, x_2, x_3)$ is in ball of radius 1.
$$
\rho = \frac{1}{2}(\mathbb{I} + x_1 \sigma_x + x_2 \sigma_y + x_3 \sigma_z)
$$
the eigenvalues of $\rho$ is $\frac{1}{2} (1 \pm |\underline{x}|)$. For $\rho \ge 0$, $\exist X \in \mathbb{C}^{2 \times 2}$, such that $\rho = X^H X$.

Equivalently speaking, the eigenvalues of $\rho$ are all greater than or equal to 0. Therefore $|\underline{x}| \le 1$. 

For pure states of a qubit, the possible vector $\underline{x}$ is in a sphere of radius 1, which we call **Bloch sphere**.

But unfortunately Bloch sphere cannot be generalized to higher dimension.

