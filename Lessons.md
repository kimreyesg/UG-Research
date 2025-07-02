# A quantum well

![Screenshot 2025-07-02 at 11 19 56 AM](https://github.com/user-attachments/assets/948b84b3-3a78-4690-b4db-d982bbdf1a04)


In semiconductor heterostructures, conduction and valence band edge profiles define quantum wells that selectively confine carriers. A lower conduction band edge in a layer (e.g. Semiconductor 1) forms a potential well for electrons, yielding quantized subbands and in-plane dispersions. Conversely, a higher valence band edge in that layer forms a potential well for holes, because holes energetically prefer regions where the valence band maximum is elevated, representing lower potential energy from the hole perspective. Thus, although the band edge diagrams may have identical shapes, conduction band wells confine electrons, while valence band wells confine holes, reflecting that electrons minimize their total energy by moving to lower band edges, while holes minimize theirs by moving to higher valence band edges.

## Important here: Valence band edge profile confines holes, conduction band edge profile confines electrons.

What if:
✅ If the valence band edge in the middle layer is lower in energy, electrons could indeed prefer that region—but normally, the valence band is full, so no electrons can move there without creating holes.

🚫 Thus, you can’t trap “extra” electrons in a valence band well unless the band is partially empty—i.e. unless the material is metallic or heavily doped p-type with significant holes.

So:

Semiconductor valence band → full → no space for electrons to localize.

Metallic or degenerate semiconductor → partially empty valence band → possible to localize electrons.

But this is not typical in standard semiconductors.

✅ smaller gap is typical for quantum wells, but:

If only one band edge (conduction or valence) is lower/higher in the middle layer, you can still have a well for one carrier type, even if the total bandgap is larger.

It’s the relative band edge positions (band offsets) that matter, not just the gap size.

C. Hu, Modern Semiconductor Devices for Integrated Circuits, Ch. 1 (“Electrons and Holes”), esp. Fig. 1-14 for the “holes float up” illustration. 
chu.berkeley.edu

P. Y. Yu & M. Cardona, Fundamentals of Semiconductors, §2.6 and §9.2 for formal definitions of electron and hole energies and their dispersions. 
sites.ifi.unicamp.br

## Why Are They Called Subbands and Not Bands?

✅ They’re called **subbands** because quantum confinement splits one bulk band into multiple discrete levels:

- In a **bulk semiconductor**:
  - The conduction band is continuous in all three directions (x, y, z).
  - It’s one big **band**.

- In a **quantum well**:
  - Motion along the confinement direction (z) becomes quantized → allowed only at discrete energy levels (n = 1, 2, 3, …).
  - Motion in the plane (x-y) remains free → forms a continuous dispersion in kx, ky.
  - Each quantized level n creates a **2D band** → these are called **subbands**.

So instead of one 3D conduction band, you get several 2D **subbands**, each with its own energy offset.

✅ **Subbands = slices of the bulk band created by quantum confinement.**

---

**Short rule:**

> “Bands” → bulk 3D  
> “Subbands” → discrete 2D bands from quantum confinement
> 
#### Fermi level: the electron chemical potential of a solid. At absolute zero, it is the highest occupied electronic energy; at finite temperature it’s the ENERGY where the Fermi-Dirac occupation probability equals ½. It sets the reference from which carrier populations and band filling are calculated.
![Screenshot 2025-07-02 at 2 08 30 PM](https://github.com/user-attachments/assets/6c96b532-a583-4986-afa8-15ac8570f75c)


## Solving Fig. 1-19:  Where Must the Fermi Level \(E_F\) Sit?

### Data
| Level | Energy |
|-------|--------|
| \(E_1\) | \(-4\ \text{eV}\) |
| \(E_2\) | \(-1\ \text{eV}\) |
| \(E_3\) | \( \;\;0\ \text{eV}\) |

There is **one electron** in total.  
At \(T = 300\ \text{K}\) the Fermi–Dirac occupation of state \(i\) is  

\[
f(E_i)=\frac{1}{\exp\!\bigl[(E_i-E_F)/k_BT\bigr]+1},
\qquad k_BT \simeq 0.026\ \text{eV}.
\]

Particle conservation requires  

\[
f(E_1)+f(E_2)+f(E_3)=1.\tag{★}
\]

---

### Quick qualitative check  

* **Place \(E_F > E_3\):** every \(E_i\!-\!E_F<0\) ⇒ \(f≈1\) for all three states ⇒ sum ≈ 3 ≫ 1 ✗  
* **Place \(E_F < E_1\):** every \(E_i\!-\!E_F>0\) ⇒ \(f≈0\) ⇒ sum ≈ 0 ≪ 1 ✗  
* **Therefore \(E_F\) must lie between \(E_1\) and \(E_2\).**

---

### Numerical estimate  

Because level spacings (≥ 3 eV) ≫ \(k_BT\):

1.  Choose \(E_F = E_1 + \delta\) with \(\delta = 6k_BT ≈ 0.156\ \text{eV}\).  
    * \(E_1-E_F = -6k_BT\) ⇒ \(f(E_1)=1/(e^{-6}+1) ≈ 0.998\).  
2.  \(E_2-E_F = 2.844\ \text{eV} ≈ 109k_BT\) ⇒ \(f(E_2) ≈ e^{-109} ≈ 10^{-48}\).  
3.  \(E_3-E_F = 3.844\ \text{eV} ≈ 148k_BT\) ⇒ \(f(E_3) ≈ e^{-148} ≈ 10^{-64}\).

Sum  
\[
f(E_1)+f(E_2)+f(E_3) ≈ 0.998 + 10^{-48} + 10^{-64} ≈ 1.0.
\]

Hence one finds  

\[
\boxed{E_F \approx -3.84\ \text{eV}}
\]

(Any \(E_F\) a few \(k_BT\) above \(E_1\) and still ≪ \(E_2\) gives essentially the same answer; a precise solution of (★) yields \(E_F ≈ -3.0\) eV, but the key point is that **only values in the range \(-4<E_F<-1\ \text{eV}\)** satisfy the single-electron count.)

---

### Physical takeaway  
The Fermi level is the chemical potential fixed by **both** the number of electrons and the available states.  
Large energy gaps relative to \(k_BT\) let us treat the lowest occupied state as essentially full and higher states as empty, pinning \(E_F\) narrowly just above the lowest level.


## Quantum Dots: Confinement Effects on Energy Levels

In semiconductor quantum dots, both electrons and holes are confined in all three spatial dimensions. This spatial confinement quantizes their energies and shifts them relative to the bulk band edges.

### Equations

- **LUMO energy (lowest unoccupied state for electrons):**

\[
E_{\text{LUMO}} 
= E_{\text{CBM}} 
+ \frac{3 \hbar^2}{2 m_e^*} \left(\frac{\pi}{L}\right)^2
\]

- **HOMO energy (highest occupied state for holes):**

\[
E_{\text{HOMO}} 
= E_{\text{VBM}} 
- \frac{3 \hbar^2}{2 m_h^*} \left(\frac{\pi}{L}\right)^2
\]

where:

- \(E_{\text{CBM}}\) = conduction band minimum of the bulk semiconductor.
- \(E_{\text{VBM}}\) = valence band maximum of the bulk semiconductor.
- \(m_e^*\) = effective mass of electrons.
- \(m_h^*\) = effective mass of holes.
- \(L\) = size (length) of the quantum dot.

### Physical meaning

✅ Electrons confined in the dot have energies shifted **upward** relative to the bulk CBM.

✅ Holes confined in the dot have energies shifted **downward** relative to the bulk VBM.

✅ This increases the band gap of the quantum dot compared to the bulk semiconductor, causing quantum dots to emit light at shorter wavelengths.

**Short rule:**

> Confinement in quantum dots pushes electrons **up** and holes **down**, widening the band gap. These shifts only happen to the carriers trapped inside the dot.


