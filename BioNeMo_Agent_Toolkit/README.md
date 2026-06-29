# BioNeMo Agent Toolkit 🚀

While general AI agents often struggle with complex biomolecular workflows due to a lack of domain-specific grounding, NVIDIA BioNeMo bridges this gap. By packaging advanced digital-biology models into robust, agent-ready "Skills," it brings deterministic engineering to structural biology and chemistry. 

Recently, NVIDIA open-sourced the [BioNeMo Agent Toolkit](https://github.com/NVIDIA-BioNeMo/bionemo-agent-toolkit)—a specialized suite designed to accelerate drug discovery and protein design. Below, we demonstrate how **JupyDeep** seamlessly orchestrates these skills to supercharge your interactive research workflows.

---

## 🛠️ Framework Setup & Skill Acquisition

First, we initialize the environment and fetch the official BioNeMo skills:

```bash
mkdir -p ·/skills
cd ./skills
git clone https://github.com/NVIDIA-BioNeMo/bionemo-agent-toolkit.git
```

## 🔬 Hands-on Skill Demonstration
We walk through a practical workflow showcasing a few high-impact skills integrated directly into JupyDeep's agentic workspace:

1. genmol-nim

The genmol-nim skill unleashes a local- or cloud-deployable microservice that leverages SAFE notation (instead of traditional SMILES) to power de novo drug design, lead optimization, and property ranking (e.g., QED and LogP) via Docker or NVIDIA APIs.

Please refer to prompt.md for the agent instructions. We adapted these guidelines from evals.json and enhanced them with JupyDeep-specific context—particularly around RDKit visualization.

2. openfold3-nim

The openfold3-nim skill leverages NVIDIA’s BioNeMo NIM microservice to predict complex biomolecular structures—including protein-ligand, protein-nucleic acid, and multi-chain complexes—via local Docker or hosted NVIDIA APIs.


