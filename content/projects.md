---
title: 'Projects'
date: 2024-05-19
type: landing

design:
  # Section spacing
  spacing: '5rem'

# Page sections
sections:
  - block: markdown
    id: section-1
    content:
      title: Prior Potentials for Stable Molecular Dynamics Simulations with Machine Learning Force Fields
      subtitle: Masters thesis at the Chair for Multiscale Modeling of Fluid Materials - Prof. Julija Zavadlav - 6 mo.
      text: |
        Top-down training of ML potentials requires running MD simulations during training. The observables from the simulation can then be compared with experimental values. Based on this, the potential parameters can be updated effectively without backpropagating through the trajectory by differentiable trajectory reweighing. However, untrained ML potentials can cause MD simulations to destabilize. In my master's thesis, I developed Delta-Learning methods for combining the stability of empirical force fields and the accuracy of ML interatomic potentials. From a statistical perspective, this Delta Learning approach can be understood as placing a prior (the classical force field) on the phase space distribution. Further, I reviewed different measures of stability of MD simulations and investigated parameters that influence the quality of both the classical and ML potentials - e.g., the functional form of the prior. The project was developed with JAX, JAX MD, and the chemtrain library.
  - block: markdown
    id: section-2
    content:
      title: Active Learning of Equivariant Graph Neural Network Potentials for Metal-Organic Frameworks
      subtitle: Research Internship at the Chair for Simulation of Nanosystems for Energy Conversion - Prof. Alessio Gagliardi - 2mo.
      text: |
        Creating a balanced ML potential training dataset that covers relevant portions of the configuration space can be difficult. This problem arises from the curse of dimensionality of phase space. One approach to tackling dataset creation is active learning. In this project, I implemented an active learning workflow for training a NequIP potential for the metal-organic framework UiO-66. The workflow consisted of iteratively training the MLIP, running metadynamics simulation to sample the configuration space along a collective variable (in this case, the volume of the MOF cell), and subsequently computing forces and potential energies with DFT calculations, thereby expanding the training dataset with new structures. The workflow was set up using the NequIP, LAMMPS+PLUMED for MD, CP2K for DFT, SLURM for HPC management, Python, and BASH for setting up config files and "scripting glue". 
  - block: markdown
    id: section-3
    content:
      title: Application of Nickel-containing Inks in the Binder Jet 3D-Printing of Ni/Al2O3 Catalysts for CO2 Methanation
      subtitle: Bachelors Thesis at the Chair of Technical Chemistry 1 - Prof. Kai-Olaf Hinrichsen - 3 mo.
      text: |
        Many essential industrial processes depend on catalysis. Optimization of catalysts and reactors can be complicated due to the manufacturing constraints of the catalyst pellets. Additive manufacturing offers the capability to produce (almost) any desired shape and could, therefore, be used for optimizing catalyst pellet geometries and, thereby, the chemical reactions. In my bachelor's thesis, I used a 3D-printing manufacturing process (binder jetting) of alumina-supported nickel catalysts for CO2 reduction. The laboratory work in the experimental group of the Chair for Technical Chemistry 1 contained a wide range of mechanical, physical, and chemical characterization - Crushing strength tests, porosometry, N2 physisorption, powder XRD, UV/VIS Spectroscopy, TEM, XPS.
  - block: markdown
    id: section-4
    content:
      title: Sintering with Concentrated Sunlight On Regolith for Constructing Lunar Habitats (SCORCH)
      subtitle: Internship at the European Space Agency - European Astronaut Centre, Cologne - Dr. Aidan Cowley - 6 mo.
      text: |
        A permanent presence of astronauts on the moon requires protection from radiation and micrometeorites. Shipping all construction materials for habitats from the Earth is expensive; the costs increase the barrier to continued lunar exploration. Utilizing local lunar resources such as sunlight and moondust (regolith) can reduce these costs. I built a 3D printer for powder bed fusion with concentrated sunlight during my internship. I took on the tasks of mechanical and electrical design, manufacturing, assembly, implementation of sensor and actuator software, process modeling with FEM, and creating documentation and experimental procedures.  - block: markdown
    id: section-5
    content:
      title: Materials Science Databases x Large Language Models
      subtitle: Presentation for Seminar "Theory and Practice of Datamanagement in Chemistry" - Prof. Helge Stein - 2 d.
      text: |
        I gave a presentation on interfacing materials science databases, data management, and large language models, which can be found here: https://github.com/steffen-wedig/ec-llm.
        As a short example, I hacked together a small streamlit applet that uses retrieval augmented generation (RAG) on the BattINFO ontology to find correct concepts of the ontology - which might be useful for tagging lab documents. Used LlamaIndex and Streamlit.

---

