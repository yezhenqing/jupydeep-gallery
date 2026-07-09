Generate a Jupyter Notebook script that implements a complete protein structural alignment and visualization pipeline. All required dependencies (`biopython`, `nglview`, `mdanalysis`) are pre-installed in the environment.

Pipeline Steps
1. Structure Prediction: Call the OpenFold3 model via the NVIDIA API (using env `NGC_API_KEY`) to predict the 3D structure of human ubiquitin using the following target sequence. Save the predicted structure as `ubiquitin_openfold3.pdb`.
   `MQIFVKTLTGKTITLEVEPSDTIENVKAKIQDKEGIPPDQQRLIFAGKQLEDGRTLSDYNIQKESTLHLVLRLRGG`

2. Reference Fetching: Download the experimental ubiquitin structure from the RCSB PDB database (PDB ID: `1UBQ`) to serve as the ground-truth reference, and save it as `ubiquitin_reference.pdb`.

3. Rigid Structural Alignment: Perform a rigid body alignment of the predicted OpenFold3 structure onto the reference structure (`1UBQ`) based on common C-alpha ($C_\alpha$) residues using `MDAnalysis.analysis.align`. Print out the final calculated RMSD value.

4. Interactive Visualization: Render the aligned structures using `nglview` in a cartoon representation. Ensure that the coordinates are properly translated/centered for optimal viewing. Color the OpenFold3 predicted structure red and the 1UBQ reference structure blue to highlight structural discrepancies.
