# Relativistic structure of the Dirac equation
the Lorentz transformation:
$$
x\^\mu
\mapsto {x\^\mu}' 
\= 
{\Lambda\^\mu}\_\nu x\^\nu
\\\\
\partial\_\mu
\mapsto {\partial\_\mu}'
\= 
{(\Lambda\^{-1})\^\nu}\_\mu
\partial\_\nu
$$

Consider how the spinor is transformed.
Find $S(\Lambda)$ such that
$$
\psi(x)
\mapsto \psi'(x')
\=
S(\Lambda) \psi(x).
$$


## Relativistic invariance of the Dirac equation
If you have the Dirac equation in an inertial system,
$$
(i\gamma\^\mu \partial\_\mu - m I\_4) \psi(x) = 0,
$$
then you will have the one in another system,
$$
(i\gamma\^\mu {\partial\_\mu}' - m I\_4) \psi'(x') = 0,
\\\\
S(\Lambda)
[i {(\Lambda\^{-1})\^\nu}\_\mu S\^{-1}(\Lambda) \gamma\^\mu S(\Lambda) {\partial\_\nu} - m I\_4]
\psi(x) = 0.
$$
Here we should be careful that $\Lambda\^\nu\_\mu$ is just a scalar constant and $\gamma\^\mu$ is a $4\times4$ matrix.

The Lorentz invariance implies
$$
\gamma\^\nu 
\= 
{(\Lambda\^{-1})\^\nu}\_\mu S\^{-1}(\Lambda) \gamma\^\mu S(\Lambda),
\\\\
\tilde{\gamma\^\mu}
\equiv
{\Lambda\^\mu}\_\nu \gamma\^\nu 
\= 
S\^{-1}(\Lambda) \gamma\^\mu S(\Lambda).
$$
This is an equation that our target $S(\Lambda)$ satisfies.

Remind the anticommutation relation of the $\gamma$ matrices,
$$
[\gamma\^\mu,\gamma\^\nu]\_+
\=
2\eta\_{\mu\nu} I\_4.
$$
Thus, we also have the same anticommutation relation for the $\tilde{\gamma}$ matrices,
$$
[\tilde{\gamma}\^\mu,\tilde{\gamma}\^\nu]\_+
\=
2\eta\_{\mu\nu} I\_4.
$$

## Infinitesimal Lorentz transformation
Let us consider the infinitesimal Lorentz transformation.
We will construct the Lorentz transformation by repeating this infinitesimal transformation in the next section.
Here is our infinitesimal transformation,
$$
{\Lambda\^\mu}\_\nu
\=
{\delta\^\mu}\_\nu + {\Delta\omega\^\mu}\_\nu,
$$
where $\Delta\omega\^\mu\_\nu$ is an infinitesimal number.
The inverse of this transformation is given by
$$
{(\Lambda\^{-1})\^\mu}\_\nu
\=
{\delta\^\mu}\_\nu - {\Delta\omega\^\mu}\_\nu.
$$
Indeed, we have
$$
({\delta\^\mu}\_\bullet + {\Delta\omega\^\mu}\_\bullet)
({\delta\^\bullet}\_\nu - {\Delta\omega\^\bullet}\_\nu)
\=
{\delta\^\mu}\_\nu + {\Delta\omega\^\mu}\_\nu - {\Delta\omega\^\mu}\_\nu
\= 0,
$$
where the second-order infinitesimal vanishes.

Reminding that our metric tensor satisfies
$$
\eta\_{\mu\nu}
\=
\eta\_{\bullet\circ}
{(\Lambda\^{-1})\^\bullet}\_\mu
{(\Lambda\^{-1})\^\circ}\_\nu,
$$
we can obtain
$$
\eta\_{\mu\nu}
\=
\eta\_{\bullet\circ}
({\delta\^\bullet}\_\mu - \Delta{\omega\^\bullet}\_\mu)
({\delta\^\circ}\_\nu - \Delta{\omega\^\circ}\_\nu)
\=
\eta\_{\mu\nu} -
\Delta\omega\_{\nu\mu} -
\Delta\omega\_{\mu\nu},
\\\\
\Delta\omega\_{\nu\mu}
\=
-\Delta\omega\_{\mu\nu},
$$
where the second-order infinitesimal has vanished again.
Remind that we denote $\Delta\omega\_{\mu\nu}=\eta\_{\mu\bullet}{\omega\^\bullet}\_{\nu}$.
Thus, we can write the infinitesimal Lorentz transformation in a matrix form,
$$
{\Lambda\^\mu}\_\nu 
\=
{\delta\^\mu}_\nu
+
\eta\^{\mu\bullet}
\Delta\omega\_{\bullet\nu}
\\\\
:=
\begin{pmatrix}
1 & \Delta\omega\_{01} & \Delta\omega\_{02} & \Delta\omega\_{03}
\\\\
\Delta\omega\_{01} & 1 & -\Delta\omega\_{12} & \Delta\omega\_{31}
\\\\
\Delta\omega\_{02} & \Delta\omega\_{12} & 1 & -\Delta\omega\_{23}
\\\\
\Delta\omega\_{03} & -\Delta\omega\_{31}&  -\Delta\omega\_{23} & 1
\end{pmatrix}.
$$
Let us check this matrix represents infinitesimal Lorentz transformation.
Firstly, we substitute 
$\Delta\omega\_{ij}=0\ (i,j\in\\{1,2,3\\})$,
$\Delta\omega\_{0i}=0\ (i\in\\{2,3\\})$ 
and 
$\Delta\omega\_{01}=-\Delta\omega$ 
to have
$$
{\Lambda\^\mu}\_\nu 
:=
\begin{pmatrix}
1 & -\Delta\omega & 0 & 0
\\\\
-\Delta\omega & 1 & 0 & 0
\\\\
0 & 0 & 1 & 0
\\\\
0 & 0 & 0 & 1
\end{pmatrix}.
$$
We can find the right-top $2\times2$ block matrix represents Lorentz boost.
Secondly, we substitute 
$\Delta\omega\_{0i}=0\ (i\in\\{2,3\\})$ 
to have
$$
{\Lambda\^\mu}\_\nu 
:=
\begin{pmatrix}
1 & 0 & 0 & 0
\\\\
0 & 1 & -\Delta\omega\_{12} & \Delta\omega\_{31}
\\\\
0 & \Delta\omega\_{12} & 1 & -\Delta\omega\_{23}
\\\\
0 & -\Delta\omega\_{31}&  -\Delta\omega\_{23} & 1
\end{pmatrix}.
$$
We can find the right bottom $3\times3$ antisymmetric block matrix represent an infinitesimal rotation.
(Remind that rotation is represented by an antiymmetric matrix.)

## Lorentz transformation

## Bilinear form
