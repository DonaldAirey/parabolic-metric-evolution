<h1>Gravity and Action from the Parabolic Metric Evolution of a Complex Manifold</h1>

<p class="metadata"><strong>Donald Airey</strong><br>
ORCID: 0000-0002-2958-1545<br>
1621 County Highway 31, Cooperstown, NY 13326, USA<br>
<a href="mailto:don@airey.us">don@airey.us</a></p>

<p class="keywords">cosmology, gravitational theory, cosmic expansion, cosmological dynamics, Newtonian cosmology, Type Ia supernovae, large-scale structure</p>

<h2>Abstract</h2>
<p>We present a bilocal geometric framework in which separations are defined between ordered pairs of events rather than by a local infinitesimal metric. This construction is motivated by the need to represent global evolution in a manner that remains well-defined over finite separations while admitting a smooth local limit. The resulting geometry is formulated on a complex manifold with an imaginary temporal coordinate and a real spatial coordinate. A constant manifold acceleration sets the global spatial scale and produces a parabolic cycle of expansion and contraction. In the local reduction, the same acceleration scale yields a circular-orbit envelope consistent with the baryonic Tully–Fisher relation. At cosmological scales, the resulting analytic distance–redshift relation predicts the Pantheon+ Type Ia supernova luminosity distances on the SH0ES-calibrated absolute scale and yields a lower covariance-weighted <span class="math">χ^2</span> than Planck-calibrated FLRW, without invoking dark matter or dark energy. The parabolic metric evolution, when combined with standard recombination microphysics, yields an acoustic angular scale consistent with Planck measurements.</p>
<a id="fig:manifold"></a>
<p align="center"><img src="figures/pme-manifold.png" alt="Figure 1: Schematic representation of the complex parabolic metric manifold. Latitude lines correspond to spatial slices at fixed epoch, while longitude lines trace the temporal evolution of the manifold." width="700"></p>
<p align="center"><em><strong>Figure 1.</strong> Schematic representation of the complex parabolic metric manifold. Latitude lines correspond to spatial slices at fixed epoch, while longitude lines trace the temporal evolution of the manifold.</em></p>

<h2>Introduction</h2>

<p>Cosmological observations tightly constrain theoretical descriptions of the universe. Measurements of the cosmic microwave background (CMB) fix early-universe conditions and global geometry with high precision [Planck2018], while Type Ia supernovae (SNe Ia) probe the late-time expansion history through the luminosity distance–redshift relation [Brout2022]. Although each dataset is internally consistent, discrepancies arise when parameters inferred from early- and late-time observations are compared. In particular, the tension in the Hubble constant [Planck2018,Riess2022] indicates that the standard cosmological model may be incomplete.</p>

<p>Historically, such discrepancies have been addressed by extending the model. The cosmological constant was introduced to permit a static universe [Einstein1917] and abandoned following the discovery of expansion [Hubble1929]. Galaxy rotation curves motivated the introduction of non-baryonic dark matter [Rubin1980], and supernova evidence for accelerated expansion led to the reintroduction of the cosmological constant as dark energy [Riess1998,Perlmutter1999]. While these additions yield a phenomenologically successful framework, the dominant components of the cosmic energy budget remain physically unexplained [Planck2018]. More recent approaches introduce additional degrees of freedom, including time-varying dark energy [DiValentino2021], further increasing the parametric structure of the model.</p>

<p>We develop a kinematic framework in which large-scale evolution and local gravitational phenomena arise from a common geometric structure, termed the Parabolic Metric Evolution (PME). Local metric descriptions specify infinitesimal separations, so finite separations between distant events must be constructed by integrating along a chosen connection; in a globally evolving system, this construction can depend on both the path and the evolution of the geometry. The PME framework replaces this path-dependent procedure with a bilocal definition that assigns separations directly to ordered event pairs while admitting a consistent local limit. Motion on the manifold is governed by a single intrinsic kinematic scale, eliminating the need for multiple independent cosmological parameters and linking global expansion and local dynamics to a common geometric origin. The geometric structure of the manifold is illustrated in Fig. 1.</p>

<p>This approach differs from relativistic metric gravity in its bilocal definition of separation and from modified-gravity models [Milgrom1983,McGaugh2016] in that the characteristic acceleration scale is not introduced phenomenologically but inherited from the global manifold kinematics by the local-reduction regime. Cosmological evolution, gravity, and the laws governing motion are thereby unified through a single acceleration scale determined by the manifold kinematics.</p>

<p>The resulting construction defines a minimal kinematic closure: the lowest-order geometric structure that consistently relates finite separations, global evolution, and local dynamics within a single framework, without introducing independent dynamical components. The bilocal definition of separation provides a representation of finite intervals compatible with global evolution, and the restriction to a single intrinsic acceleration scale selects the simplest nontrivial homogeneous dynamics beyond uniform motion, yielding a closed and self-consistent description across cosmological and local regimes.</p>

<h2>Bilocal Geometry</h2>

<h3>Foundational Structure</h3>

<p>The framework is defined by the following postulates:</p>

<ol>

<li>Physical separations are defined bilocally between ordered pairs of events.</li>

<li>The manifold evolution is governed by a constant acceleration scale <span class="math">A</span>.</li>

<li>The manifold is parameterized by an intrinsic evolution coordinate <span class="math">χ</span>.</li>

<li>Observable time is defined operationally through null exchange, providing an invariant ordering of events. The intrinsic evolution parameter is related to this observable time by the projection <span class="math">χ = i t</span>, which fixes the real–imaginary decomposition of temporal and spatial functionals and serves as a defining structural postulate of the framework.</li>

</ol>

<p>All subsequent results follow from this structure.</p>

<h3>Bilocal Spatial Separation</h3>

<p>Let <span class="math">p_e=(x_e^0,x_e^1)</span> denote an emission event and <span class="math">p_o=(x_o^0,x_o^1)</span> an observation event, with the bilocal interval constructed from a temporal functional obtained from accumulated evolution between slices and a spatial functional defined from separations on the emission and observation slices.</p>

<p>The bilocal construction is illustrated in Figure 2. The spatial slices scale with a global manifold extent <span class="math">L(t)</span>, so the separations at emission and observation satisfy</p>

<a id="eq:comoving_definition"></a>
<table><tr><td><pre><code>\frac{\Delta x_e^1}{L(t_e)}=\frac{\Delta x_o^1}{L(t_o)} .</code></pre></td><td><strong>(1)</strong></td></tr></table>

<p>Imposing symmetry under interchange of emission and observation together with a smooth coincidence limit motivates adopting the midpoint average as the minimal symmetric choice,</p>

<a id="equation-2"></a>
<table><tr><td><pre><code>\Delta s^1=\Delta x_o^1-\frac12(\Delta x_o^1-\Delta x_e^1),</code></pre></td><td><strong>(2)</strong></td></tr></table>

<a id="eq:spatial_half_expansion"></a>
<table><tr><td><pre><code>\Delta s^1=\frac12(\Delta x_o^1+\Delta x_e^1),</code></pre></td><td><strong>(3)</strong></td></tr></table>

<a id="fig:bilocalconstruction"></a>
<p align="center"><img src="figures/bilocal-geometry.png" alt="Figure 2: Geometric construction of the bilocal interval between emission event &lt;span class=&quot;math&quot;&gt;p_e&lt;/span&gt; and observation event &lt;span class=&quot;math&quot;&gt;p_o&lt;/span&gt;, showing the accumulated temporal evolution and the symmetric midpoint spatial separation between scaled slices." width="700"></p>
<p align="center"><em><strong>Figure 2.</strong> Geometric construction of the bilocal interval between emission event <span class="math">p_e</span> and observation event <span class="math">p_o</span>, showing the accumulated temporal evolution and the symmetric midpoint spatial separation between scaled slices.</em></p>

<h3>Invariance of the Bilocal Interval</h3>

<p>Consider a bilocal scalar constructed from the temporal and spatial endpoint functionals <span class="math">(Δ s^0,Δ s^1)</span>. We adopt a quadratic form as the lowest-order scalar consistent with finite separations, ensuring that the local reduction yields a well-defined null condition while avoiding higher-order dependence on endpoint structure,</p>

<a id="equation-4"></a>
<table><tr><td><pre><code>\Delta s^2 = a\,(\Delta s^0)^2 + b\,(\Delta s^1)^2 + 2c\,\Delta s^0 \Delta s^1 .</code></pre></td><td><strong>(4)</strong></td></tr></table>

<p>Under interchange of the ordered endpoints <span class="math">(p_e,p_o)</span>, the temporal functional changes sign while the symmetric spatial functional does not, so the mixed term changes sign. Invariance therefore requires <span class="math">c=0</span>.</p>

<p>In the local reduction, sufficiently small endpoint separations render the temporal and spatial functionals linear in the coordinate increments. The null condition must define a finite null ratio, which requires both temporal and spatial contributions to enter non-degenerately so that the null condition defines a finite null ratio. The interval therefore reduces to</p>

<pre><code>\Delta s^2 = a (\Delta s^0)^2 + b (\Delta s^1)^2 .</code></pre>

<p>The remaining quadratic form is therefore constrained up to a positive overall factor and a relative scaling between the temporal and spatial functionals. These functionals are not arbitrary coordinates but are identified with the canonical imaginary and real components of the complex manifold, with this identification fixing their relative normalization. The bilocal interval is therefore</p>

<a id="eq:bilocal_interval"></a>
<table><tr><td><pre><code>\Delta s^2 = (\Delta s^0)^2 + (\Delta s^1)^2 ,</code></pre></td><td><strong>(5)</strong></td></tr></table>

<p>with <span class="math">Δ s^0</span> purely imaginary and <span class="math">Δ s^1</span> real.</p>

<h3>Imaginary Velocity</h3>

<p>The intrinsic evolution of the manifold is parameterized by a coordinate <span class="math">χ</span>. Observable time is introduced by the projection <span class="math">χ = i t</span>, so that <span class="math">dχ = i dt</span>, fixing the real–imaginary decomposition used in the bilocal construction.</p>

<p>With constant intrinsic acceleration <span class="math">A</span>, the velocity scale along the manifold history follows from integration with respect to <span class="math">χ</span>,</p>

<pre><code>v(t) = \int A\, d\chi .</code></pre>

<p>Substituting <span class="math">dχ = i dt</span> gives <span class="math">v(t) = i \int A dt</span>, which evaluates to</p>

<a id="eq:imaginary_velocity"></a>
<table><tr><td><pre><code>v(t) = i(At - V_0),</code></pre></td><td><strong>(6)</strong></td></tr></table>

<p>where <span class="math">V_0</span> is an integration constant representing the initial expansion rate of the manifold.</p>

<h3>Induced Spatial Evolution</h3>

<p>The observable spatial extent arises from integrating the imaginary velocity along the imaginary temporal direction. The global spatial scale of the manifold is therefore <span class="math">L(t) \equiv \int v(t)  dχ</span>. Substituting the expression for <span class="math">v(t)</span> and using <span class="math">dχ = i dt</span> gives <span class="math">L(t) = \int i(At - V_0)  i  dt</span>. Evaluating the integral yields</p>

<a id="eq:manifold_extent"></a>
<table><tr><td><pre><code>L(t) = V_0 t - \frac{1}{2} A t^2.</code></pre></td><td><strong>(7)</strong></td></tr></table>

<h3>Manifold Deceleration</h3>

<p>The intrinsic evolution is defined along <span class="math">χ</span>, while observable dynamics are expressed in the projected time coordinate <span class="math">t</span> with <span class="math">dχ = i dt</span>. Rewriting the manifold extent in terms of <span class="math">t</span> yields its observable form. Differentiating twice with respect to <span class="math">t</span> gives</p>

<a id="eq:manifolddeceleration"></a>
<table><tr><td><pre><code>\frac{d^2 L}{dt^2} = -A,</code></pre></td><td><strong>(8)</strong></td></tr></table>

<p>so the manifold extent evolves with a constant kinematic deceleration of magnitude <span class="math">A</span>, which is universal and independent of position or epoch.</p>

<h2>Cosmological Distance</h2>

<p>Observable cosmological distances follow from the bilocal interval defined in equation (5).</p>

<h3>Temporal Separation</h3>

<p>The temporal component of the bilocal interval is obtained from the accumulated tangent evolution along the manifold history between the emission and observation parameters <span class="math">t_e</span> and <span class="math">t_o</span>, <span class="math">Δ s^0 \equiv \int_{t_e}^{t_o} v(t) dt</span>. Substituting Eq. (6) gives</p>

<a id="equation-9"></a>
<table><tr><td><pre><code>\Delta s^0 = \int_{t_e}^{t_o} i\left(A t - V_0\right)\,dt .</code></pre></td><td><strong>(9)</strong></td></tr></table>

<p>Evaluating the integral yields</p>

<a id="equation-10"></a>
<table><tr><td><pre><code>\Delta s^0 = i\left(\frac{A}{2}\left(t_o^2 - t_e^2\right) - V_0\left(t_o - t_e\right)\right) .</code></pre></td><td><strong>(10)</strong></td></tr></table>

<p>The temporal separation is purely imaginary and depends only on the endpoints.</p>

<h3>Spatial Separation</h3>

<p>Solving equation (1) for the emission separation gives</p>

<a id="equation-11"></a>
<table><tr><td><pre><code>\Delta x_e^1 = \Delta x_o^1\,\frac{L(t_e)}{L(t_o)} .</code></pre></td><td><strong>(11)</strong></td></tr></table>

<p>Because spatial slices scale with the manifold extent <span class="math">L(t)</span> and the slice separations satisfy the bilocal scaling relation given in equation (3), the spatial component becomes</p>

<a id="eq:bilocal_spatial"></a>
<table><tr><td><pre><code>\Delta s^1 =\frac{\Delta x_o^1}{2}\left(1 +\frac{V_0 t_e - \frac{1}{2} A t_e^2}{V_0 t_o - \frac{1}{2} A t_o^2}\right).</code></pre></td><td><strong>(12)</strong></td></tr></table>

<h3>Bilocal Metric Formula</h3>

<p>Substituting the temporal and spatial separations into equation (5) yields the interval relating the emission and observation events,</p>

<a id="eq:bilocal_metric"></a>
<table><tr><td><pre><code>\Delta s^2 = \left[i\left(\frac{A}{2}\left(t_o^2 - t_e^2\right) - V_0\left(t_o - t_e\right)\right)\right]^2+ \left[\frac{\Delta x_o^1}{2}\left(1 + \frac{V_0 t_e - \frac{1}{2}A t_e^2}{V_0 t_o - \frac{1}{2}A t_o^2}\right)\right]^2 .</code></pre></td><td><strong>(13)</strong></td></tr></table>

<h3>Redshift Relation</h3>

<p>Redshift is defined observationally by the ratio of observed to emitted wavelength,</p>

<a id="equation-14"></a>
<table><tr><td><pre><code>1+z \equiv \frac{\lambda_o}{\lambda_e}.</code></pre></td><td><strong>(14)</strong></td></tr></table>

<p>We identify wavelength with a comoving spatial separation and assume that such separations scale with the manifold extent, so that <span class="math">λ(t) \propto L(t)</span>.</p>

<a id="eq:redshift_relation"></a>
<table><tr><td><pre><code>1+z = \frac{L(t_o)}{L(t_e)}.</code></pre></td><td><strong>(15)</strong></td></tr></table>

<p>Using equation (7), the emission epoch <span class="math">t_e</span> is expressed in terms of <span class="math">t_o</span> and the observed redshift <span class="math">z</span>,</p>

<a id="eq:te_solution"></a>
<table><tr><td><pre><code>t_e = \frac{V_0(1+z) - \sqrt{(1+z)\big[(V_0 - A t_o)^2 + V_0^2 z\big]}}{A(1+z)},</code></pre></td><td><strong>(16)</strong></td></tr></table>

<p>where the negative branch is chosen so that <span class="math">t_e &lt; t_o</span>.</p>

<p>Substituting into equation (13) and imposing the null condition <span class="math">Δ s^2 = 0</span> yields the observable spatial separation,</p>

<a id="eq:distance_redshift_relation"></a>
<table><tr><td><pre><code>D_C(z)= \Delta x_o^1= \frac{t_o\left(2V_0 - A t_o\right) z}{2 + z}.</code></pre></td><td><strong>(17)</strong></td></tr></table>

<h2>Causal Structure</h2>

<p>The null structure of the bilocal interval also determines the extent of causal connectivity on the manifold. The largest spatial separation permitted by null ordering is obtained from equation (13) with the emission event at the origin of the manifold history, <span class="math">t_e = 0</span>, and the observation event at epoch <span class="math">t_o = t</span>. Solving the null condition <span class="math">Δ s^2 = 0</span> for the observed separation gives the causal horizon</p>

<a id="equation-18"></a>
<table><tr><td><pre><code>d_{\mathrm{ch}}(t) = t\left(2V_0 - A t\right) .</code></pre></td><td><strong>(18)</strong></td></tr></table>

<p>Differentiating the causal horizon gives the expansion rate of the causal boundary,</p>

<a id="equation-19"></a>
<table><tr><td><pre><code>c_{\mathrm{c}}(t)=\frac{d}{dt}\,d_{\mathrm{ch}}=2\left(V_0-At\right).</code></pre></td><td><strong>(19)</strong></td></tr></table>

<p>This quantity defines the rate at which the accessible causal domain can be extended under the operational clock, and therefore characterizes the growth of the causally orderable region.</p>

<p>Comparing the causal horizon with the manifold extent <span class="math">L(t)</span> defined in equation (7) yields</p>

<a id="equation-20"></a>
<table><tr><td><pre><code>\frac{d_{\mathrm{ch}}(t)}{L(t)} = 2 .</code></pre></td><td><strong>(20)</strong></td></tr></table>

<p>The causal horizon is therefore twice the manifold extent at all epochs, placing the entire last-scattering surface within a single causal region. Because the homogeneous manifold acceleration introduces no preferred direction, the large-scale isotropy of the cosmic microwave background follows directly from the geometry.</p>

<h2>Gravity</h2>

<p>When the temporal interval between neighboring events is small compared with the characteristic evolution scale of the manifold extent <span class="math">L(t)</span>, the bilocal construction admits a smooth local reduction yielding an effective acceleration field inherited from the manifold kinematics.</p>

<h3>Coincidence Limit</h3>

<p>The local description is obtained as the coincidence limit of the bilocal interval as the endpoint separation tends to zero. Let the observation event occur at epoch <span class="math">t</span> and the emission event at <span class="math">t-Δ t</span>, with <span class="math">Δ t \to 0</span>. To extract the leading nontrivial local structure, the temporal and spatial bilocal functionals are expanded to first and second orders in <span class="math">Δ t</span>.</p>

<p>Using the local expansion of the manifold extent,</p>

<pre><code>L(t-\Delta t)=L(t)-\dot L(t)\,\Delta t-\frac{1}{2}A\,\Delta t^2,</code></pre>

<p>the slice-separation relation gives</p>

<a id="equation-21"></a>
<table><tr><td><pre><code>\frac{\Delta x_e^1}{L(t-\Delta t)}=\frac{\Delta x_o^1}{L(t)} .</code></pre></td><td><strong>(21)</strong></td></tr></table>

<p>Hence</p>

<a id="equation-22"></a>
<table><tr><td><pre><code>\Delta x_e^1=\Delta x_o^1\left(1-\frac{\dot L}{L}\Delta t\right),</code></pre></td><td><strong>(22)</strong></td></tr></table>

<p>so the bilocal spatial component becomes</p>

<a id="equation-23"></a>
<table><tr><td><pre><code>\Delta s^1=\Delta x_o^1\left(1-\frac{1}{2}\frac{\dot L}{L}\Delta t\right)\approx \Delta x_o^1</code></pre></td><td><strong>(23)</strong></td></tr></table>

<p>to leading order in <span class="math">Δ t</span>. Over the same interval, the temporal component is</p>

<a id="equation-24"></a>
<table><tr><td><pre><code>\Delta s^0=\int_{t-\Delta t}^{t} i\left(A t&#x27; - V_0\right)\,dt&#x27; \approx i\left(V_0-At\right)\Delta t.</code></pre></td><td><strong>(24)</strong></td></tr></table>

<p>Substituting these leading terms into equation (5) yields</p>

<a id="eq:local_interval"></a>
<table><tr><td><pre><code>\Delta s^2 \approx -\left(V_0-At\right)^2\Delta t^2 + (\Delta x_o^1)^2 .</code></pre></td><td><strong>(25)</strong></td></tr></table>

<p>which is the emergent local interval obtained from the coincidence limit of the bilocal geometry. The local interval therefore defines a tangent of fixed magnitude <span class="math">V_0-At</span> shared by all trajectories at epoch <span class="math">t</span>, whose projections onto orthogonal temporal and spatial components give rise to timelike, null, and spacelike directions.</p>

<h3>Acceleration Field</h3>

<p>Consider an event pair <span class="math">(p_e,p_o)</span> whose temporal separation <span class="math">Δ t</span> satisfies <span class="math">Δ t \ll L/\dot L</span>. Expanding the manifold extent about a reference epoch <span class="math">t_0</span> gives</p>

<a id="equation-26"></a>
<table><tr><td><pre><code>L(t_0+\delta t)=L(t_0)+\dot{L}(t_0)\,\delta t+\frac{1}{2}\ddot{L}(t_0)\,\delta t^2+\cdots .</code></pre></td><td><strong>(26)</strong></td></tr></table>

<p>Using equation (8), the quadratic term is governed by the constant local value <span class="math">\ddot{L}(t_0)=-A</span>. The local reduction therefore contains a homogeneous second-order contribution corresponding to a uniform deceleration of magnitude <span class="math">A</span> inherited from the global manifold evolution, which provides the physical origin of gravity in the local limit. This uniform deceleration defines the background acceleration field underlying local gravitational dynamics.</p>

<p>The effective inward acceleration in a bound system decomposes into a homogeneous background and a sourced concentration,</p>

<a id="eq:ain_scalar"></a>
<table><tr><td><pre><code>a_{\mathrm{in}}(x)=a_{\mathrm{bg}}+a_{\mathrm{conc}}(x).</code></pre></td><td><strong>(27)</strong></td></tr></table>

<p>The background term <span class="math">a_{bg}</span> is uniform and has constant magnitude <span class="math">A</span>. In the absence of localized content, it defines the manifold evolution, and an inertial frame follows it without inducing concentration or depletion. Localized inertial content, however, resists this acceleration, redistributing the flux into spatial concentrations that define the sourced gravitational component <span class="math">a_{conc}(x)</span> governing bound dynamics. The inertial parameter <span class="math">m</span> entering this redistribution is the same quantity that weights the invariant separation in the construction of geometric action, so that the gravitational response corresponds to a redistribution of the inertia-weighted action-space separation underlying the local geometry.</p>

<h3>Minimal Local Closure</h3>

<p>The bilocal construction fixes the homogeneous background acceleration scale <span class="math">A</span> through the second-order local reduction of the manifold extent but does not determine the sourced concentration arising from spatial variations in inertial resistance. A weak-field closure is therefore required.</p>

<p>We adopt a minimal closure as the lowest-order local form consistent with locality, linearity in enclosed inertial content, rotational invariance, and additivity. These conditions restrict the sourced field to a divergence relation as the leading-order connection between field structure and inertial content, rather than an assumed inverse-square form. The concentration field therefore satisfies a divergence proportional to a local inertial density, with enclosed content given by its volume integral. In the weak-field limit, this density is dominated by rest mass and reduces to the baryonic density. All intrinsic kinematic scales are fixed by the acceleration scale <span class="math">A</span>, while the constant <span class="math">G</span> sets the coupling to localized inertial content without introducing an additional kinematic scale.</p>

<p>For a spherically symmetric configuration the sourced acceleration is radial,</p>

<a id="equation-28"></a>
<table><tr><td><pre><code>\mathbf a_{\mathrm{conc}}(r)=a_r(r)\,\hat r.</code></pre></td><td><strong>(28)</strong></td></tr></table>

<p>In the local-reduction regime relevant for gravitationally bound systems, the concentration field resides in three spatial dimensions, so spherical symmetry is defined with respect to ordinary 2-spheres in <span class="math">R^3</span>. The flux through a sphere of radius <span class="math">r</span> is</p>

<a id="equation-29"></a>
<table><tr><td><pre><code>\Phi(r)=\oint_S \mathbf a_{\mathrm{conc}}\cdot d\mathbf S
=4\pi r^2 a_r(r).</code></pre></td><td><strong>(29)</strong></td></tr></table>

<p>Imposing flux conservation together with linearity in the enclosed inertial content gives</p>

<a id="eq:aft_flux_integral"></a>
<table><tr><td><pre><code>\oint_S \mathbf a_{\mathrm{conc}}\cdot d\mathbf S = -4\pi G M(r),</code></pre></td><td><strong>(30)</strong></td></tr></table>

<p>where <span class="math">M(r)</span> is the enclosed inertial content within radius <span class="math">r</span>, obtained from the local density by</p>

<a id="equation-31"></a>
<table><tr><td><pre><code>M(r)=\int_V \rho_{\mathrm{inertial}}\,dV,</code></pre></td><td><strong>(31)</strong></td></tr></table>

<p>and <span class="math">G</span> is the empirical coupling relating inertial content to concentration of the background acceleration. Spherical symmetry then yields</p>

<a id="eq:aft_inverse_square"></a>
<table><tr><td><pre><code>\mathbf a_{\mathrm{conc}}(r)=-\frac{G M(r)}{r^2}\,\hat r,</code></pre></td><td><strong>(32)</strong></td></tr></table>

<p>and Gauss's theorem gives</p>

<a id="eq:aft_gauss_law"></a>
<table><tr><td><pre><code>\nabla\!\cdot \mathbf{a}_{\mathrm{conc}} = -4\pi G \rho_{\mathrm{inertial}},</code></pre></td><td><strong>(33)</strong></td></tr></table>

<p>which is the Poisson equation for the sourced weak-field limit. In the weak-field regime relevant for galactic dynamics, the inertial density is dominated by baryonic rest-mass contributions, so <span class="math">ρ_{inertial}\approxρ_b</span>.</p>

<h3>Circular Orbits</h3>

<p>For a body in a circular orbit of radius <span class="math">r</span> with tangential speed <span class="math">v</span>, the required centripetal acceleration is</p>

<a id="equation-34"></a>
<table><tr><td><pre><code>a_{\mathrm{cent}}(r) = -\frac{v^2}{r} .</code></pre></td><td><strong>(34)</strong></td></tr></table>

<p>Equating this with the inward acceleration from equation (27) gives</p>

<a id="equation-35"></a>
<table><tr><td><pre><code>-\frac{v^2}{r} = -A - \frac{G M_b(r)}{r^2} ,</code></pre></td><td><strong>(35)</strong></td></tr></table>

<p>and multiplying by <span class="math">r</span> gives</p>

<a id="equation-36"></a>
<table><tr><td><pre><code>v^2 = A r + \frac{G M_b(r)}{r} .</code></pre></td><td><strong>(36)</strong></td></tr></table>

<p>Then, solving for the enclosed baryonic mass gives</p>

<a id="eq:massradius"></a>
<table><tr><td><pre><code>M_b(r) = \frac{r\left(v^2 - A r\right)}{G}.</code></pre></td><td><strong>(37)</strong></td></tr></table>

<h3>Circular-Orbit Solutions</h3>

<p>Equation (37) defines the PME fundamental plane, a two-parameter family of circular-orbit solutions relating baryonic mass <span class="math">M</span>, orbital radius <span class="math">r</span>, and orbital speed <span class="math">v</span>.</p>

<p>For fixed orbital speed <span class="math">v</span>, the mass function <span class="math">M(r)</span> is a concave quadratic in <span class="math">r</span>. Differentiating gives</p>

<a id="equation-38"></a>
<table><tr><td><pre><code>\frac{dM}{dr} = \frac{v^2 - 2 A r}{G} .</code></pre></td><td><strong>(38)</strong></td></tr></table>

<p>The mass therefore reaches a maximum at</p>

<a id="equation-39"></a>
<table><tr><td><pre><code>r_{\max} = \frac{v^2}{2A} .</code></pre></td><td><strong>(39)</strong></td></tr></table>

<p>Substituting this radius into equation (37) yields the maximum baryonic mass compatible with a circular orbit at speed <span class="math">v</span>,</p>

<a id="eq:btfr_envelope"></a>
<table><tr><td><pre><code>M_{\max}(v) = \frac{v^4}{4 A G}.</code></pre></td><td><strong>(40)</strong></td></tr></table>

<p>The surface <span class="math">M(v,r)</span> therefore defines a fundamental plane of circular-orbit solutions, as shown in Figure 3, with the ridge <span class="math">M_{\max}(v)</span> giving the upper envelope of baryonic mass for a given orbital speed. Galaxies dominated by circular rotation are expected to saturate this boundary and follow a characteristic mass–velocity relation.</p>

<a id="fig:fundamentalplane"></a>
<p align="center"><img src="figures/fundamental-plane.png" alt="Figure 3: PME fundamental plane defined by equation (37). The baryonic mass surface &lt;span class=&quot;math&quot;&gt;M(v,r)&lt;/span&gt; is shown as a function of orbital speed &lt;span class=&quot;math&quot;&gt;v&lt;/span&gt; and orbital radius &lt;span class=&quot;math&quot;&gt;r&lt;/span&gt; for an illustrative manifold acceleration scale &lt;span class=&quot;math&quot;&gt;A = 10^{-11} m s^{-2}&lt;/span&gt;. The red ridge marks the locus &lt;span class=&quot;math&quot;&gt;M_{\max}(v)&lt;/span&gt; corresponding to the maximum baryonic mass permitted by the manifold kinematics at each orbital speed. Galaxies populating this ridge reproduce the baryonic Tully–Fisher relation." width="700"></p>
<p align="center"><em><strong>Figure 3.</strong> PME fundamental plane defined by equation (37). The baryonic mass surface <span class="math">M(v,r)</span> is shown as a function of orbital speed <span class="math">v</span> and orbital radius <span class="math">r</span> for an illustrative manifold acceleration scale <span class="math">A = 10^{-11} m s^{-2}</span>. The red ridge marks the locus <span class="math">M_{\max}(v)</span> corresponding to the maximum baryonic mass permitted by the manifold kinematics at each orbital speed. Galaxies populating this ridge reproduce the baryonic Tully–Fisher relation.</em></p>

<h3>Baryonic Tully–Fisher Relation</h3>

<p><span class="math">M_{\max}(v)</span> defines the scaling <span class="math">M \propto v^4</span>, consistent with the observed baryonic Tully–Fisher relation [McGaugh2000].</p>

<p>A characteristic acceleration scale in galaxy dynamics has previously been emphasized in frameworks such as MOND [Milgrom1983], in which the force law is modified to reproduce Tully–Fisher-type scaling.</p>

<p>The manifold acceleration <span class="math">A</span> is determined empirically by fitting the circular-orbit envelope (equation (40)) to the SPARC galaxy sample of McGaugh, Lelli and Schombert [McGaugh2016], using the assumptions <span class="math">\Upsilon_*=0.5</span>, <span class="math">f_{gas}=1.33</span>, zero intrinsic mass-to-light uncertainty, and the quality cut <span class="math">Qual\leq 3</span>. These rotationally supported disk systems are well suited to the analysis, as their kinematics closely follow the circular-orbit approximation.</p>

<p>For each galaxy the rotation curve provides an asymptotic circular velocity <span class="math">v</span>, while the baryonic mass <span class="math">M_b</span> is computed as <span class="math">M_b=\Upsilon_* L_{3.6}+f_{gas} M_{HI}</span>. The value of <span class="math">A</span> is determined by minimizing the <span class="math">χ^2</span> statistic between the theoretical envelope and the observed <span class="math">(M_b,v)</span> pairs. The best-fit manifold acceleration is</p>

<a id="equation-41"></a>
<table><tr><td><pre><code>A = 3.7\times10^{-11}\,\mathrm{m\,s^{-2}} .</code></pre></td><td><strong>(41)</strong></td></tr></table>

<p>The observed galaxies follow the predicted <span class="math">M\propto v^4</span> scaling across a wide range of baryonic masses and rotational velocities, as shown in Figure 4. The baryonic Tully–Fisher relation is a direct consequence of the constant-acceleration structure of the manifold and an observational signature of the acceleration flux.</p>

<a id="fig:btfrchart"></a>
<p align="center"><img src="figures/btfr-chart.png" alt="Figure 4: Log–log plot of baryonic mass &lt;span class=&quot;math&quot;&gt;M_b&lt;/span&gt; versus outer rotation speed &lt;span class=&quot;math&quot;&gt;v&lt;/span&gt; for the SPARC galaxy sample of McGaugh, Lelli and Schombert [McGaugh2016]. Black circles show the observed galaxies. The solid red line shows the PME circular-orbit envelope evaluated at the best-fit acceleration." width="700"></p>
<p align="center"><em><strong>Figure 4.</strong> Log–log plot of baryonic mass <span class="math">M_b</span> versus outer rotation speed <span class="math">v</span> for the SPARC galaxy sample of McGaugh, Lelli and Schombert [McGaugh2016]. Black circles show the observed galaxies. The solid red line shows the PME circular-orbit envelope evaluated at the best-fit acceleration.</em></p>

<h3>Global Acceleration Budget</h3>

<p>The local closure fixes all non-homogeneous acceleration flux as sourced by inertial content. In the weak-field regime this reduces to baryonic mass. Integrating the flux law over the full homogeneous domain of scale <span class="math">L</span> gives</p>

<a id="equation-42"></a>
<table><tr><td><pre><code>\Phi_{\mathrm{tot}}=\oint \mathbf a_{\mathrm{conc}}\!\cdot d\mathbf S=-4\pi G M_b^{\mathrm{tot}} .</code></pre></td><td><strong>(42)</strong></td></tr></table>

<p>Using the global relation between baryonic mass and the background acceleration scale,</p>

<a id="equation-43"></a>
<table><tr><td><pre><code>M_b^{\mathrm{tot}}=\frac{A L^2}{G},</code></pre></td><td><strong>(43)</strong></td></tr></table>

<p>yields</p>

<a id="equation-44"></a>
<table><tr><td><pre><code>\Phi_{\mathrm{tot}}=-4\pi A L^2 .</code></pre></td><td><strong>(44)</strong></td></tr></table>

<p>Thus the available concentration flux is fixed by the background scale <span class="math">A</span> and is completely accounted for by baryonic mass. Local gravitational systems therefore correspond to partial redistributions of a finite acceleration budget, so gravitational collapse approaches a saturated configuration rather than an unbounded one.</p>

<h3>Mach's Bucket</h3>

<p>The bilocal reduction introduces a homogeneous acceleration scale <span class="math">A</span> fixed by the geometry of the manifold. This acceleration is not sourced by baryonic matter; instead, baryonic mass redistributes it through conservation of acceleration flux (equation (30)).</p>

<p>For a rotating system of radius <span class="math">r</span> and tangential speed <span class="math">v</span>, circular motion requires an inward centripetal acceleration <span class="math">v^{2}/r</span>. In this framework, that requirement is met by redistributing the background field to produce the necessary inward concentration.</p>

<p>Because the total acceleration is finite, this redistribution cannot be local: any concentration within the system must be balanced globally. Rotational inertia therefore depends on the global distribution of mass through the shared acceleration field, providing a Machian interpretation.</p>

<h3>Regularity of the Manifold</h3>

<p>Because the manifold acceleration scale is finite, collapse approaches saturated configurations of finite density and radius rather than singular limits. The manifold accordingly remains smooth under the evolution defined by the geometry and does not admit singular collapse.</p>

<p>Causal ordering is fixed by the intrinsic geometry of allowable separations, not by any imposed signal speed. Only trajectories consistent with this ordering admit an operational time parameter, excluding closed timelike curves and the associated causal paradoxes.</p>

<p>The causal structure and finite acceleration budget thereby avoid singularities and causal paradoxes.</p>

<h2>Local Dynamics</h2>

<p>Having established the gravitational and causal structure, we now define the operational dynamics governing motion within the manifold.</p>

<h3>Operational Time</h3>

<p>Imposing the null condition <span class="math">Δ s^2=0</span> on equation (25) gives</p>

<a id="equation-45"></a>
<table><tr><td><pre><code>(V_0 - At)^2 \Delta t^2=\Delta x^2,</code></pre></td><td><strong>(45)</strong></td></tr></table>

<p>so that</p>

<a id="equation-46"></a>
<table><tr><td><pre><code>\Delta t=\frac{\Delta x}{(V_0 - At)}.</code></pre></td><td><strong>(46)</strong></td></tr></table>

<p>This defines the null boundary of the local geometry and fixes the relation between spatial separation and temporal increment through the scale <span class="math">(V_0 - At)</span>.</p>

<p>Observable time is defined operationally by null exchange between nearby worldlines. One tick of the clock is a complete round trip of a signal along null trajectories, and the temporal parameter <span class="math">t</span> is identified with the number of such cycles, which defines an invariant ordering of events. The null relation ensures that each cycle corresponds to a temporal increment determined by the local scale <span class="math">(V_0 - At)</span> at that epoch, and restricts admissible trajectories to those consistent with this ordering.</p>

<p>The null relation therefore fixes the local causal structure and operational ordering of events. Observable motion and the invariant timelike interval both arise from this same local geometry, so causality, motion, and measurable duration are unified through the null structure of the manifold.</p>

<h3>Proper Time</h3>

<p>Using the local interval defined in equation (25),</p>

<a id="equation-47"></a>
<table><tr><td><pre><code>ds^2 = -(V_0 - At)^2\,dt^2 + dx^2,</code></pre></td><td><strong>(47)</strong></td></tr></table>

<p>proper time defines the invariant timelike interval along admissible trajectories, <span class="math">dτ^2 \equiv -ds^2</span>, so that</p>

<a id="equation-48"></a>
<table><tr><td><pre><code>d\tau^2 = (V_0 - At)^2\,dt^2 - dx^2,</code></pre></td><td><strong>(48)</strong></td></tr></table>

<p>giving</p>

<a id="equation-49"></a>
<table><tr><td><pre><code>d\tau = (V_0 - At)\sqrt{1 - \frac{v^2}{(V_0 - At)^2}}\;dt,</code></pre></td><td><strong>(49)</strong></td></tr></table>

<p>where <span class="math">v = dx/dt</span>.</p>

<h3>Local Momentum</h3>

<p>A non-zero manifold acceleration defines a global acceleration flux that selects a timelike direction. The local interval arises from the Euclidean bilocal scalar (equation (5)) with orthogonal temporal (imaginary) and spatial (real) components, so it resolves as projections of a tangent of fixed magnitude whose spatial and temporal components vary with orientation. In the homogeneous local limit, this orientation is represented by an angle <span class="math">θ</span> relative to the flux.</p>

<p>Let <span class="math">dλ</span> denote an increment of the underlying constant-magnitude tangent. Resolving the tangent via the local invariant (equation (25)), the orthogonal projections admit a representation in terms of an angle <span class="math">θ</span>, yielding</p>

<a id="equation-50"></a>
<table><tr><td><pre><code>dx = (V_0 - At)\sin\theta\,d\lambda,\qquad dt = \cos\theta\,d\lambda.</code></pre></td><td><strong>(50)</strong></td></tr></table>

<p>Observable kinematics are defined with respect to the temporal parameter <span class="math">t</span>. In the homogeneous local limit, the measurable velocity may be expressed as</p>

<a id="equation-51"></a>
<table><tr><td><pre><code>v = \frac{dx}{dt} = (V_0 - At)\tan\theta.</code></pre></td><td><strong>(51)</strong></td></tr></table>

<p>The null boundary is reached when <span class="math">v = V_0 - At</span>, which requires <span class="math">\tanθ = 1</span> and therefore <span class="math">θ = π/4</span>. Observable motion is accordingly restricted to the timelike domain <span class="math">0 \le θ &lt; π/4</span>. At this boundary, the underlying geometric structure remains well-defined through the orientation angle <span class="math">θ</span>, but the kinematic description in terms of <span class="math">t</span> ceases to apply. Beyond this limit, the projection geometry persists but no longer corresponds to observable motion; its continuation is defined in terms of phase evolution.</p>

<p>Momentum is defined from the observable velocity,</p>

<a id="equation-52"></a>
<table><tr><td><pre><code>P = m\,v,</code></pre></td><td><strong>(52)</strong></td></tr></table>

<p>and is the spatial projection of the geometric momentum scale <span class="math">m(V_0-At)</span> with respect to the temporal parameter <span class="math">t</span>.</p>

<h3>Local Action</h3>

<p>In the coincidence limit, the bilocal interval (equation (25)) defines a local tangent of fixed magnitude and an invariant interval <span class="math">ds</span> describing local manifold separation. Weighting this invariant separation by the tangent momentum scale</p>

<a id="equation-53"></a>
<table><tr><td><pre><code>P_{\mathrm{geom}} \equiv m(V_0-At),</code></pre></td><td><strong>(53)</strong></td></tr></table>

<p>defines the invariant geometric action increment,</p>

<a id="equation-54"></a>
<table><tr><td><pre><code>dS_{\mathrm{geom}} \equiv P_{\mathrm{geom}}\,ds,</code></pre></td><td><strong>(54)</strong></td></tr></table>

<p>with quadratic form</p>

<a id="equation-55"></a>
<table><tr><td><pre><code>dS_{\mathrm{geom}}^2 = P_{\mathrm{geom}}^2\,ds^2.</code></pre></td><td><strong>(55)</strong></td></tr></table>

<p>Using the local invariant</p>

<a id="equation-56"></a>
<table><tr><td><pre><code>ds^2 = - (V_0 - At)^2 dt^2 + dx^2,</code></pre></td><td><strong>(56)</strong></td></tr></table>

<p>the action-space interval becomes</p>

<a id="equation-57"></a>
<table><tr><td><pre><code>dS_{\mathrm{geom}}^2 =m^2(V_0-At)^2\left[-(V_0-At)^2 dt^2 + dx^2\right].</code></pre></td><td><strong>(57)</strong></td></tr></table>

<p>The temporal component defines the geometric energy scale associated with tangent evolution.</p>

<a id="eq:geometric_energy_definition"></a>
<table><tr><td><pre><code>E_{\mathrm{geom}}(t)\equiv -m(V_0-At)^2,</code></pre></td><td><strong>(58)</strong></td></tr></table>

<p>while the spatial component is governed by the same geometric momentum scale <span class="math">P_{geom}=m(V_0-At)</span>.</p>

<p>Evaluating the local interval on the tangent direction shows that the fixed-magnitude tangent satisfies <span class="math">|ds/dλ|^2 = (V_0-At)^2</span>, so that</p>

<a id="equation-59"></a>
<table><tr><td><pre><code>ds=(V_0-At)\,d\lambda,</code></pre></td><td><strong>(59)</strong></td></tr></table>

<p>and therefore</p>

<a id="eq:action_definition"></a>
<table><tr><td><pre><code>dS_{\mathrm{geom}} = m(V_0-At)^2\,d\lambda,</code></pre></td><td><strong>(60)</strong></td></tr></table>

<p>so the invariant geometric action accumulates along the manifold tangent,</p>

<a id="equation-61"></a>
<table><tr><td><pre><code>S_{\mathrm{geom}} = \int dS_{\mathrm{geom}}.</code></pre></td><td><strong>(61)</strong></td></tr></table>

<p>Observable action is obtained by projection into the timelike sector,</p>

<a id="equation-62"></a>
<table><tr><td><pre><code>dS = P\,dx - H\,dt,</code></pre></td><td><strong>(62)</strong></td></tr></table>

<p>which defines the canonical momentum and observable Hamiltonian. The observable action therefore plays the role of the Hamilton–Jacobi principal function, while the invariant geometric action remains well-defined across the full manifold.</p>

<h3>Phase Evolution</h3>

<p>The projection-based kinematic description applies within the timelike sector, where the local invariant defines a real proper-time interval. At the null boundary, <span class="math">ds^2=0</span> and <span class="math">dτ \to 0</span>, marking the limit of observable timelike motion. Beyond this boundary, observable motion ceases, while the invariant geometric structure remains well-defined and the geometric action continues to accumulate along the manifold tangent.</p>

<p>The continued evolution of this invariant scalar is represented as phase,</p>

<a id="equation-63"></a>
<table><tr><td><pre><code>\phi = \frac{S_{\mathrm{geom}}}{\hbar},</code></pre></td><td><strong>(63)</strong></td></tr></table>

<p>where <span class="math">ℏ</span> sets the scale relating geometric action to phase. Because action has units of length within the present framework, <span class="math">ℏ</span> acquires the interpretation of a minimum indivisible bilocal separation, a necessary structural feature of a geometry that does not admit infinitesimal separations.</p>

<p>Phase evolution therefore represents the continuation of invariant geometric evolution beyond the proper-time-parametrized sector, while the underlying manifold evolution remains continuous across the null boundary.</p>

<h2>Late-Time Evolution</h2>

<p>The distance–redshift relation derived from the bilocal interval predicts the late-time expansion history.</p>

<h3>Type Ia Supernova Sample</h3>

<p>We use the Pantheon+ compilation of 1701 spectroscopically confirmed Type Ia supernovae presented by Brout et al. [Brout2022]. The publicly released Pantheon+SH0ES dataset provides the observed distance moduli <span class="math">μ_{obs}</span>, redshifts <span class="math">z</span>, and the full STAT+SYS covariance matrix for covariance-weighted <span class="math">χ^2</span> inference. The distance moduli are absolutely calibrated through the SH0ES determination of the Type Ia absolute magnitude <span class="math">M_B</span>.</p>

<h3>Luminosity Distance</h3>

<p>The spatial separation predicted by the manifold geometry is given by equation (17). The luminosity distance follows from the standard relation <span class="math">D_L(z) = (1+z)D_C(z)</span>. Substituting the spatial separation yields the corresponding analytic luminosity distance</p>

<a id="eq:pme_luminosity_distance"></a>
<table><tr><td><pre><code>D_L(z) =-\frac{t_o\left(A t_o - 2V_0\right) z(1+z)}{2+z}.</code></pre></td><td><strong>(64)</strong></td></tr></table>

<h3>Distance Modulus</h3>

<p>Type Ia supernova observations are reported in terms of the distance modulus, which relates the observed luminosity distance to the measured brightness of each supernova,</p>

<a id="equation-65"></a>
<table><tr><td><pre><code>\mu(z) = 5\log_{10}\!\left(\frac{D_L(z)}{10\,\mathrm{pc}}\right).</code></pre></td><td><strong>(65)</strong></td></tr></table>

<h3>Manifold Kinematic Parameters</h3>

<p>The local null scale at the observation epoch is</p>

<a id="eq:co_definition"></a>
<table><tr><td><pre><code>c_o = V_0 - A t_o .</code></pre></td><td><strong>(66)</strong></td></tr></table>

<p>Operationally, photon exchange is used as a proxy for this local null scale, so the measured speed of light at the observation epoch determines <span class="math">c_o</span>, fixing the integration constant,</p>

<a id="eq:velocity_boundary_condition"></a>
<table><tr><td><pre><code>V_0 = c_o + A t_o .</code></pre></td><td><strong>(67)</strong></td></tr></table>

<p>With the manifold acceleration <span class="math">A</span> determined from the baryonic Tully–Fisher analysis, the Cepheid-calibrated Pantheon+ subset is used to determine the observation epoch <span class="math">t_o</span> on the absolute distance scale. For each candidate value of <span class="math">t_o</span>, the corresponding <span class="math">V_0</span> follows algebraically from equation (67), and theoretical distance moduli <span class="math">μ_{th}(z)</span> are evaluated at the calibration-set redshifts. These are compared with the observed values <span class="math">μ_{obs}(z)</span>, defining the residual vector</p>

<a id="equation-68"></a>
<table><tr><td><pre><code>r_i = \mu_{\mathrm{obs}}(z_i) - \mu_{\mathrm{th}}(z_i).</code></pre></td><td><strong>(68)</strong></td></tr></table>

<p>The best-fit observation epoch is obtained by minimizing the covariance-weighted chi-square statistic</p>

<a id="equation-69"></a>
<table><tr><td><pre><code>\chi^2 = r^{\mathrm T} C^{-1} r,</code></pre></td><td><strong>(69)</strong></td></tr></table>

<p>where <span class="math">C</span> is the full Pantheon+ STAT+SYS covariance matrix. The resulting best-fit value of <span class="math">t_o</span> then determines <span class="math">V_0</span>, completing the kinematic parameter set. The resulting parameters are listed in Table 1.</p>

<figure id="tab:pme_parameters">
<table>
<thead><tr><th>Parameter</th><th>Value</th></tr></thead>
<tbody>
<tr><td><span class="math">A</span></td><td><span class="math">3.7\times10^{-11} m s^{-2}</span></td></tr>
<tr><td><span class="math">V_0</span></td><td><span class="math">3.16\times10^{8} m s^{-1}</span></td></tr>
<tr><td><span class="math">t_o</span></td><td><span class="math">4.51\times10^{17} s</span></td></tr>
</tbody>
</table>
<figcaption><strong>Table 1.</strong> PME kinematic parameters determined from BTFR and Cepheid-calibrated Pantheon+ subset.</figcaption>
</figure>

<h3>Comparison with Observations</h3>

<a id="fig:hubblechart"></a>
<p align="center"><img src="figures/hubble-diagram.png" alt="Figure 5: Pantheon+SH0ES distance moduli as a function of redshift &lt;span class=&quot;math&quot;&gt;z&lt;/span&gt;, compared with the PME prediction and the spatially flat FLRW model. PME parameters are fixed by BTFR and Cepheid calibration. FLRW parameters are fixed by the Planck 2018 results." width="700"></p>
<p align="center"><em><strong>Figure 5.</strong> Pantheon+SH0ES distance moduli as a function of redshift <span class="math">z</span>, compared with the PME prediction and the spatially flat FLRW model. PME parameters are fixed by BTFR and Cepheid calibration. FLRW parameters are fixed by the Planck 2018 results.</em></p>

<p>Figure 5 shows the PME prediction and the Planck 2018 FLRW model compared with the Pantheon+SH0ES data.</p>

<p>The Pantheon+SH0ES dataset provides observed distance moduli <span class="math">μ_{obs}(z)</span> calibrated on an absolute scale through the SH0ES determination of the Type Ia supernova absolute magnitude. This calibration is applied identically to both models.</p>

<p>Each model predicts <span class="math">D_L(z)</span>, which is mapped to <span class="math">μ_{th}(z)</span> using the definition of <span class="math">μ(z)</span> introduced earlier. We compare <span class="math">μ_{th}(z)</span> to <span class="math">μ_{obs}(z)</span> using the full Pantheon+ STAT+SYS covariance matrix.</p>

<p>PME is evaluated using the fixed parameter set derived above. FLRW is evaluated using a spatially flat model specified by the Planck 2018 parameter set <span class="math">Ω_m = 0.315</span>, <span class="math">Ω_Λ = 1-Ω_m</span>, and <span class="math">H_0 = 67.4 km s^{-1 Mpc^{-1}}</span> [Planck2018]. The comparison is performed on the out-of-sample supernovae, excluding the Cepheid calibration records.</p>

<p>The resulting covariance-weighted chi-square values are</p>

<a id="equation-70"></a>
<table><tr><td><pre><code>\chi^2_{\mathrm{PME}}=2726,\qquad \chi^2_{\mathrm{FLRW}}=4049,</code></pre></td><td><strong>(70)</strong></td></tr></table>

<p>for <span class="math">ν=1625</span>, corresponding to reduced values <span class="math">χ^2/ν=1.68</span> and <span class="math">2.49</span>, respectively. PME predicts the observed distance moduli substantially more accurately than the Planck 2018 FLRW model across the Pantheon+SH0ES sample, without dark sector parameters.</p>

<h3>Hubble Function</h3>

<p>The Hubble expansion rate is defined by the fractional rate of change of the real spatial extent of the manifold, <span class="math">H(t) \equiv \dot{L}(t)/{L(t)}</span>. Differentiating equation (7) gives <span class="math">\dot{L}(t)=V_0-At</span>, so</p>

<a id="eq:hubble_function"></a>
<table><tr><td><pre><code>H(t) = \frac{V_0 - At}{V_0 t - \frac{1}{2}A t^2}.</code></pre></td><td><strong>(71)</strong></td></tr></table>

<p>Evaluating equation (71) at the observation epoch <span class="math">t=t_o</span> using the best-fit manifold parameters gives the present-day expansion rate</p>

<a id="equation-72"></a>
<table><tr><td><pre><code>H_0 = 66.5\,\mathrm{km\,s^{-1}\,Mpc^{-1}}.</code></pre></td><td><strong>(72)</strong></td></tr></table>

<p>The Hubble constant therefore emerges as a prediction rather than a fitted parameter.</p>

<h3>Cosmic Time</h3>

<p>The redshift–time relation differs from standard cosmological evolution due to the underlying parabolic evolution. Table 2 compares the resulting cosmic times with those from FLRW algorithms.</p>

<figure id="tab:cosmic_time_comparison">
<table>
<thead><tr><th><span class="math">z</span></th><th>PME [Myr]</th><th>FLRW [Myr]</th></tr></thead>
<tbody>
<tr><td>0</td><td>14,283</td><td>13,791</td></tr>
<tr><td>1</td><td>7,039</td><td>5,840</td></tr>
<tr><td>10</td><td>1,265</td><td>470</td></tr>
<tr><td>100</td><td>137</td><td>16.4</td></tr>
<tr><td>1,000</td><td>13.9</td><td>0.429</td></tr>
</tbody>
</table>
<figcaption><strong>Table 2.</strong> Cosmic time as a function of redshift. PME predictions are compared with FLRW values computed using Planck 2018 parameters [Planck2018].</figcaption>
</figure>

<p>The parabolic expansion yields uniformly larger cosmic ages than FLRW, significantly extending the available time for early structure formation.</p>

<h2>Early-Time Evolution</h2>

<p>Independent constraints arise from the cosmic microwave background (CMB), whose acoustic scale probes the distance to last scattering relative to the sound horizon.</p>

<p>The expansion history is determined by the PME kinematics derived above, while recombination microphysics is evaluated using standard rate equations. Thermodynamic quantities are mapped using the scale factor</p>

<a id="eq:scale_factor"></a>
<table><tr><td><pre><code>a(t) = \frac{L(t)}{L(t_o)} .</code></pre></td><td><strong>(73)</strong></td></tr></table>

<h3>Baryon and Photon Densities</h3>

<p>The recombination history and pre-decoupling sound speed require the baryon and photon densities. The baryon density is fixed by the manifold acceleration scale rather than introduced as an independent cosmological parameter. This follows from the local divergence law (equation (33)), which relates the sourced acceleration field to the baryonic density.</p>

<p>For a homogeneous baryonic distribution of density <span class="math">ρ_b</span> within a region of characteristic size <span class="math">L</span>, the enclosed mass is</p>

<a id="equation-74"></a>
<table><tr><td><pre><code>M(L)=\frac{4\pi}{3}L^3\rho_b ,</code></pre></td><td><strong>(74)</strong></td></tr></table>

<p>so the corresponding baryon-sourced acceleration at radius <span class="math">L</span> is</p>

<a id="equation-75"></a>
<table><tr><td><pre><code>\frac{GM(L)}{L^2}=\frac{4\pi}{3}G L\rho_b .</code></pre></td><td><strong>(75)</strong></td></tr></table>

<p>Evaluating this expression at the present manifold extent <span class="math">L(t_o)</span>, which contains the full homogeneous baryonic source, and identifying it with the inferred manifold acceleration <span class="math">A</span> gives</p>

<a id="equation-76"></a>
<table><tr><td><pre><code>A=\frac{4\pi}{3}G L(t_o)\rho_b ,</code></pre></td><td><strong>(76)</strong></td></tr></table>

<p>hence</p>

<a id="equation-77"></a>
<table><tr><td><pre><code>\rho_b=\frac{3A}{4\pi G\,t_o\left(V_0-\frac{1}{2}A t_o\right)} .</code></pre></td><td><strong>(77)</strong></td></tr></table>

<p>Using the kinematic parameters determined in the previous sections yields</p>

<a id="equation-78"></a>
<table><tr><td><pre><code>\rho_b = 9.49\times10^{-28}\,\mathrm{kg\,m^{-3}}.</code></pre></td><td><strong>(78)</strong></td></tr></table>

<p>This value is consistent with independent observational estimates of the present-day baryon density from primordial light-element abundances [Cooke2018].</p>

<p>The photon density is determined from the measured CMB temperature <span class="math">T_γ=2.725 K</span>. The mapping between temperature and photon density depends on the local geometric scale <span class="math">(V_0 - At)</span>, so the photon density is treated as epoch dependent rather than constant. For a blackbody radiation field, the photon number density is</p>

<a id="equation-79"></a>
<table><tr><td><pre><code>n_\gamma(t)=\frac{2\zeta(3)}{\pi^2}\left(\frac{k_B T_\gamma}{\hbar (V_0-At)}\right)^3 ,</code></pre></td><td><strong>(79)</strong></td></tr></table>

<p>and, following the geometric sign convention of Eq. (58), the mean photon energy is</p>

<a id="equation-80"></a>
<table><tr><td><pre><code>\langle E_\gamma\rangle=-\frac{\pi^4}{30\zeta(3)}k_B T_\gamma .</code></pre></td><td><strong>(80)</strong></td></tr></table>

<p>The corresponding photon energy density is</p>

<a id="equation-81"></a>
<table><tr><td><pre><code>u_\gamma(t)=n_\gamma(t)\langle E_\gamma\rangle ,</code></pre></td><td><strong>(81)</strong></td></tr></table>

<p>so the mass-equivalent photon density becomes</p>

<a id="equation-82"></a>
<table><tr><td><pre><code>\rho_\gamma(t)=\frac{u_\gamma(t)}{-(V_0-At)^2}.</code></pre></td><td><strong>(82)</strong></td></tr></table>

<p>These densities determine the baryon–photon momentum ratio and the free-electron density entering the visibility function.</p>

<h3>Recombination Epoch</h3>

<p>The recombination epoch is the time of maximum photon visibility, i.e. the most probable last-scattering time in the baryon–photon plasma.</p>

<p>To determine the ionization history, we evaluate the standard recombination rate equations using <code>Recfast++</code> with the PME expansion geometry. The background evolution is provided by the PME Hubble function (equation (71)) in place of the FLRW algorithm, with the expansion rate governed by the best-fit manifold parameters. The baryon sector is specified by the present-day baryon density derived above. The resulting ionization history is used to interpolate the free-electron fraction <span class="math">x_e(z)</span> entering the visibility function. The free-electron number density <span class="math">n_e(t)</span> is defined as</p>

<a id="equation-83"></a>
<table><tr><td><pre><code>n_e(t)=x_e(t)\,\frac{\rho_b}{m_p}\,a(t)^{-3},</code></pre></td><td><strong>(83)</strong></td></tr></table>

<p>where <span class="math">ρ_b</span> is the present-day baryon mass density, <span class="math">m_p</span> is the proton mass.</p>

<p>The Thomson scattering rate is expressed in terms of the local particle density, cross section, and local geometric scale,</p>

<a id="equation-84"></a>
<table><tr><td><pre><code>\Gamma_T(t)=n_e(t)\,\sigma_T\,(V_0 - At),</code></pre></td><td><strong>(84)</strong></td></tr></table>

<p>where <span class="math">σ_T</span> is the Thomson cross section. The optical depth is then defined as the accumulated interaction probability along the manifold history,</p>

<a id="equation-85"></a>
<table><tr><td><pre><code>\tau_T(t)=\int_t^{t_o}\Gamma_T(t&#x27;)\,dt&#x27;.</code></pre></td><td><strong>(85)</strong></td></tr></table>

<p>The corresponding visibility function is</p>

<a id="equation-86"></a>
<table><tr><td><pre><code>g(t)=\Gamma_T(t)\,e^{-\tau_T(t)} .</code></pre></td><td><strong>(86)</strong></td></tr></table>

<p>Evaluating <span class="math">g(t)</span> on the PME expansion background using the <code>Recfast++</code> microphysics parametrization yields a maximum at <span class="math">z_* = 1039</span>, <span class="math">t_* = 13.4 Myr</span> shown in Fig. 6.</p>

<a id="fig:visibility"></a>
<p align="center"><img src="figures/visibility-function.png" alt="Figure 6: Photon visibility function &lt;span class=&quot;math&quot;&gt;g(z)&lt;/span&gt; evaluated using the recombination history on the PME expansion background. The peak defines the recombination epoch, yielding &lt;span class=&quot;math&quot;&gt;z_* = 1039&lt;/span&gt;." width="700"></p>
<p align="center"><em><strong>Figure 6.</strong> Photon visibility function <span class="math">g(z)</span> evaluated using the recombination history on the PME expansion background. The peak defines the recombination epoch, yielding <span class="math">z_* = 1039</span>.</em></p>

<h3>Sound Horizon</h3>

<p>Prior to recombination, baryons and photons form a tightly coupled fluid whose acoustic interaction distance defines the sound horizon. The thermodynamic evolution follows the scale factor <span class="math">a(t)</span> defined in equation (73).</p>

<p>The baryon–photon momentum ratio is</p>

<a id="equation-87"></a>
<table><tr><td><pre><code>R(t)=\frac{3\rho_b}{4\rho_\gamma(t)}\,\frac{a(t)^{-3}}{a(t)^{-4}}=\frac{3\rho_b}{4\rho_\gamma(t)}\,a(t),</code></pre></td><td><strong>(87)</strong></td></tr></table>

<p>giving the sound speed</p>

<a id="equation-88"></a>
<table><tr><td><pre><code>c_s(t)=\frac{c_{\mathrm{c}}(t)}{\sqrt{3\left(1+R(t)\right)}} .</code></pre></td><td><strong>(88)</strong></td></tr></table>

<p>The causal expansion rate <span class="math">c_{c}(t)</span> sets the rate at which interactions can be ordered through the operational clock and thus defines the effective causal scale entering the acoustic horizon integral, so that the sound horizon is</p>

<a id="equation-89"></a>
<table><tr><td><pre><code>r_s=\int_0^{t_*} c_s(t)\,dt .</code></pre></td><td><strong>(89)</strong></td></tr></table>

<p>Evaluating this expression using the manifold parameters yields <span class="math">r_s=3.7 Mpc</span>.</p>

<h3>Acoustic Angular Scale</h3>

<p>The observed acoustic angle is determined by the ratio of the sound horizon at recombination to the bilocally assigned transverse size of the emission–observation pair. <span class="math">L(t)</span> denotes the circumference of the spatial slice at epoch <span class="math">t</span>, so the relevant transverse quantity is the effective bilocal transverse circumference associated with the ordered pair <span class="math">(t_*,t_o)</span>.</p>

<p>To define this quantity, consider a transverse bilocal path whose endpoints lie at antipodal points on the spatial slices at emission and observation. The transverse separations between antipodal points on those slices are therefore the corresponding slice circumferences, <span class="math">L(t_*)</span> and <span class="math">L(t_o)</span>. Applying the bilocal spatial rule of equation (3) to this transverse configuration defines the bilocal spatial separation between antipodal transverse endpoints, which we identify as the effective transverse circumference,</p>

<a id="eq:bilocal_transverse_circumference"></a>
<table><tr><td><pre><code>C_\perp \equiv \frac12\left[L(t_o)+L(t_*)\right].</code></pre></td><td><strong>(90)</strong></td></tr></table>

<p>Using the redshift relation from equation (15), this becomes</p>

<a id="equation-91"></a>
<table><tr><td><pre><code>C_\perp=\frac{L(t_o)}{2}\,\frac{2+z_*}{1+z_*}.</code></pre></td><td><strong>(91)</strong></td></tr></table>

<p>The corresponding effective transverse radius is</p>

<a id="equation-92"></a>
<table><tr><td><pre><code>r_\perp=\frac{C_\perp}{2\pi}=\frac{L(t_o)}{4\pi}\,\frac{2+z_*}{1+z_*}.</code></pre></td><td><strong>(92)</strong></td></tr></table>

<p>The acoustic angular scale is then</p>

<a id="equation-93"></a>
<table><tr><td><pre><code>\theta_*=\frac{r_s}{r_\perp}.</code></pre></td><td><strong>(93)</strong></td></tr></table>

<p>Substituting the expression above for <span class="math">r_\perp</span> gives</p>

<a id="equation-94"></a>
<table><tr><td><pre><code>\theta_*=\frac{4\pi(1+z_*)}{L(t_o)(2+z_*)}\,r_s.</code></pre></td><td><strong>(94)</strong></td></tr></table>

<p>Using equation (7) evaluated at <span class="math">t_o</span> yields</p>

<a id="eq:acoustic_angle_final"></a>
<table><tr><td><pre><code>\theta_*=\frac{8\pi(1+z_*)}{t_o(2V_0-A t_o)(2+z_*)}\,r_s.</code></pre></td><td><strong>(95)</strong></td></tr></table>

<p>Evaluating this expression with the manifold parameters gives</p>

<a id="equation-96"></a>
<table><tr><td><pre><code>\theta_* = 0.0103.</code></pre></td><td><strong>(96)</strong></td></tr></table>

<p>Expressed in the conventional CMB notation,</p>

<a id="equation-97"></a>
<table><tr><td><pre><code>100\,\theta_* = 1.03.</code></pre></td><td><strong>(97)</strong></td></tr></table>

<p>This result follows from the PME expansion geometry combined with standard recombination microphysics.</p>

<h2>Discussion</h2>

<p>A detailed nucleosynthesis calculation has not been attempted within the present framework. Standard Big Bang nucleosynthesis treatments assume time-independent microphysics, including fixed particle rest energies and equilibrium thermodynamic mappings. In PME, however, the effective manifold energy scale varies explicitly with cosmic time through <span class="math">E_{geom}=-m(V_0-At)^2</span>, derived from the temporal component of the inertia-weighted action-space interval, and the operational reaction clock need not coincide with the geometric expansion time. These features break the time-translation invariance implicit in conventional BBN calculations, so the reaction network must be re-derived within the PME framework.</p>

<p>This distinction also affects baryon asymmetry. In equilibrium with time-reversal symmetric, time-independent microphysics, matter–antimatter annihilation drives the net baryon number toward zero, leaving a radiation-dominated universe. Standard cosmology therefore treats the baryon-to-photon ratio as an external parameter rather than deriving it from Standard Model physics. The explicitly time-dependent evolution of the PME energy scale relaxes the equilibrium assumptions underlying this argument, permitting a nonzero residual baryon density without invoking additional symmetry-breaking mechanisms. PME therefore provides a framework in which baryon asymmetry may arise from the underlying geometric evolution, allowing nucleosynthesis to be formulated self-consistently once the reaction network is derived within this context.</p>

<p>The framework predicts a residual non-Keplerian contribution to bound motion with radial scaling <span class="math">A r^2/GM</span>. In compact systems this effect is suppressed and becomes significant only at larger radii. Solar-System observations therefore constrain the model but do not probe the regime in which the background term becomes dynamically dominant. Improved precision, particularly at large heliocentric distances, should reveal systematic departures from purely Keplerian motion. Detection or exclusion of such a signal provides a direct test of the construction.</p>

<p>Extending the bilocal framework to perturbations, structure growth, nucleosynthesis, and a fully intrinsic treatment of recombination is required to assess viability beyond the homogeneous background solution. The present formulation establishes a constrained kinematic structure whose physical adequacy must ultimately be judged by its ability to reproduce observational phenomena across these additional domains.</p>

<h3>Code Availability</h3>

<p>A computational notebook implementing the bilocal geometry, distance–redshift relation, and observational analysis is publicly available at:</p>

<p align="center"><a href="https://www.wolframcloud.com/obj/32b2e831-2cbe-4ff5-b821-aa23f476f015">https://www.wolframcloud.com/obj/32b2e831-2cbe-4ff5-b821-aa23f476f015</a></p>

<p>The notebook reproduces the results and figures presented in this work and is provided to enable independent verification of the calculations.</p>

<h2>Conclusion</h2>

<p>A constrained bilocal construction on a complex manifold yields a quadratic interval whose local reduction yields a homogeneous acceleration scale. This single geometric scale governs both the parabolic evolution of the manifold and the redistribution of acceleration flux in gravitationally bound systems. The bilocal geometry produces an emergent local null constraint, defines an invariant action geometry, and admits a canonical decomposition into temporal and spatial contributions. From this structure, a Hamiltonian system and associated Hamilton–Jacobi equation arise as the projection of the inertia-weighted invariant geometric action into the timelike sector, so that particle motion follows geodesics of action space without introducing independent dynamical postulates, while phase evolution provides its continuation beyond the observable domain. Gravity and inertia therefore emerge as complementary manifestations of a conserved acceleration field inherited from the manifold kinematics.</p>

<p>The evolution implied by this construction yields a closed analytic distance–redshift relation, from which the Pantheon+ Type Ia supernova luminosity distances follow directly on an absolute scale. The same parameter set predicts the present-day Hubble constant and produces uniformly extended cosmic ages. In the local-reduction regime, redistribution of the homogeneous acceleration field generates an inverse-square sourced component and a circular-orbit envelope consistent with the observed baryonic Tully–Fisher relation. The acceleration scale inferred from galaxy dynamics then fixes the baryonic density of the homogeneous universe, linking galactic and cosmological observables without introducing non-baryonic dark matter or dark energy components.</p>

<p>The bilocal construction also determines the causal horizon and implies a constant ratio between the causal domain and manifold extent, placing the last-scattering surface within a single causal region and accounting for large-scale isotropy. The geometry yields a transverse scale for recombination that reproduces the observed acoustic angular scale. Because the available acceleration flux is finite, gravitational collapse approaches saturated configurations, eliminating curvature singularities and enforcing a globally ordered causal structure. Rotational inertia emerges from redistribution of the same finite acceleration budget, providing a Machian interpretation in which local inertial behavior depends on the global distribution of inertial content.</p>

<p>Evolution, causal structure, action, gravity, inertia, and dynamical law therefore arise from a common bilocal origin, with all dynamics derived from the momentum weighted invariant separation, providing a unified explanation of isotropy, galaxy rotation, Type Ia supernova magnitudes, the acoustic scale, nonsingular gravitational collapse, the baryonic density, and the Hubble constant.</p>
