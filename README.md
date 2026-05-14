# Gravity and Action from the Parabolic Metric Evolution of a Complex Manifold

**Donald Airey**
ORCID: 0000-0002-2958-1545
Cooperstown, NY, USA
Email: [don@airey.us](mailto:don@airey.us)

## Keywords

* cosmology
* gravitational theory
* cosmic expansion
* cosmological dynamics
* Newtonian cosmology
* Type Ia supernovae
* large-scale structure

---

# Abstract

We present a bilocal geometric framework in which separations are defined between ordered pairs of events rather than by a local infinitesimal metric. This construction is motivated by the need to represent global evolution in a manner that remains well-defined over finite separations while admitting a smooth local limit.

The resulting geometry is formulated on a complex manifold with an imaginary temporal coordinate and a real spatial coordinate. A constant manifold acceleration sets the global spatial scale and produces a parabolic cycle of expansion and contraction.

In the local reduction, the same acceleration scale yields a circular-orbit envelope consistent with the baryonic Tully–Fisher relation. At cosmological scales, the resulting analytic distance–redshift relation predicts the Pantheon+ Type Ia supernova luminosity distances on the SH0ES-calibrated absolute scale and yields a lower covariance-weighted χ² than Planck-calibrated FLRW, without invoking dark matter or dark energy.

The parabolic metric evolution, when combined with standard recombination microphysics, yields an acoustic angular scale consistent with Planck measurements.

![Complex Manifold](Manifold.png)

---

# Introduction

Cosmological observations tightly constrain theoretical descriptions of the universe. Measurements of the cosmic microwave background (CMB) fix early-universe conditions and global geometry with high precision, while Type Ia supernovae probe the late-time expansion history through the luminosity distance–redshift relation.

Although each dataset is internally consistent, discrepancies arise when parameters inferred from early- and late-time observations are compared. In particular, the tension in the Hubble constant indicates that the standard cosmological model may be incomplete.

Historically, such discrepancies have been addressed by extending the model. The cosmological constant was introduced to permit a static universe and abandoned following the discovery of expansion. Galaxy rotation curves motivated the introduction of non-baryonic dark matter, and supernova evidence for accelerated expansion led to the reintroduction of the cosmological constant as dark energy.

While these additions yield a phenomenologically successful framework, the dominant components of the cosmic energy budget remain physically unexplained.

We develop a kinematic framework in which large-scale evolution and local gravitational phenomena arise from a common geometric structure, termed the **Parabolic Metric Evolution (PME)**.

The PME framework replaces path-dependent metric integration with a bilocal definition assigning separations directly to ordered event pairs while admitting a consistent local limit.

Motion on the manifold is governed by a single intrinsic kinematic scale, eliminating the need for multiple independent cosmological parameters and linking global expansion and local dynamics to a common geometric origin.

---

# Bilocal Geometry

## Foundational Structure

The framework is defined by the following postulates:

1. Physical separations are defined bilocally between ordered pairs of events.
2. The manifold evolution is governed by a constant acceleration scale `A`.
3. The manifold is parameterized by an intrinsic evolution coordinate `χ`.
4. Observable time is defined operationally through null exchange.

The intrinsic evolution parameter is related to observable time by:

```math
χ = i t
```

All subsequent results follow from this structure.

---

## Bilocal Spatial Separation

The bilocal spatial interval is defined by:

```math
\frac{\Delta x_e^1}{L(t_e)} = \frac{\Delta x_o^1}{L(t_o)}
```

Using midpoint symmetry:

```math
\Delta s^1 = \frac12(\Delta x_o^1 + \Delta x_e^1)
```

---

## Invariance of the Bilocal Interval

The quadratic bilocal scalar is:

```math
\Delta s^2 = (\Delta s^0)^2 + (\Delta s^1)^2
```

where:

* `Δs⁰` is imaginary
* `Δs¹` is real

---

## Imaginary Velocity

With constant intrinsic acceleration `A`:

```math
v(t) = i(At - V_0)
```

where `V₀` is the initial expansion rate.

---

## Induced Spatial Evolution

The manifold extent is:

```math
L(t) = V_0 t - \frac12 A t^2
```

Differentiating twice:

```math
\frac{d^2L}{dt^2} = -A
```

Thus the manifold evolves with constant deceleration magnitude `A`.

---

# Cosmological Distance

## Redshift Relation

Redshift is defined by:

```math
1 + z = \frac{L(t_o)}{L(t_e)}
```

Using the manifold extent:

```math
L(t) = V_0 t - \frac12 A t^2
```

The resulting comoving distance relation is:

```math
D_C(z) = \frac{t_o(2V_0 - At_o)z}{2 + z}
```

---

# Causal Structure

The causal horizon is:

```math
d_{\mathrm{ch}}(t) = t(2V_0 - At)
```

Its expansion rate is:

```math
c_c(t) = 2(V_0 - At)
```

The causal horizon always satisfies:

```math
\frac{d_{\mathrm{ch}}(t)}{L(t)} = 2
```

Thus the entire last-scattering surface remains causally connected.

---

# Gravity

## Local Interval

In the coincidence limit:

```math
ds^2 = -(V_0 - At)^2dt^2 + dx^2
```

This defines the emergent local geometry.

---

## Acceleration Field

The inward acceleration decomposes as:

```math
a_{\mathrm{in}}(x) = a_{\mathrm{bg}} + a_{\mathrm{conc}}(x)
```

where:

* `a_bg` is the homogeneous background acceleration
* `a_conc` is the sourced concentration field

The sourced field satisfies:

```math
\nabla \cdot \mathbf a_{\mathrm{conc}} = -4\pi G\rho_{\mathrm{inertial}}
```

For spherical symmetry:

```math
\mathbf a_{\mathrm{conc}}(r) = -\frac{GM(r)}{r^2}\hat r
```

---

## Circular Orbits

The circular orbit relation is:

```math
v^2 = Ar + \frac{GM_b(r)}{r}
```

which yields:

```math
M_b(r) = \frac{r(v^2 - Ar)}{G}
```

The maximum mass envelope becomes:

```math
M_{\max}(v) = \frac{v^4}{4AG}
```

This reproduces the baryonic Tully–Fisher relation.

---

# Local Dynamics

## Operational Time

The null condition gives:

```math
(V_0 - At)^2\Delta t^2 = \Delta x^2
```

thus:

```math
\Delta t = \frac{\Delta x}{V_0 - At}
```

Observable time is defined operationally through null exchange.

---

## Proper Time

Proper time is defined by:

```math
d\tau^2 = (V_0 - At)^2dt^2 - dx^2
```

which yields:

```math
d\tau = (V_0 - At)\sqrt{1 - \frac{v^2}{(V_0 - At)^2}}dt
```

---

## Local Momentum

The observable velocity is:

```math
v = (V_0 - At)\tan\theta
```

Momentum is:

```math
P = mv
```

with null boundary at:

```math
\theta = \frac\pi4
```

---

## Local Action

Define the geometric momentum scale:

```math
P_{\mathrm{geom}} = m(V_0 - At)
```

The invariant geometric action increment is:

```math
dS_{\mathrm{geom}} = P_{\mathrm{geom}}ds
```

with action-space interval:

```math
dS_{\mathrm{geom}}^2 = m^2(V_0 - At)^2[-(V_0 - At)^2dt^2 + dx^2]
```

The geometric energy scale is:

```math
E_{\mathrm{geom}}(t) = -m(V_0 - At)^2
```

Observable action is:

```math
dS = Pdx - Hdt
```

---

## Phase Evolution

Beyond the null boundary, geometric evolution continues as phase:

```math
\phi = \frac{S_{\mathrm{geom}}}{\hbar}
```

where `ħ` defines the minimum bilocal separation scale.

---

# Late-Time Evolution

## Luminosity Distance

The luminosity distance is:

```math
D_L(z) = -\frac{t_o(At_o - 2V_0)z(1+z)}{2+z}
```

Distance modulus:

```math
\mu(z) = 5\log_{10}\left(\frac{D_L(z)}{10\,\mathrm{pc}}\right)
```

---

## PME Parameters

| Parameter | Value               |
| --------- | ------------------- |
| `A`       | `3.7 × 10⁻¹¹ m s⁻²` |
| `V₀`      | `3.16 × 10⁸ m s⁻¹`  |
| `t₀`      | `4.51 × 10¹⁷ s`     |

Predicted Hubble constant:

```math
H_0 = 66.5\,\mathrm{km\,s^{-1}\,Mpc^{-1}}
```

---

# Early-Time Evolution

## Scale Factor

```math
a(t) = \frac{L(t)}{L(t_o)}
```

---

## Recombination Epoch

Using PME expansion geometry with standard recombination microphysics yields:

* recombination redshift: `z* = 1039`
* recombination time: `t* = 13.4 Myr`

---

## Acoustic Angular Scale

The predicted acoustic angle is:

```math
\theta_* = 0.0103
```

or conventionally:

```math
100\theta_* = 1.03
```

consistent with Planck observations.

---

# Discussion

PME proposes a unified geometric origin for:

* cosmological expansion
* gravity
* inertia
* action
* causal structure
* phase evolution

The framework:

* eliminates dark matter and dark energy components
* reproduces Type Ia supernova luminosity distances
* predicts the Hubble constant
* reproduces the baryonic Tully–Fisher relation
* predicts the acoustic angular scale
* removes curvature singularities through finite acceleration flux

The theory remains to be extended to:

* perturbation growth
* structure formation
* intrinsic recombination derivations
* nucleosynthesis

---

# Code Availability

Computational notebook:

[https://www.wolframcloud.com/obj/32b2e831-2cbe-4ff5-b821-aa23f476f015](https://www.wolframcloud.com/obj/32b2e831-2cbe-4ff5-b821-aa23f476f015)

---

# Conclusion

The Parabolic Metric Evolution framework defines a bilocal geometric structure in which evolution, gravity, inertia, causal structure, and dynamical law emerge from a common acceleration geometry.

The framework derives:

* cosmological expansion
* local gravitational structure
* baryonic Tully–Fisher scaling
* Type Ia supernova luminosity relations
* the Hubble constant
* the acoustic angular scale

from a single acceleration scale inherited from the manifold geometry.

This construction provides a unified geometric interpretation of cosmological and local dynamics without introducing independent dark-sector components.
