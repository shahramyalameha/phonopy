.. _thermal_displacement:

Thermal displacement
====================

From Eq. (10.71) in the book "Thermodynamics of Crystal", atomic
displacement, **u**, is written by

.. math::

   u^\alpha(jl,t) = \left(\frac{\hbar}{2Nm_j}\right)^{\frac{1}{2}}
   \sum_{\mathbf{q},\nu}\left[\omega_\nu(\mathbf{q})\right]^{-\frac{1}{2}}
   \left[\hat{a}_\nu(\mathbf{q})\exp(-i\omega_\nu(\mathbf{q})t)+
   \hat{a}^\dagger_\nu(\mathbf{-q})\exp({i\omega_\nu(\mathbf{q})}t)\right]
   \exp({i\mathbf{q}\cdot\mathbf{r}(jl)})
   e^\alpha_\nu(j,\mathbf{q})

where *j* and *l* are the labels for the *j*-th atomic position in the
*l*-th unit cell, *t* is the time, :math:`\alpha` is the Cartesian
component, *m* is the atomic mass, *N* is the number of the unit
cells, :math:`\mathbf{q}` is the wave vector, :math:`\nu` is the index
of phonon mode. *e* is the polarization vector of the atom *jl* and
the band :math:`\nu` at :math:`\mathbf{q}`. :math:`\mathbf{r}(jl)` is
the atomic position and :math:`\omega` is the phonon
frequency. :math:`\hat{a}^\dagger` and :math:`\hat{a}` are the
creation and annihilation operators of phonon. The expectation value
of the squared atomic displacement is calculated as,

.. math::

   \left\langle |u^\alpha(jl, t)|^2 \right\rangle = \frac{\hbar}{2Nm_j}
   \sum_{\mathbf{q},\nu}\omega_\nu(\mathbf{q})^{-1}
   (1+2n_\nu(\mathbf{q}))|e^\alpha_\nu(j,\mathbf{q})|^2,

where *n* is the phonon population, which is give by,

.. math::

   n_\nu(\mathbf{q}) =
   \frac{1}{\exp(\hbar\omega_\nu(\mathbf{q})/\mathrm{k_B}T)-1},

where *T* is the temperature, and :math:`\mathrm{k_B}` is the
Boltzmann constant. The equation is calculated using the commutation
relation of the creation and annihilation operators and the 
expectation values of the combination of the operations, e.g.,

.. math::

   [ \hat{a}_\nu(\mathbf{q}), \hat{a}^\dagger_{\nu'}(\mathbf{q'}) ]
   = \delta(\mathbf{q}-\mathbf{q}')\delta_{\nu\nu'},

   [ \hat{a}_\nu(\mathbf{q}), \hat{a}_{\nu'}(\mathbf{q'}) ] = 0,

   [ \hat{a}^\dagger_\nu(\mathbf{q}), \hat{a}^\dagger_{\nu'}(\mathbf{q'}) ] = 0,

   \langle|\hat{a}_\nu(\mathbf{q})\hat{a}_{\nu'}(\mathbf{q'})|\rangle
   = 0,

   \langle|\hat{a}^\dagger_\nu(\mathbf{q})\hat{a}^\dagger_{\nu'}(\mathbf{q'})|\rangle
   = 0.
   

.. |sflogo| image:: http://sflogo.sourceforge.net/sflogo.php?group_id=161614&type=1
            :target: http://sourceforge.net

|sflogo|