<h1 align="center">Gravity and Action from the Parabolic Metric Evolution of a Complex Manifold</h1>

<p align="center">
  <strong>Donald Airey</strong><br>
  ORCID: 0000-0002-2958-1545<br>
  Cooperstown, NY, USA<br>
  <a href="mailto:don@airey.us">don@airey.us</a>
</p>

<p align="center">
  <em>cosmology · gravitational theory · cosmic expansion · cosmological dynamics · Type Ia supernovae · large-scale structure</em>
</p>

<hr>

<h2>Abstract</h2>

<p>
We present a bilocal geometric framework in which separations are defined between ordered pairs of events rather than by a local infinitesimal metric. This construction is motivated by the need to represent global evolution in a manner that remains well-defined over finite separations while admitting a smooth local limit.
</p>

<p>
The resulting geometry is formulated on a complex manifold with an imaginary temporal coordinate and a real spatial coordinate. A constant manifold acceleration sets the global spatial scale and produces a parabolic cycle of expansion and contraction.
</p>

<p>
In the local reduction, the same acceleration scale yields a circular-orbit envelope consistent with the baryonic Tully–Fisher relation. At cosmological scales, the resulting analytic distance–redshift relation predicts the Pantheon+ Type Ia supernova luminosity distances on the SH0ES-calibrated absolute scale and yields a lower covariance-weighted χ² than Planck-calibrated FLRW, without invoking dark matter or dark energy.
</p>

<p>
The parabolic metric evolution, when combined with standard recombination microphysics, yields an acoustic angular scale consistent with Planck measurements.
</p>

<p align="center">
  <img src="figures/pme-manifold.png" alt="Complex parabolic metric manifold" width="700">
</p>

<p align="center">
  <em>Schematic representation of the complex parabolic metric manifold. Latitude lines correspond to spatial slices at fixed epoch, while longitude lines trace the temporal evolution of the manifold.</em>
</p>

<hr>

<h2>Overview</h2>

<p>
The Parabolic Metric Evolution (PME) framework develops a kinematic description in which large-scale cosmological evolution and local gravitational phenomena arise from a common geometric structure. Instead of assigning distances only through local infinitesimal metric elements, PME defines separations bilocally between ordered pairs of events.
</p>

<p>
The framework is governed by a single acceleration scale, denoted <code>A</code>, which determines both the parabolic evolution of the manifold and the local acceleration structure associated with gravitational systems.
</p>

<hr>

<h2>Foundational Structure</h2>

<ol>
  <li>Physical separations are defined bilocally between ordered pairs of events.</li>
  <li>The manifold evolution is governed by a constant acceleration scale <code>A</code>.</li>
  <li>The manifold is parameterized by an intrinsic evolution coordinate <code>χ</code>.</li>
  <li>Observable time is defined operationally through null exchange.</li>
</ol>

<p>The intrinsic evolution parameter is related to observable time by:</p>

<pre><code>χ = i t</code></pre>

<p>The induced spatial extent of the manifold is:</p>

<pre><code>L(t) = V₀ t − ½ A t²</code></pre>

<p>Differentiating twice gives:</p>

<pre><code>d²L/dt² = −A</code></pre>

<p>
Thus the manifold evolves with a constant deceleration magnitude <code>A</code>, universal and independent of position or epoch.
</p>

<hr>

<h2>Bilocal Geometry</h2>

<p>
The bilocal interval is constructed from a temporal functional and a spatial functional. The spatial slices scale with the global manifold extent <code>L(t)</code>, so separations at emission and observation satisfy:
</p>

<pre><code>Δxₑ¹ / L(tₑ) = Δxₒ¹ / L(tₒ)</code></pre>

<p>The symmetric midpoint spatial component is:</p>

<pre><code>Δs¹ = ½(Δxₒ¹ + Δxₑ¹)</code></pre>

<p>The bilocal interval is:</p>

<pre><code>Δs² = (Δs⁰)² + (Δs¹)²</code></pre>

<p>
where <code>Δs⁰</code> is purely imaginary and <code>Δs¹</code> is real.
</p>

<p align="center">
  <img src="figures/bilocal-geometry.png" alt="Bilocal geometry construction" width="700">
</p>

<p align="center">
  <em>Geometric construction of the bilocal interval between emission and observation events.</em>
</p>

<hr>

<h2>Cosmological Distance</h2>

<p>Redshift is defined by the ratio of manifold extents:</p>

<pre><code>1 + z = L(tₒ) / L(tₑ)</code></pre>

<p>Imposing the null condition yields the observable spatial separation:</p>

<pre><code>D_C(z) = tₒ(2V₀ − A tₒ) z / (2 + z)</code></pre>

<p>The luminosity distance is:</p>

<pre><code>D_L(z) = −tₒ(A tₒ − 2V₀) z(1 + z) / (2 + z)</code></pre>

<p>The distance modulus is:</p>

<pre><code>μ(z) = 5 log₁₀(D_L(z) / 10 pc)</code></pre>

<hr>

<h2>Causal Structure</h2>

<p>The causal horizon is:</p>

<pre><code>d_ch(t) = t(2V₀ − A t)</code></pre>

<p>The causal-boundary expansion rate is:</p>

<pre><code>c_c(t) = 2(V₀ − A t)</code></pre>

<p>The causal horizon and manifold extent satisfy:</p>

<pre><code>d_ch(t) / L(t) = 2</code></pre>

<p>
The causal horizon is therefore twice the manifold extent at all epochs, placing the last-scattering surface within a single causal region.
</p>

<hr>

<h2>Gravity</h2>

<p>In the local coincidence limit, the bilocal geometry reduces to:</p>

<pre><code>ds² = −(V₀ − A t)² dt² + dx²</code></pre>

<p>The inward acceleration decomposes into a homogeneous background and a sourced concentration:</p>

<pre><code>a_in(x) = a_bg + a_conc(x)</code></pre>

<p>The sourced weak-field limit satisfies:</p>

<pre><code>∇ · a_conc = −4πGρ_inertial</code></pre>

<p>For spherical symmetry:</p>

<pre><code>a_conc(r) = −GM(r)/r²</code></pre>

<hr>

<h2>Circular Orbits and the Baryonic Tully–Fisher Relation</h2>

<p>For circular motion:</p>

<pre><code>v² = A r + GM_b(r)/r</code></pre>

<p>Solving for enclosed baryonic mass:</p>

<pre><code>M_b(r) = r(v² − A r)/G</code></pre>

<p>The maximum baryonic mass compatible with circular orbit speed <code>v</code> is:</p>

<pre><code>M_max(v) = v⁴ / (4 A G)</code></pre>

<p>
This gives the scaling <code>M ∝ v⁴</code>, consistent with the observed baryonic Tully–Fisher relation.
</p>

<p align="center">
  <img src="figures/fundamental-plane.png" alt="PME fundamental plane" width="750">
</p>

<p align="center">
  <em>PME fundamental plane of circular-orbit solutions.</em>
</p>

<p align="center">
  <img src="figures/btfr-chart.png" alt="Baryonic Tully-Fisher relation" width="700">
</p>

<p align="center">
  <em>Baryonic mass versus outer rotation speed for the SPARC galaxy sample, compared with the PME circular-orbit envelope.</em>
</p>

<hr>

<h2>Local Dynamics</h2>

<h3>Operational Time</h3>

<p>The null condition gives:</p>

<pre><code>(V₀ − A t)² Δt² = Δx²</code></pre>

<p>so that:</p>

<pre><code>Δt = Δx / (V₀ − A t)</code></pre>

<p>Observable time is defined operationally by null exchange between nearby worldlines.</p>

<h3>Proper Time</h3>

<pre><code>dτ² = (V₀ − A t)² dt² − dx²</code></pre>

<pre><code>dτ = (V₀ − A t) √(1 − v²/(V₀ − A t)²) dt</code></pre>

<h3>Momentum</h3>

<pre><code>v = (V₀ − A t) tan θ</code></pre>

<pre><code>P = m v</code></pre>

<p>The null boundary occurs at:</p>

<pre><code>θ = π/4</code></pre>

<h3>Geometric Action</h3>

<p>The geometric momentum scale is:</p>

<pre><code>P_geom = m(V₀ − A t)</code></pre>

<p>The invariant geometric action increment is:</p>

<pre><code>dS_geom = P_geom ds</code></pre>

<p>The geometric energy scale is:</p>

<pre><code>E_geom(t) = −m(V₀ − A t)²</code></pre>

<h3>Phase Evolution</h3>

<p>Beyond the null boundary, geometric evolution continues as phase:</p>

<pre><code>φ = S_geom / ℏ</code></pre>

<hr>

<h2>Late-Time Evolution</h2>

<p>
The PME distance-redshift relation is compared with the Pantheon+SH0ES Type Ia supernova sample. PME is evaluated using parameters fixed by the baryonic Tully–Fisher relation and Cepheid calibration.
</p>

<table>
  <thead>
    <tr>
      <th align="left">Parameter</th>
      <th align="left">Value</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td><code>A</code></td>
      <td><code>3.7 × 10⁻¹¹ m s⁻²</code></td>
    </tr>
    <tr>
      <td><code>V₀</code></td>
      <td><code>3.16 × 10⁸ m s⁻¹</code></td>
    </tr>
    <tr>
      <td><code>tₒ</code></td>
      <td><code>4.51 × 10¹⁷ s</code></td>
    </tr>
  </tbody>
</table>

<p>The resulting covariance-weighted chi-square values are:</p>

<pre><code>χ²_PME  = 2726
χ²_FLRW = 4049</code></pre>

<p>for <code>ν = 1625</code>, corresponding to reduced values:</p>

<pre><code>χ²_PME/ν  = 1.68
χ²_FLRW/ν = 2.49</code></pre>

<p align="center">
  <img src="figures/hubble-diagram.png" alt="Hubble diagram" width="700">
</p>

<p align="center">
  <em>Pantheon+SH0ES distance moduli compared with PME and Planck-calibrated FLRW.</em>
</p>

<h3>Hubble Function</h3>

<pre><code>H(t) = (V₀ − A t) / (V₀ t − ½ A t²)</code></pre>

<p>The present-day expansion rate predicted by PME is:</p>

<pre><code>H₀ = 66.5 km s⁻¹ Mpc⁻¹</code></pre>

<h3>Cosmic Time Comparison</h3>

<table>
  <thead>
    <tr>
      <th align="right">z</th>
      <th align="right">PME [Myr]</th>
      <th align="right">FLRW [Myr]</th>
    </tr>
  </thead>
  <tbody>
    <tr><td align="right">0</td><td align="right">14,283</td><td align="right">13,791</td></tr>
    <tr><td align="right">1</td><td align="right">7,039</td><td align="right">5,840</td></tr>
    <tr><td align="right">10</td><td align="right">1,265</td><td align="right">470</td></tr>
    <tr><td align="right">100</td><td align="right">137</td><td align="right">16.4</td></tr>
    <tr><td align="right">1,000</td><td align="right">13.9</td><td align="right">0.429</td></tr>
  </tbody>
</table>

<hr>

<h2>Early-Time Evolution</h2>

<p>The scale factor is:</p>

<pre><code>a(t) = L(t) / L(tₒ)</code></pre>

<p>The present-day baryon density derived from the manifold acceleration scale is:</p>

<pre><code>ρ_b = 9.49 × 10⁻²⁸ kg m⁻³</code></pre>

<p>Using PME expansion geometry with standard recombination microphysics gives:</p>

<ul>
  <li>Recombination redshift: <code>z* = 1039</code></li>
  <li>Recombination time: <code>t* = 13.4 Myr</code></li>
  <li>Sound horizon: <code>r_s = 3.7 Mpc</code></li>
</ul>

<p align="center">
  <img src="figures/visibility-function.png" alt="Photon visibility function" width="700">
</p>

<p align="center">
  <em>Photon visibility function evaluated on the PME expansion background.</em>
</p>

<h3>Acoustic Angular Scale</h3>

<p>The predicted acoustic angular scale is:</p>

<pre><code>θ* = 0.0103</code></pre>

<p>or, in conventional CMB notation:</p>

<pre><code>100 θ* = 1.03</code></pre>

<hr>

<h2>Discussion</h2>

<p>
PME proposes a unified geometric origin for cosmological expansion, gravity, inertia, action, causal structure, and phase evolution. The framework eliminates independent dark matter and dark energy components, while linking local gravitational structure and cosmological observables through a single acceleration scale.
</p>

<p>
The framework predicts residual non-Keplerian contributions to bound motion with radial scaling <code>A r² / GM</code>. Solar-System observations constrain the model but do not probe the regime in which the background term becomes dynamically dominant. Improved precision at large heliocentric distances provides a direct observational test.
</p>

<p>
Further work is required to extend the bilocal framework to perturbations, structure growth, nucleosynthesis, and a fully intrinsic treatment of recombination.
</p>

<hr>

<h2>Code Availability</h2>

<p>
A computational notebook implementing the bilocal geometry, distance-redshift relation, and observational analysis is publicly available here:
</p>

<p align="center">
  <a href="https://www.wolframcloud.com/obj/32b2e831-2cbe-4ff5-b821-aa23f476f015">
    Wolfram Cloud Computational Notebook
  </a>
</p>

<hr>

<h2>Conclusion</h2>

<p>
A constrained bilocal construction on a complex manifold yields a quadratic interval whose local reduction produces a homogeneous acceleration scale. This single geometric scale governs both the parabolic evolution of the manifold and the redistribution of acceleration flux in gravitationally bound systems.
</p>

<p>
The evolution implied by this construction yields a closed analytic distance-redshift relation, predicts the present-day Hubble constant, produces extended cosmic ages, reproduces the baryonic Tully–Fisher relation, and yields an acoustic angular scale consistent with observation.
</p>

<p>
Evolution, causal structure, action, gravity, inertia, and dynamical law therefore arise from a common bilocal origin, with all dynamics derived from momentum-weighted invariant separation.
</p>

<hr>

<h2>Suggested Repository Structure</h2>

<pre><code>README.md
LICENSE
CITATION.cff
paper/
  PME.pdf
  PME.tex
figures/
  pme-manifold.png
  bilocal-geometry.png
  fundamental-plane.png
  btfr-chart.png
  hubble-diagram.png
  visibility-function.png
notebooks/
  analysis.nb
data/
</code></pre>
