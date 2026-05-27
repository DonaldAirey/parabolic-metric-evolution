<h1 align="center">Gravity and Action from the Evolution of a Complex Manifold</h1>

<p align="center">
  <a href="https://doi.org/10.5281/zenodo.20414999">
    <img src="https://zenodo.org/badge/1238949153.svg" alt="DOI">
  </a>
</p>

<p align="center">
  <strong>Parabolic Metric Evolution (PME)</strong> &mdash; an alternative cosmological framework
  that derives gravity, the Hubble constant, and galaxy rotation curves from a single acceleration scale,
  without invoking dark matter or dark energy.
</p>

<hr>

<h2>Overview</h2>

<p>
This repository accompanies the paper <em>Gravity and Action from the Evolution of a Complex Manifold</em>,
which develops the Parabolic Metric Evolution (PME) framework as an alternative to standard FLRW cosmology.
PME addresses the Hubble tension, galaxy rotation curves, and the baryonic Tully&ndash;Fisher relation
through a single geometric construction grounded in a complex manifold with a constant acceleration scale.
The framework reproduces key cosmological and galactic observations without introducing dark matter,
dark energy, or any independent dynamical components.
</p>

<h3>Highlights</h3>

<ul>
  <li>Fits the Pantheon+ Type Ia supernova distances on the SH0ES-calibrated absolute scale with substantially lower covariance-weighted &chi;<sup>2</sup> than Planck-calibrated FLRW.</li>
  <li>Predicts the present-day Hubble constant <em>H<sub>0</sub></em> = 66.5 km s<sup>&minus;1</sup> Mpc<sup>&minus;1</sup> as a derived quantity rather than a fitted parameter.</li>
  <li>Reproduces the baryonic Tully&ndash;Fisher relation from the SPARC galaxy sample using the same acceleration scale <em>A</em> = 3.7&times;10<sup>&minus;11</sup> m s<sup>&minus;2</sup>.</li>
  <li>Yields a CMB acoustic angular scale 100&theta;<sub>*</sub> = 1.03, consistent with Planck measurements.</li>
  <li>Produces uniformly extended cosmic ages, easing tension with early massive-galaxy observations.</li>
</ul>

<h3>Repository Contents</h3>

<ul>
  <li><code>Gravity and Action from the Evolution of a Complex Manifold.pdf</code> &mdash; full manuscript.</li>
  <li><code>figures/</code> &mdash; figures referenced in the manuscript and this README (manifold schematic, BTFR plot, Hubble diagram, visibility function, fundamental plane).</li>
  <li><code>notebooks/</code> &mdash; Wolfram Language notebooks reproducing the bilocal geometry, distance&ndash;redshift relation, BTFR fit to SPARC data, and Pantheon+ comparison.</li>
  <li><code>CITATION.cff</code> &mdash; structured citation metadata.</li>
  <li><code>LICENSE</code> &mdash; GPL-3.0 license.</li>
</ul>

<hr>

<h2>Abstract</h2>

<p>
We present a bilocal geometric framework in which separations are defined between ordered pairs of events rather than by a local infinitesimal metric. This construction is motivated by the need to represent global evolution in a manner that remains well-defined over finite separations while admitting a smooth local limit.
</p>

<p>
The resulting geometry is formulated on a complex manifold with an imaginary temporal coordinate and a real spatial coordinate. A constant manifold acceleration sets the global spatial scale and produces a parabolic cycle of expansion and contraction.
</p>

<p>
In the local reduction, the same acceleration scale yields a circular-orbit envelope consistent with the baryonic Tully–Fisher relation. At cosmological scales, the resulting analytic distance–redshift relation predicts the Pantheon+ Type Ia supernova luminosity distances on the SH0ES-calibrated absolute scale and yields a lower covariance-weighted $\chi^2$ than Planck-calibrated FLRW, without invoking dark matter or dark energy.
</p>

<p>
The parabolic metric evolution, when combined with standard recombination microphysics, yields an acoustic angular scale consistent with Planck measurements.
</p>

<p align="center">
  <img src="figures/pme-manifold.png" alt="Complex parabolic metric manifold" width="500">
</p>

<p align="center">
  <em>
    Figure 1 - Schematic representation of the complex parabolic metric manifold.
    Latitude lines correspond to spatial slices at fixed epoch,
    while longitude lines trace the temporal evolution of the manifold.
  </em>
</p>

<hr>

<h2>Introduction</h2>

<p>
Cosmological observations tightly constrain theoretical descriptions of the universe. Measurements of the cosmic microwave background (CMB) fix early-universe conditions and global geometry with high precision, while Type Ia supernovae (SNe Ia) probe the late-time expansion history through the luminosity distance–redshift relation. Although each dataset is internally consistent, discrepancies arise when parameters inferred from early- and late-time observations are compared. In particular, the tension in the Hubble constant indicates that the standard cosmological model may be incomplete.
</p>

<p>
Historically, such discrepancies have been addressed by extending the model. The cosmological constant was introduced to permit a static universe and abandoned following the discovery of expansion. Galaxy rotation curves motivated the introduction of non-baryonic dark matter, and supernova evidence for accelerated expansion led to the reintroduction of the cosmological constant as dark energy. While these additions yield a phenomenologically successful framework, the dominant components of the cosmic energy budget remain physically unexplained. More recent approaches introduce additional degrees of freedom, including time-varying dark energy, further increasing the parametric structure of the model.
</p>

<p>
We develop a kinematic framework in which large-scale evolution and local gravitational phenomena arise from a common geometric structure, termed the Parabolic Metric Evolution (PME). Local metric descriptions specify infinitesimal separations, so finite separations between distant events must be constructed by integrating along a chosen connection; in a globally evolving system, this construction can depend on both the path and the evolution of the geometry. The PME framework replaces this path-dependent procedure with a bilocal definition that assigns separations directly to ordered event pairs while admitting a consistent local limit. Motion on the manifold is governed by a single intrinsic kinematic scale, eliminating the need for multiple independent cosmological parameters and linking global expansion and local dynamics to a common geometric origin.
</p>

<p>
This approach differs from relativistic metric gravity in its bilocal definition of separation and from modified-gravity models in that the characteristic acceleration scale is not introduced phenomenologically but inherited from the global manifold kinematics by the local-reduction regime. Cosmological evolution, gravity, and the laws governing motion are thereby unified through a single acceleration scale determined by the manifold kinematics.
</p>

<p>
The resulting construction defines a minimal kinematic closure: the lowest-order geometric structure that consistently relates finite separations, global evolution, and local dynamics within a single framework, without introducing independent dynamical components. The bilocal definition of separation provides a representation of finite intervals compatible with global evolution, and the restriction to a single intrinsic acceleration scale selects the simplest nontrivial homogeneous dynamics beyond uniform motion, yielding a closed and self-consistent description across cosmological and local regimes.
</p>

<hr>

<h2>Bilocal Geometry</h2>

<h3>Foundational Structure</h3>

<p>The framework is defined by the following postulates:</p>

<ol>
  <li>Physical separations are defined bilocally between ordered pairs of events.</li>
  <li>The manifold evolution is governed by a constant acceleration scale $A$.</li>
  <li>The manifold is parameterized by an intrinsic evolution coordinate $\chi$.</li>
  <li>Observable time is defined operationally through null exchange, providing an invariant ordering of events. The intrinsic evolution parameter is related to this observable time by the projection $\chi = it$, which fixes the real–imaginary decomposition of temporal and spatial functionals and serves as a defining structural postulate of the framework.</li>
</ol>

<p>All subsequent results follow from this structure.</p>

<h3>Bilocal Spatial Separation</h3>

<p>
Let $p_e=(x_e^0,x_e^1)$ denote an emission event and $p_o=(x_o^0,x_o^1)$ an observation event, with the bilocal interval constructed from a temporal functional obtained from accumulated evolution between slices and a spatial functional defined from separations on the emission and observation slices.
</p>

<p>
The spatial slices scale with a global manifold extent $L(t)$, so the separations at emission and observation satisfy
</p>

<p>

$$\frac{\Delta x_e^1}{L(t_e)}=\frac{\Delta x_o^1}{L(t_o)}$$

</p>

<p>
Imposing symmetry under interchange of emission and observation together with a smooth coincidence limit motivates adopting the midpoint average as the minimal symmetric choice,
</p>

<p>

$$\Delta s^1=\Delta x_o^1-\frac12(\Delta x_o^1-\Delta x_e^1)$$

</p>

<p>

$$\Delta s^1=\frac12(\Delta x_o^1+\Delta x_e^1)$$

</p>

<p align="center">
  <img src="figures/invariant-interval.png" alt="Bilocal geometry construction" width="500">
</p>

<p align="center">
Geometric construction of the bilocal interval between emission event $p_e$ and observation event $p_o$, showing the accumulated temporal evolution and the symmetric midpoint spatial separation between scaled slices.
</p>

<h3>Invariance of the Bilocal Interval</h3>

<p>
Consider a bilocal scalar constructed from the temporal and spatial endpoint functionals $(\Delta s^0,\Delta s^1)$. We adopt a quadratic form as the lowest-order scalar consistent with finite separations, ensuring that the local reduction yields a well-defined null condition while avoiding higher-order dependence on endpoint structure,
</p>

<p>

$$\Delta s^2 = a\,(\Delta s^0)^2 + b\,(\Delta s^1)^2 + 2c\,\Delta s^0 \Delta s^1$$

</p>

<p>
Under interchange of the ordered endpoints $(p_e,p_o)$, the temporal functional changes sign while the symmetric spatial functional does not, so the mixed term changes sign. Invariance therefore requires $c=0$.
</p>

<p>
In the local reduction, sufficiently small endpoint separations render the temporal and spatial functionals linear in the coordinate increments. The null condition must define a finite null ratio, which requires both temporal and spatial contributions to enter non-degenerately so that the null condition defines a finite null ratio. The interval therefore reduces to
</p>

<p>

$$\Delta s^2 = a\,(\Delta s^0)^2 + b\,(\Delta s^1)^2$$

</p>

<p>
The remaining quadratic form is constrained up to a positive overall factor and a relative scaling between the temporal and spatial functionals. These functionals are identified with the canonical imaginary and real components of the complex manifold, with this identification fixing their relative normalization. The bilocal interval is therefore
</p>

<p>

$$\Delta s^2 = (\Delta s^0)^2 + (\Delta s^1)^2$$

</p>

<p>
with $\Delta s^0$ purely imaginary and $\Delta s^1$ real.
</p>

<h3>Imaginary Velocity</h3>

<p>
The intrinsic evolution of the manifold is parameterized by a coordinate $\chi$. Observable time is introduced by the projection $\chi = it$, so that $d\chi = i\,dt$, fixing the real–imaginary decomposition used in the bilocal construction.
</p>

<p>
With constant intrinsic acceleration $A$, the velocity scale along the manifold history follows from integration with respect to $\chi$,
</p>

<p>

$$v(t) = \int A\, d\chi$$

</p>

<p>
Substituting $d\chi = i\,dt$ gives $v(t) = i\!\int A\,dt$, which evaluates to
</p>

<p>

$$v(t) = i(At - V_0)$$

</p>

<p>
where $V_0$ is an integration constant representing the initial expansion rate of the manifold.
</p>

<h3>Induced Spatial Evolution</h3>

<p>
The observable spatial extent arises from integrating the imaginary velocity along the imaginary temporal direction. The global spatial scale of the manifold is therefore $L(t) \equiv \int v(t)\, d\chi$. Substituting the expression for $v(t)$ and using $d\chi = i\,dt$ gives $L(t) = \int i(At - V_0)\, i\, dt$. Evaluating the integral yields
</p>

<p>

$$L(t) = V_0 t - \frac{1}{2} A t^2$$

</p>

<h3>Manifold Deceleration</h3>

<p>
The intrinsic evolution is defined along $\chi$, while observable dynamics are expressed in the projected time coordinate $t$ with $d\chi = i\,dt$. Rewriting the manifold extent in terms of $t$ yields its observable form. Differentiating twice with respect to $t$ gives
</p>

<p>

$$\frac{d^2 L}{dt^2} = -A$$

</p>

<p>
so the manifold extent evolves with a constant kinematic deceleration of magnitude $A$, which is universal and independent of position or epoch.
</p>

<hr>

<h2>Cosmological Distance</h2>

<p>
Observable cosmological distances follow from the bilocal interval defined above.
</p>

<h3>Temporal Separation</h3>

<p>
The temporal component of the bilocal interval is obtained from the accumulated tangent evolution along the manifold history between the emission and observation parameters $t_e$ and $t_o$, $\Delta s^0 \equiv \int_{t_e}^{t_o} v(t)\,dt$. Substituting the imaginary velocity gives
</p>

<p>

$$\Delta s^0 = \int_{t_e}^{t_o} i\left(A t - V_0\right)\,dt$$

</p>

<p>
Evaluating the integral yields
</p>

<p>

$$\Delta s^0 = i\left(\frac{A}{2}\left(t_o^2 - t_e^2\right) - V_0\left(t_o - t_e\right)\right)$$

</p>

<p>
The temporal separation is purely imaginary and depends only on the endpoints.
</p>

<h3>Spatial Separation</h3>

<p>
Because spatial slices scale with the manifold extent $L(t)$ and the slice separations satisfy the bilocal scaling relation, the spatial component becomes
</p>

<p>

$$\Delta s^1 =\frac{\Delta x_o^1}{2}\left(1 +\frac{V_0 t_e - \frac{1}{2} A t_e^2}{V_0 t_o - \frac{1}{2} A t_o^2}\right)$$

</p>

<h3>Bilocal Metric Formula</h3>

<p>
Substituting the temporal and spatial separations into the bilocal interval yields the interval relating the emission and observation events,
</p>

<p>

$$\Delta s^2 = \left[i\left(\frac{A}{2}\left(t_o^2 - t_e^2\right) - V_0\left(t_o - t_e\right)\right)\right]^2+ \left[\frac{\Delta x_o^1}{2}\left(1 + \frac{V_0 t_e - \frac{1}{2}A t_e^2}{V_0 t_o - \frac{1}{2}A t_o^2}\right)\right]^2$$

</p>

<h3>Redshift Relation</h3>

<p>
Redshift is defined observationally by the ratio of observed to emitted wavelength,
</p>

<p>

$$1+z \equiv \frac{\lambda_o}{\lambda_e}$$

</p>

<p>
We identify wavelength with a comoving spatial separation and assume that such separations scale with the manifold extent, so that $\lambda(t) \propto L(t)$,
</p>

<p>

$$1+z = \frac{L(t_o)}{L(t_e)}$$

</p>

<p>
Using the manifold extent, the emission epoch $t_e$ is expressed in terms of $t_o$ and the observed redshift $z$,
</p>

<p>

$$t_e = \frac{V_0(1+z) - \sqrt{(1+z)\big[(V_0 - A t_o)^2 + V_0^2 z\big]}}{A(1+z)}$$

</p>

<p>
where the negative branch is chosen so that $t_e < t_o$. Substituting into the bilocal metric and imposing the null condition $\Delta s^2 = 0$ yields the observable spatial separation,
</p>

<p>

$$D_C(z)= \frac{t_o\left(2V_0 - A t_o\right) z}{2 + z}$$

</p>

<hr>

<h2>Causal Structure</h2>

<p>
The null structure of the bilocal interval also determines the extent of causal connectivity on the manifold. The largest spatial separation permitted by null ordering is obtained with the emission event at the origin of the manifold history, $t_e = 0$, and the observation event at epoch $t_o = t$. Solving the null condition $\Delta s^2 = 0$ for the observed separation gives the causal horizon
</p>

<p>

$$d_{\mathrm{ch}}(t) = t\left(2V_0 - A t\right)$$

</p>

<p>
Differentiating the causal horizon gives the expansion rate of the causal boundary,
</p>

<p>

$$c_{\mathrm{c}}(t)=\frac{d}{dt}\,d_{\mathrm{ch}}=2\left(V_0-At\right)$$

</p>

<p>
This quantity defines the rate at which the accessible causal domain can be extended under the operational clock, and therefore characterizes the growth of the causally orderable region.
</p>

<p>
Comparing the causal horizon with the manifold extent $L(t)$ yields
</p>

<p>

$$\frac{d_{\mathrm{ch}}(t)}{L(t)} = 2$$

</p>

<p>
The causal horizon is therefore twice the manifold extent at all epochs, placing the entire last-scattering surface within a single causal region. Because the homogeneous manifold acceleration introduces no preferred direction, the large-scale isotropy of the cosmic microwave background follows directly from the geometry.
</p>

<hr>

<h2>Gravity</h2>

<p>
When the temporal interval between neighboring events is small compared with the characteristic evolution scale of the manifold extent $L(t)$, the bilocal construction admits a smooth local reduction yielding an effective acceleration field inherited from the manifold kinematics.
</p>

<h3>Coincidence Limit</h3>

<p>
The local description is obtained as the coincidence limit of the bilocal interval as the endpoint separation tends to zero. Let the observation event occur at epoch $t$ and the emission event at $t-\Delta t$, with $\Delta t \to 0$. Using the local expansion of the manifold extent,
</p>

<p>

$$L(t-\Delta t)=L(t)-\dot L(t)\,\Delta t-\frac{1}{2}A\,\Delta t^2$$

</p>

<p>
the bilocal spatial component reduces to leading order in $\Delta t$ as $\Delta s^1 \approx \Delta x_o^1$, and the temporal component becomes
</p>

<p>

$$\Delta s^0 \approx i\left(V_0-At\right)\Delta t$$

</p>

<p>
Substituting these leading terms into the bilocal interval yields the emergent local interval,
</p>

<p>

$$\Delta s^2 \approx -\left(V_0-At\right)^2\Delta t^2 + (\Delta x_o^1)^2$$

</p>

<p>
The local interval therefore defines a tangent of fixed magnitude $V_0-At$ shared by all trajectories at epoch $t$, whose projections onto orthogonal temporal and spatial components give rise to timelike, null, and spacelike directions.
</p>

<h3>Acceleration Field</h3>

<p>
Expanding the manifold extent about a reference epoch $t_0$ gives
</p>

<p>

$$L(t_0+\delta t)=L(t_0)+\dot{L}(t_0)\,\delta t+\frac{1}{2}\ddot{L}(t_0)\,\delta t^2+\cdots$$

</p>

<p>
The quadratic term is governed by the constant local value $\ddot{L}(t_0)=-A$. The local reduction therefore contains a homogeneous second-order contribution corresponding to a uniform deceleration of magnitude $A$ inherited from the global manifold evolution, which provides the physical origin of gravity in the local limit. This uniform deceleration defines the background acceleration field underlying local gravitational dynamics.
</p>

<p>
The effective inward acceleration in a bound system decomposes into a homogeneous background and a sourced concentration,
</p>

<p>

$$a_{\mathrm{in}}(x)=a_{\mathrm{bg}}+a_{\mathrm{conc}}(x)$$

</p>

<p>
The background term $a_{\mathrm{bg}}$ is uniform and has constant magnitude $A$. In the absence of localized content, it defines the manifold evolution, and an inertial frame follows it without inducing concentration or depletion. Localized inertial content, however, resists this acceleration, redistributing the flux into spatial concentrations that define the sourced gravitational component $a_{\mathrm{conc}}(x)$ governing bound dynamics. The inertial parameter $m$ entering this redistribution is the same quantity that weights the invariant separation in the construction of geometric action, so that the gravitational response corresponds to a redistribution of the inertia-weighted action-space separation underlying the local geometry.
</p>

<h3>Minimal Local Closure</h3>

<p>
The bilocal construction fixes the homogeneous background acceleration scale $A$ through the second-order local reduction of the manifold extent but does not determine the sourced concentration arising from spatial variations in inertial resistance. A weak-field closure is therefore required.
</p>

<p>
We adopt a minimal closure as the lowest-order local form consistent with locality, linearity in enclosed inertial content, rotational invariance, and additivity. These conditions restrict the sourced field to a divergence relation as the leading-order connection between field structure and inertial content, rather than an assumed inverse-square form. The concentration field therefore satisfies a divergence proportional to a local inertial density, with enclosed content given by its volume integral. In the weak-field limit, this density is dominated by rest mass and reduces to the baryonic density. All intrinsic kinematic scales are fixed by the acceleration scale $A$, while the constant $G$ sets the coupling to localized inertial content without introducing an additional kinematic scale.
</p>

<p>
For a spherically symmetric configuration the flux through a sphere of radius $r$ is
</p>

<p>

$$\Phi(r)=\oint_S \mathbf a_{\mathrm{conc}}\cdot d\mathbf S=4\pi r^2 a_r(r)$$

</p>

<p>
Imposing flux conservation together with linearity in the enclosed inertial content gives
</p>

<p>

$$\oint_S \mathbf a_{\mathrm{conc}}\cdot d\mathbf S = -4\pi G M(r)$$

</p>

<p>
where $M(r)$ is the enclosed inertial content within radius $r$, obtained from the local density by $M(r)=\int_V \rho_{\mathrm{inertial}}\,dV$, and $G$ is the empirical coupling relating inertial content to concentration of the background acceleration. Spherical symmetry then yields
</p>

<p>

$$\mathbf a_{\mathrm{conc}}(r)=-\frac{G M(r)}{r^2}\,\hat r$$

</p>

<p>
and Gauss's theorem gives the Poisson equation for the sourced weak-field limit,
</p>

<p>

$$\nabla\!\cdot \mathbf{a}_{\mathrm{conc}} = -4\pi G \rho_{\mathrm{inertial}}$$

</p>

<p>
In the weak-field regime relevant for galactic dynamics, the inertial density is dominated by baryonic rest-mass contributions, so $\rho_{\mathrm{inertial}}\approx\rho_b$.
</p>

<h3>Circular Orbits</h3>

<p>
For a body in a circular orbit of radius $r$ with tangential speed $v$, the required centripetal acceleration is $a_{\mathrm{cent}}(r) = -v^2/r$. Equating this with the inward acceleration from the decomposition above and multiplying by $r$ gives $v^2 = A r + G M_b(r)/r$. Solving for the enclosed baryonic mass gives
</p>

<p>

$$M_b(r) = \frac{r\left(v^2 - A r\right)}{G}$$

</p>

<h3>Circular-Orbit Solutions</h3>

<p>
The equation above defines the PME fundamental plane, a two-parameter family of circular-orbit solutions relating baryonic mass $M$, orbital radius $r$, and orbital speed $v$. For fixed orbital speed $v$, the mass function $M(r)$ is a concave quadratic in $r$. The mass therefore reaches a maximum at
</p>

<p>

$$r_{\max} = \frac{v^2}{2A}$$

</p>

<p>
Substituting this radius into the mass–radius relation yields the maximum baryonic mass compatible with a circular orbit at speed $v$,
</p>

<p>

$$M_{\max}(v) = \frac{v^4}{4 A G}$$

</p>

<p>
The surface $M(v,r)$ therefore defines a fundamental plane of circular-orbit solutions, with the ridge $M_{\max}(v)$ giving the upper envelope of baryonic mass for a given orbital speed. Galaxies dominated by circular rotation are expected to saturate this boundary and follow a characteristic mass–velocity relation.
</p>

<p align="center">
  <img src="figures/fundamental-plane.png" alt="PME fundamental plane" width="700">
</p>

<p align="center">
  <em>
    PME fundamental plane. The baryonic mass surface $M(v,r)$ is shown as a function of orbital speed $v$ and
    orbital radius $r$ for an illustrative manifold acceleration scale $A = 10^{-11}\ \mathrm{m\,s^{-2}}$.
    The red ridge marks the locus $M_{\max}(v)$ corresponding to the maximum baryonic mass permitted by the
    manifold kinematics at each orbital speed. Galaxies populating this ridge reproduce the baryonic
    Tully–Fisher relation.
  </em>
</p>

<h3>Baryonic Tully–Fisher Relation</h3>

<p>
$M_{\max}(v)$ defines the scaling $M \propto v^4$, consistent with the observed baryonic Tully–Fisher relation. A characteristic acceleration scale in galaxy dynamics has previously been emphasized in frameworks such as MOND, in which the force law is modified to reproduce Tully–Fisher-type scaling.
</p>

<p>
The manifold acceleration $A$ is determined empirically by fitting the circular-orbit envelope to the SPARC galaxy sample of McGaugh, Lelli and Schombert, using the assumptions $\Upsilon_\star=0.5$, $f_{\mathrm{gas}}=1.33$, zero intrinsic mass-to-light uncertainty, and the quality cut $\mathrm{Qual}\leq 3$. These rotationally supported disk systems are well suited to the analysis, as their kinematics closely follow the circular-orbit approximation.
</p>

<p>
For each galaxy the rotation curve provides an asymptotic circular velocity $v$, while the baryonic mass $M_b$ is computed as $M_b=\Upsilon_\star L_{3.6}+f_{\mathrm{gas}}\,M_{\mathrm{HI}}$. The value of $A$ is determined by minimizing the $\chi^2$ statistic between the theoretical envelope and the observed $(M_b,v)$ pairs. The best-fit manifold acceleration is
</p>

<p>

$$A = 3.7\times10^{-11}\ \mathrm{m\,s^{-2}}$$

</p>

<p>
The observed galaxies follow the predicted $M\propto v^4$ scaling across a wide range of baryonic masses and rotational velocities. The baryonic Tully–Fisher relation is a direct consequence of the constant-acceleration structure of the manifold and an observational signature of the acceleration flux.
</p>

<p align="center">
  <img src="figures/btfr-plot.png" alt="Baryonic Tully–Fisher relation" width="500">
</p>

<p align="center">
  <em>
    Log–log plot of baryonic mass $M_b$ versus outer rotation speed $v$ for the SPARC galaxy sample of
    McGaugh, Lelli and Schombert. Black circles show the observed galaxies. The solid red line shows the
    PME circular-orbit envelope evaluated at the best-fit acceleration.
  </em>
</p>

<h3>Global Acceleration Budget</h3>

<p>
The local closure fixes all non-homogeneous acceleration flux as sourced by inertial content. In the weak-field regime this reduces to baryonic mass. Integrating the flux law over the full homogeneous domain of scale $L$ and using the global relation between baryonic mass and the background acceleration scale,
</p>

<p>

$$M_b^{\mathrm{tot}}=\frac{A L^2}{G}$$

</p>

<p>
yields
</p>

<p>

$$\Phi_{\mathrm{tot}}=-4\pi A L^2$$

</p>

<p>
The available concentration flux is fixed by the background scale $A$ and is completely accounted for by baryonic mass. Local gravitational systems therefore correspond to partial redistributions of a finite acceleration budget, so gravitational collapse approaches a saturated configuration rather than an unbounded one.
</p>

<h3>Mach's Bucket</h3>

<p>
The bilocal reduction introduces a homogeneous acceleration scale $A$ fixed by the geometry of the manifold. This acceleration is not sourced by baryonic matter; instead, baryonic mass redistributes it through conservation of acceleration flux.
</p>

<p>
For a rotating system of radius $r$ and tangential speed $v$, circular motion requires an inward centripetal acceleration $v^{2}/r$. In this framework, that requirement is met by redistributing the background field to produce the necessary inward concentration.
</p>

<p>
Because the total acceleration is finite, this redistribution cannot be local: any concentration within the system must be balanced globally. Rotational inertia therefore depends on the global distribution of mass through the shared acceleration field, providing a Machian interpretation.
</p>

<h3>Regularity of the Manifold</h3>

<p>
Because the manifold acceleration scale is finite, collapse approaches saturated configurations of finite density and radius rather than singular limits. The manifold accordingly remains smooth under the evolution defined by the geometry and does not admit singular collapse.
</p>

<p>
Causal ordering is fixed by the intrinsic geometry of allowable separations, not by any imposed signal speed. Only trajectories consistent with this ordering admit an operational time parameter, excluding closed timelike curves and the associated causal paradoxes. The causal structure and finite acceleration budget thereby avoid singularities and causal paradoxes.
</p>

<hr>

<h2>Local Dynamics</h2>

<p>
Having established the gravitational and causal structure, we now define the operational dynamics governing motion within the manifold.
</p>

<h3>Operational Time</h3>

<p>
Imposing the null condition $\Delta s^2=0$ on the local interval gives
</p>

<p>

$$(V_0 - At)^2 \Delta t^2=\Delta x^2$$

</p>

<p>
so that
</p>

<p>

$$\Delta t=\frac{\Delta x}{(V_0 - At)}$$

</p>

<p>
This defines the null boundary of the local geometry and fixes the relation between spatial separation and temporal increment through the scale $(V_0 - At)$.
</p>

<p>
Observable time is defined operationally by null exchange between nearby worldlines. One tick of the clock is a complete round trip of a signal along null trajectories, and the temporal parameter $t$ is identified with the number of such cycles, which defines an invariant ordering of events. The null relation ensures that each cycle corresponds to a temporal increment determined by the local scale $(V_0 - At)$ at that epoch, and restricts admissible trajectories to those consistent with this ordering.
</p>

<p>
The null relation therefore fixes the local causal structure and operational ordering of events. Observable motion and the invariant timelike interval both arise from this same local geometry, so causality, motion, and measurable duration are unified through the null structure of the manifold.
</p>

<h3>Proper Time</h3>

<p>
Using the local interval, proper time defines the invariant timelike interval along admissible trajectories, $d\tau^2 \equiv -ds^2$, so that
</p>

<p>

$$d\tau^2 = (V_0 - At)^2\,dt^2 - dx^2$$

</p>

<p>
giving
</p>

<p>

$$d\tau = (V_0 - At)\sqrt{1 - \frac{v^2}{(V_0 - At)^2}}\;dt$$

</p>

<p>
where $v = dx/dt$.
</p>

<h3>Local Momentum</h3>

<p>
A non-zero manifold acceleration defines a global acceleration flux that selects a timelike direction. In the homogeneous local limit, the orientation relative to the flux is represented by an angle $\theta$. Resolving the tangent via the local invariant, the orthogonal projections admit a representation yielding
</p>

<p>

$$dx = (V_0 - At)\sin\theta\,d\lambda,\qquad dt = \cos\theta\,d\lambda$$

</p>

<p>
The measurable velocity may be expressed as
</p>

<p>

$$v = \frac{dx}{dt} = (V_0 - At)\tan\theta$$

</p>

<p>
The null boundary is reached when $v = V_0 - At$, which requires $\tan\theta = 1$ and therefore $\theta = \pi/4$. Observable motion is accordingly restricted to the timelike domain $0 \le \theta < \pi/4$. At this boundary, the underlying geometric structure remains well-defined through the orientation angle $\theta$, but the kinematic description in terms of $t$ ceases to apply. Beyond this limit, the projection geometry persists but no longer corresponds to observable motion; its continuation is defined in terms of phase evolution.
</p>

<p>
Momentum is defined from the observable velocity,
</p>

<p>

$$P = m\,v$$

</p>

<p>
and is the spatial projection of the geometric momentum scale $m(V_0-At)$ with respect to the temporal parameter $t$.
</p>

<h3>Local Action</h3>

<p>
In the coincidence limit, weighting the invariant separation $ds$ by the tangent momentum scale $P_{\mathrm{geom}} \equiv m(V_0-At)$ defines the invariant geometric action increment $dS_{\mathrm{geom}} \equiv P_{\mathrm{geom}}\,ds$, with quadratic form
</p>

<p>

$$dS_{\mathrm{geom}}^2 = P_{\mathrm{geom}}^2\,ds^2 = m^2(V_0-At)^2\left[-(V_0-At)^2 dt^2 + dx^2\right]$$

</p>

<p>
The temporal component defines the geometric energy scale associated with tangent evolution,
</p>

<p>

$$E_{\mathrm{geom}}(t)\equiv -m(V_0-At)^2$$

</p>

<p>
while the spatial component is governed by the geometric momentum scale $P_{\mathrm{geom}}=m(V_0-At)$. Evaluating the local interval on the tangent direction gives $ds=(V_0-At)\,d\lambda$, so that
</p>

<p>

$$dS_{\mathrm{geom}} = m(V_0-At)^2\,d\lambda$$

</p>

<p>
and the invariant geometric action accumulates along the manifold tangent as $S_{\mathrm{geom}} = \int dS_{\mathrm{geom}}$.
</p>

<p>
Observable action is obtained by projection into the timelike sector,
</p>

<p>

$$dS = P\,dx - H\,dt$$

</p>

<p>
which defines the canonical momentum and observable Hamiltonian. The observable action therefore plays the role of the Hamilton–Jacobi principal function, while the invariant geometric action remains well-defined across the full manifold.
</p>

<h3>Phase Evolution</h3>

<p>
The projection-based kinematic description applies within the timelike sector, where the local invariant defines a real proper-time interval. At the null boundary, $ds^2=0$ and $d\tau \to 0$, marking the limit of observable timelike motion. Beyond this boundary, observable motion ceases, while the invariant geometric structure remains well-defined and the geometric action continues to accumulate along the manifold tangent.
</p>

<p>
The continued evolution of this invariant scalar is represented as phase,
</p>

<p>

$$\phi = \frac{S_{\mathrm{geom}}}{\hbar}$$

</p>

<p>
where $\hbar$ sets the scale relating geometric action to phase. Because action has units of length within the present framework, $\hbar$ acquires the interpretation of a minimum indivisible bilocal separation — a necessary structural feature of a geometry that does not admit infinitesimal separations.
</p>

<p>
Phase evolution therefore represents the continuation of invariant geometric evolution beyond the proper-time-parametrized sector, while the underlying manifold evolution remains continuous across the null boundary.
</p>

<hr>

<h2>Late-Time Evolution</h2>

<p>
The distance–redshift relation derived from the bilocal interval predicts the late-time expansion history.
</p>

<h3>Type Ia Supernova Sample</h3>

<p>
We use the Pantheon+ compilation of 1701 spectroscopically confirmed Type Ia supernovae presented by Brout et al. The publicly released Pantheon+SH0ES dataset provides the observed distance moduli $\mu_{\mathrm{obs}}$, redshifts $z$, and the full STAT+SYS covariance matrix for covariance-weighted $\chi^2$ inference. The distance moduli are absolutely calibrated through the SH0ES determination of the Type Ia absolute magnitude $M_B$.
</p>

<h3>Luminosity Distance</h3>

<p>
The luminosity distance follows from the standard relation $D_L(z) = (1+z)D_C(z)$. Substituting the spatial separation yields the corresponding analytic luminosity distance
</p>

<p>

$$D_L(z) =-\frac{t_o\left(A t_o - 2V_0\right) z(1+z)}{2+z}$$

</p>

<h3>Distance Modulus</h3>

<p>
Type Ia supernova observations are reported in terms of the distance modulus, which relates the observed luminosity distance to the measured brightness of each supernova,
</p>

<p>

$$\mu(z) = 5\log_{10}\!\left(\frac{D_L(z)}{10\ \mathrm{pc}}\right)$$

</p>

<h3>Manifold Kinematic Parameters</h3>

<p>
The local null scale at the observation epoch is $c_o = V_0 - A t_o$. Operationally, photon exchange is used as a proxy for this local null scale, so the measured speed of light at the observation epoch determines $c_o$, fixing the integration constant,
</p>

<p>

$$V_0 = c_o + A t_o$$

</p>

<p>
With the manifold acceleration $A$ determined from the baryonic Tully–Fisher analysis, the Cepheid-calibrated Pantheon+ subset is used to determine the observation epoch $t_o$ on the absolute distance scale. For each candidate value of $t_o$, the corresponding $V_0$ follows algebraically from the equation above, and theoretical distance moduli $\mu_{\mathrm{th}}(z)$ are evaluated at the calibration-set redshifts. These are compared with the observed values $\mu_{\mathrm{obs}}(z)$, defining the residual vector $r_i = \mu_{\mathrm{obs}}(z_i) - \mu_{\mathrm{th}}(z_i)$. The best-fit observation epoch is obtained by minimizing the covariance-weighted chi-square statistic
</p>

<p>

$$\chi^2 = r^{\mathrm T} C^{-1} r$$

</p>

<p>
where $C$ is the full Pantheon+ STAT+SYS covariance matrix. The resulting best-fit parameters are listed in the table below.
</p>

| Parameter | Value |
|-----------|-------|
| $A$ | $3.7\times10^{-11}\ \mathrm{m\,s^{-2}}$ |
| $V_0$ | $3.16\times10^{8}\ \mathrm{m\,s^{-1}}$ |
| $t_o$ | $4.51\times10^{17}\ \mathrm{s}$ |

<h3>Comparison with Observations</h3>

<p align="center">
  <img src="figures/hubble-diagram.png" alt="Hubble diagram" width="500">
</p>

<p align="center">
  <em>
    Pantheon+SH0ES distance moduli as a function of redshift $z$, compared with the PME prediction and the
    spatially flat FLRW model. PME parameters are fixed by BTFR and Cepheid calibration. FLRW parameters
    are fixed by the Planck 2018 results.
  </em>
</p>

<p>
The Pantheon+SH0ES dataset provides observed distance moduli calibrated on an absolute scale through the SH0ES determination of the Type Ia supernova absolute magnitude. This calibration is applied identically to both models.
</p>

<p>
PME is evaluated using the fixed parameter set derived above. FLRW is evaluated using a spatially flat model specified by the Planck 2018 parameter set $\Omega_m = 0.315$, $\Omega_\Lambda = 1-\Omega_m$, and $H_0 = 67.4\ \mathrm{km\,s^{-1}\,Mpc^{-1}}$. The comparison is performed on the out-of-sample supernovae, excluding the Cepheid calibration records.
</p>

<p>
The resulting covariance-weighted chi-square values are
</p>

<p>

$$\chi^2_{\mathrm{PME}}=2726,\qquad \chi^2_{\mathrm{FLRW}}=4049$$

</p>

<p>
for $\nu=1625$ degrees of freedom, corresponding to reduced values $\chi^2/\nu=1.68$ and $2.49$, respectively. PME predicts the observed distance moduli substantially more accurately than the Planck 2018 FLRW model across the Pantheon+SH0ES sample, without dark sector parameters.
</p>

<h3>Hubble Function</h3>

<p>
The Hubble expansion rate is defined by the fractional rate of change of the real spatial extent of the manifold, $H(t) \equiv \dot{L}(t)/{L(t)}$. Differentiating the manifold extent gives $\dot{L}(t)=V_0-At$, so
</p>

<p>

$$H(t) = \frac{V_0 - At}{V_0 t - \frac{1}{2}A t^2}$$

</p>

<p>
Evaluating at the observation epoch $t=t_o$ using the best-fit manifold parameters gives the present-day expansion rate
</p>

<p>

$$H_0 = 66.5\ \mathrm{km\,s^{-1}\,Mpc^{-1}}$$

</p>

<p>
The Hubble constant therefore emerges as a prediction rather than a fitted parameter.
</p>

<h3>Cosmic Time</h3>

<p>
The redshift–time relation differs from standard cosmological evolution due to the underlying parabolic evolution. The table below compares the resulting cosmic times with those from FLRW algorithms. The parabolic expansion yields uniformly larger cosmic ages than FLRW, significantly extending the available time for early structure formation.
</p>

| $z$ | PME [Myr] | FLRW [Myr] |
|-----|-----------|------------|
| 0 | 14,283 | 13,791 |
| 1 | 7,039 | 5,840 |
| 10 | 1,265 | 470 |
| 100 | 137 | 16.4 |
| 1,000 | 13.9 | 0.429 |

<hr>

<h2>Early-Time Evolution</h2>

<p>
Independent constraints arise from the cosmic microwave background (CMB), whose acoustic scale probes the distance to last scattering relative to the sound horizon. The expansion history is determined by the PME kinematics derived above, while recombination microphysics is evaluated using standard rate equations. Thermodynamic quantities are mapped using the scale factor
</p>

<p>

$$a(t) = \frac{L(t)}{L(t_o)}$$

</p>

<h3>Baryon and Photon Densities</h3>

<p>
The baryon density is fixed by the manifold acceleration scale rather than introduced as an independent cosmological parameter. This follows from the local divergence law, which relates the sourced acceleration field to the baryonic density. For a homogeneous baryonic distribution of density $\rho_b$ within a region of characteristic size $L$, the enclosed mass is $M(L)=\frac{4\pi}{3}L^3\rho_b$, so the baryon-sourced acceleration at radius $L$ is $GM(L)/L^2=\frac{4\pi}{3}G L\rho_b$. Evaluating at the present manifold extent $L(t_o)$ and identifying with the inferred manifold acceleration $A$ gives
</p>

<p>

$$\rho_b=\frac{3A}{4\pi G\,t_o\left(V_0-\frac{1}{2}A t_o\right)}$$

</p>

<p>
Using the kinematic parameters determined in the previous sections yields
</p>

<p>

$$\rho_b = 9.49\times10^{-28}\ \mathrm{kg\,m^{-3}}$$

</p>

<p>
This value is consistent with independent observational estimates of the present-day baryon density from primordial light-element abundances.
</p>

<p>
The photon density is determined from the measured CMB temperature $T_\gamma=2.725\ \mathrm{K}$. The mapping between temperature and photon density depends on the local geometric scale $(V_0 - At)$, so the photon density is treated as epoch dependent rather than constant. For a blackbody radiation field, the photon number density is
</p>

<p>

$$n_\gamma(t)=\frac{2\zeta(3)}{\pi^2}\left(\frac{k_B T_\gamma}{\hbar (V_0-At)}\right)^3$$

</p>

<p>
and, following the geometric sign convention, the mean photon energy is $\langle E_\gamma\rangle=-\frac{\pi^4}{30\zeta(3)}k_B T_\gamma$. The mass-equivalent photon density becomes
</p>

<p>

$$\rho_\gamma(t)=\frac{n_\gamma(t)\langle E_\gamma\rangle}{-(V_0-At)^2}$$

</p>

<p>
These densities determine the baryon–photon momentum ratio and the free-electron density entering the visibility function.
</p>

<h3>Recombination Epoch</h3>

<p>
The recombination epoch is the time of maximum photon visibility, i.e., the most probable last-scattering time in the baryon–photon plasma. We evaluate the standard recombination rate equations using <code>Recfast++</code> with the PME expansion geometry in place of the FLRW algorithm, with the expansion rate governed by the best-fit manifold parameters. The free-electron number density is
</p>

<p>

$$n_e(t)=x_e(t)\,\frac{\rho_b}{m_p}\,a(t)^{-3}$$

</p>

<p>
where $\rho_b$ is the present-day baryon mass density and $m_p$ is the proton mass. The Thomson scattering rate is
</p>

<p>

$$\Gamma_T(t)=n_e(t)\,\sigma_T\,(V_0 - At)$$

</p>

<p>
where $\sigma_T$ is the Thomson cross section. The optical depth is then
</p>

<p>

$$\tau_T(t)=\int_t^{t_o}\Gamma_T(t')\,dt'$$

</p>

<p>
and the corresponding visibility function is
</p>

<p>

$$g(t)=\Gamma_T(t)\,e^{-\tau_T(t)}$$

</p>

<p>
Evaluating $g(t)$ on the PME expansion background using the <code>Recfast++</code> microphysics parametrization yields a maximum at $z_* = 1039$, $t_* = 13.4\ \mathrm{Myr}$.
</p>

<p align="center">
  <img src="figures/visibility-function.png" alt="Photon visibility function" width="500">
</p>

<p align="center">
  <em>
    Photon visibility function $g(z)$ evaluated using the recombination history on the PME expansion background.
    The peak defines the recombination epoch, yielding $z_* = 1039$.
  </em>
</p>

<h3>Sound Horizon</h3>

<p>
Prior to recombination, baryons and photons form a tightly coupled fluid whose acoustic interaction distance defines the sound horizon. The thermodynamic evolution follows the scale factor $a(t)$. The baryon–photon momentum ratio is
</p>

<p>

$$R(t)=\frac{3\rho_b}{4\rho_\gamma(t)}\,\frac{a(t)^{-3}}{a(t)^{-4}}=\frac{3\rho_b}{4\rho_\gamma(t)}\,a(t)$$

</p>

<p>
giving the sound speed
</p>

<p>

$$c_s(t)=\frac{c_{\mathrm{c}}(t)}{\sqrt{3\left(1+R(t)\right)}}$$

</p>

<p>
The causal expansion rate $c_{\mathrm{c}}(t)$ sets the rate at which interactions can be ordered through the operational clock and thus defines the effective causal scale entering the acoustic horizon integral, so that the sound horizon is
</p>

<p>

$$r_s=\int_0^{t_*} c_s(t)\,dt$$

</p>

<p>
Evaluating this expression using the manifold parameters yields $r_s=3.7\ \mathrm{Mpc}$.
</p>

<h3>Acoustic Angular Scale</h3>

<p>
The observed acoustic angle is determined by the ratio of the sound horizon at recombination to the bilocally assigned transverse size of the emission–observation pair. $L(t)$ denotes the circumference of the spatial slice at epoch $t$, so the relevant transverse quantity is the effective bilocal transverse circumference associated with the ordered pair $(t_*,t_o)$. Applying the bilocal spatial rule to this transverse configuration defines the effective bilocal transverse circumference,
</p>

<p>

$$C_{\perp} \equiv \frac{1}{2}\left[L(t_{o})+L(t_{\ast})\right]=\frac{L(t_{o})}{2}\frac{2+z_{\ast}}{1+z_{\ast}}$$

</p>

<p>
The corresponding effective transverse radius is
</p>

<p>

$$r_\perp=\frac{C_\perp}{2\pi}=\frac{L(t_o)}{4\pi}\,\frac{2+z_{\ast}}{1+z_{\ast}}$$

</p>

<p>
The acoustic angular scale is then $\theta_*=r_s/r_\perp$. Substituting and using the manifold extent evaluated at $t_o$ gives
</p>

<p>

$$\theta_{\ast}=\frac{8\pi(1+z_{\ast})}{t_o(2V_0-A t_o)(2+z_{\ast})}\,r_s$$

</p>

<p>
Evaluating this expression with the manifold parameters gives
</p>

<p>

$$\theta_* = 0.0103, \qquad 100\,\theta_* = 1.03$$

</p>

<p>
This result follows from the PME expansion geometry combined with standard recombination microphysics.
</p>

<hr>

<h2>Discussion</h2>

<p>
A detailed nucleosynthesis calculation has not been attempted within the present framework. Standard Big Bang nucleosynthesis treatments assume time-independent microphysics, including fixed particle rest energies and equilibrium thermodynamic mappings. In PME, however, the effective manifold energy scale varies explicitly with cosmic time through $E_{\mathrm{geom}}=-m(V_0-At)^2$, derived from the temporal component of the inertia-weighted action-space interval, and the operational reaction clock need not coincide with the geometric expansion time. These features break the time-translation invariance implicit in conventional BBN calculations, so the reaction network must be re-derived within the PME framework.
</p>

<p>
This distinction also affects baryon asymmetry. In equilibrium with time-reversal symmetric, time-independent microphysics, matter–antimatter annihilation drives the net baryon number toward zero, leaving a radiation-dominated universe. Standard cosmology therefore treats the baryon-to-photon ratio as an external parameter rather than deriving it from Standard Model physics. The explicitly time-dependent evolution of the PME energy scale relaxes the equilibrium assumptions underlying this argument, permitting a nonzero residual baryon density without invoking additional symmetry-breaking mechanisms. PME therefore provides a framework in which baryon asymmetry may arise from the underlying geometric evolution, allowing nucleosynthesis to be formulated self-consistently once the reaction network is derived within this context.
</p>

<p>
The framework predicts a residual non-Keplerian contribution to bound motion with radial scaling $A r^2/GM$. In compact systems this effect is suppressed and becomes significant only at larger radii. Solar-system observations therefore constrain the model but do not probe the regime in which the background term becomes dynamically dominant. Improved precision, particularly at large heliocentric distances, should reveal systematic departures from purely Keplerian motion. Detection or exclusion of such a signal provides a direct test of the construction.
</p>

<p>
Extending the bilocal framework to perturbations, structure growth, nucleosynthesis, and a fully intrinsic treatment of recombination is required to assess viability beyond the homogeneous background solution. The present formulation establishes a constrained kinematic structure whose physical adequacy must ultimately be judged by its ability to reproduce observational phenomena across these additional domains.
</p>

<h3>Code Availability</h3>

<p>
A computational notebook implementing the bilocal geometry, distance–redshift relation, and observational analysis is publicly available at:
</p>

<p align="center">
  <a href="https://www.wolframcloud.com/obj/32b2e831-2cbe-4ff5-b821-aa23f476f015">
    https://www.wolframcloud.com/obj/32b2e831-2cbe-4ff5-b821-aa23f476f015
  </a>
</p>

<p>
The notebook reproduces the results and figures presented in this work and is provided to enable independent verification of the calculations.
</p>

<hr>

<h2>Conclusion</h2>

<p>
A constrained bilocal construction on a complex manifold yields a quadratic interval whose local reduction yields a homogeneous acceleration scale. This single geometric scale governs both the parabolic evolution of the manifold and the redistribution of acceleration flux in gravitationally bound systems. The bilocal geometry produces an emergent local null constraint, defines an invariant action geometry, and admits a canonical decomposition into temporal and spatial contributions. From this structure, a Hamiltonian system and associated Hamilton–Jacobi equation arise as the projection of the inertia-weighted invariant geometric action into the timelike sector, so that particle motion follows geodesics of action space without introducing independent dynamical postulates, while phase evolution provides its continuation beyond the observable domain. Gravity and inertia therefore emerge as complementary manifestations of a conserved acceleration field inherited from the manifold kinematics.
</p>

<p>
The evolution implied by this construction yields a closed analytic distance–redshift relation, from which the Pantheon+ Type Ia supernova luminosity distances follow directly on an absolute scale. The same parameter set predicts the present-day Hubble constant and produces uniformly extended cosmic ages. In the local-reduction regime, redistribution of the homogeneous acceleration field generates an inverse-square sourced component and a circular-orbit envelope consistent with the observed baryonic Tully–Fisher relation. The acceleration scale inferred from galaxy dynamics then fixes the baryonic density of the homogeneous universe, linking galactic and cosmological observables without introducing non-baryonic dark matter or dark energy components.
</p>

<p>
The bilocal construction also determines the causal horizon and implies a constant ratio between the causal domain and manifold extent, placing the last-scattering surface within a single causal region and accounting for large-scale isotropy. The geometry yields a transverse scale for recombination that reproduces the observed acoustic angular scale. Because the available acceleration flux is finite, gravitational collapse approaches saturated configurations, eliminating curvature singularities and enforcing a globally ordered causal structure. Rotational inertia emerges from redistribution of the same finite acceleration budget, providing a Machian interpretation in which local inertial behavior depends on the global distribution of inertial content.
</p>

<p>
Evolution, causal structure, action, gravity, inertia, and dynamical law therefore arise from a common bilocal origin, with all dynamics derived from the momentum-weighted invariant separation, providing a unified explanation of isotropy, galaxy rotation, Type Ia supernova magnitudes, the acoustic scale, nonsingular gravitational collapse, the baryonic density, and the Hubble constant.
</p>

<hr>

<h2>How to Cite</h2>

<p>
If you use this work, please cite both the manuscript and the archived repository:
</p>

<pre><code>@misc{Airey2026PME,
  author       = {Airey, Donald},
  title        = {Gravity and Action from the Evolution of a Complex Manifold},
  year         = {2026},
  publisher    = {Zenodo},
  doi          = {10.5281/zenodo.20414999},
  url          = {https://doi.org/10.5281/zenodo.20414999}
}
</code></pre>

<p>
GitHub also provides a <strong>Cite this repository</strong> button in the right sidebar, which generates APA and BibTeX citations from the included <code>CITATION.cff</code> file.
</p>

<hr>

<h2>License</h2>

<p>
Copyright &copy; 2026 Donald Airey. This work is licensed under the
<a href="LICENSE">GNU General Public License v3.0</a>.
</p>
