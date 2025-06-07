# Fundamentals of Solid State 🧱

This is your go-to resource for exploring the world of materials science, starting from the fundamentals. This repository provides interactive tools to master key concepts using Mathematica. Feel free to download and interact/modify it. 🚀

## Repository Purpose 🌟

- **Educational Materials**: Clear explanations of foundational Solid State and DFT concepts, like Bloch's Theorem.
- **Practical Examples**: Input files, output analyses, and visualizations.
- **Interactive Tools**: Mathematica notebooks to explore key concepts and develop an intuitive understanding of electronic properties.

## Repository Contents 📂

### 1. Foundational Concepts 📚

*The band structure is fixed by the crystal, but the electronic properties depend on how electrons fill it.*

- **Bloch's Theorem 🌊**:
  - Explains why electrons in periodic crystals form wavefunctions with a plane-wave component modulated by a periodic function.
  - Includes notes and an interactive notebook.
 
- **The Kronig-Penney Model  (Repulsive) ⚙️**:
  - The Kronig-Penney model is a one-dimensional model of a crystal formed by an infinite arrangement of delta function potentials (here, the repulsive case).
  - This model does not produce bound states; therefore is not appropriate for illustrating atomic-like systems.
  - In the provided Mathematica notebook, you’ll find a solution to this problem, which is a typical quantum mechanics problem.
  - The notebook also illustrates the relationship between crystal momentum and electron energy.
  - Manipulating the plot will also demonstrate how bands and band gaps are formed and what happens when the potential is increased.

 - **The Kronig-Penney Model (Attractive) 🎯**:
    - This simulation demonstrates why energy bands form and how degeneracy is lifted as we modify the a/ℓ ratio.
    - Key for introducing the Tight Binding Model.
    - In the attractive case, the degeneracy of the single well's bound state is lifted as the wells are brought closer, and a band forms.
    - In the repulsive case, the band structure is the result of scattering interference and the crystal’s periodicity, not from splitting a degenerate level, but from allowing certain energies due to constructive interference (Bloch's theorem).
    
- **Electrons Interacting with a Periodic Potential🫆**:
  - Band formation: You see how energy bands emerge from free electron states when a periodic potential is added.
  - Band gaps: The model shows how energy gaps naturally appear at the edges of the Brillouin zone due to Bragg scattering.
  - Fourier thinking: You learn to represent both wavefunctions and potentials in terms of plane waves, which is key for understanding crystal momentum and reciprocal space.
  - Perturbative intuition: It helps build intuition for how small perturbations (like a weak lattice potential) can cause significant changes in energy spectra.
  - Numerical skills: You practice constructing and solving matrix eigenvalue problems, which is essential in computational physics.

- **Including More G Vectors 🤖**:
  -  Observe the impact of increasing the number of plane wave components when calculating a band structure in this Manipulate plot using the code for electrons interacting with a periodic potential.
  -  Additionally, observe the effects of increasing the potential.
 
- **The Nearly-Free Electron Model 🫧**:
  - Explain the Nearly-Free Electron Model and its application of the degenerate perturbation model.
  - Explain why the Fourier transform is important in this context.
  - Demonstrate how inner products are used in the process, ultimately leading to a nice quantum mechanics problem.
  - How can we eliminate degeneracy in the band edge of a free electron model that has been slightly perturbed?





📚*Cohen, M. L., & Louie, S. G. (2016). Fundamentals of condensed matter physics. Cambridge University Press.*



  
