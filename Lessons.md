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
