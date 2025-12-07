Quantum Thermodynamic Neuron on a 4‑Qubit Transmon Lattice

This repo contains a Python simulation of a **4‑qubit transmon‑style lattice**
evolving under a noisy GKSL master equation with mean‑field couplings,
square‑wave bath driving, and diagnostics inspired by a **thermodynamic neuron**
 developed by Lipka‑Bartosik *et al.*,Science Advances 4 Sep 2024 Vol 10, Issue 36 https://www.science.org/doi/10.1126/sciadv.adm8792
 
 Other citations, but not limited too:

The script generates a high‑resolution animated dashboard (GIF) with:

- 4 Bloch spheres with trails and T₁/T₂/η info
- Per‑qubit phase histograms, density bars, and local Wigner functions
- A collective lattice Wigner snapshot
- Thermodynamic diagnostics (QFI, Bures length, entropy production, OTOC, Choi spectrum, etc.)
- A simple **Floquet Driven thermodynamic‑neuron logic self‑test** (NOT, NOR, 3‑MAJORITY) displayed in an HTML dashboard

## Installation

```bash
git clone https://github.com/<YOUR_USERNAME>/quantum-thermodynamic-neuron.git
cd quantum-thermodynamic-neuron

python -m venv .venv
source .venv/bin/activate    # Windows: .venv\Scripts\activate

pip install -r requirements.txt

How to ctivate a Single Mode(1 Qubit) : python quantum_unified_revised_v23.py --mode single --bath_enable --q_tmax 10.0

How to activate a Lattice Mode ( 4 interacting Qubits) : python quantum_unified_revised_v23.py --mode lattice --bath_enable --q_tmax 12.0 --fps 18



