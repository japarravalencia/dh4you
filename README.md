# Mitigating Digital Fatigue and the Goodhart Trap in Type 2 Diabetes Prevention (SD-DT RK4 Simulator)

[![Live Simulator](https://img.shields.io/badge/Live_RK4_Simulator-GitHub_Pages-008080?style=for-the-badge)](https://japarravalencia.github.io/dt-t2d-digital-fatigue/)
[![Zenodo DOI](https://img.shields.io/badge/Zenodo_DOI-10.5281%2Fzenodo.XXXXXXX-0f2648?style=for-the-badge)](https://doi.org/10.5281/zenodo.XXXXXXX)
[![License: CC BY 4.0](https://img.shields.io/badge/License-CC_BY_4.0-lightgrey.svg?style=for-the-badge)](https://creativecommons.org/licenses/by/4.0/)

Open Science replication package and browser-native RK4 interactive flight simulator accompanying the manuscript submitted to *Health Policy and Technology* (Elsevier):

> **Parra Valencia, J. A., Ospina, A., Ospina, D., & Suárez, F. (2026).** *Mitigating Digital Fatigue and the Goodhart Trap in Type 2 Diabetes Prevention: A System Dynamics Digital Twin Policy Assessment for Young Adults.*

## Launch & Permanent Archive
- **Interactive Web Flight Simulator (GitHub Pages):** https://japarravalencia.github.io/dt-t2d-digital-fatigue/
- **Permanent XMILE & Verification Archive (Zenodo):** https://doi.org/10.5281/zenodo.XXXXXXX

## Contents (100% Open Science, Zero Participant PII)
- `index.html` — Browser-native 4th-order Runge-Kutta (RK4, `dt = 0.25 d`, 180 days) interactive simulator featuring all 4 digital health governance levers (UUIDv4 privacy, 30-second fast-logging, JITAI alert cap, adaptive Resilience Mode), environmental stress sliders, feedback loop explorer, and CSV export.
- `Digital Twin Empoderamiento para App Nov 2026.stmx` — Native OASIS XMILE 1.0 model (Stella Architect v4.3; 6 stocks + `SMTH1`, 12 flows, 18 auxiliaries, 31 constants, zero unit warnings).
- `experimentos_dt_t2d_rk4_sobol.py` — Deterministic Python verification suite running 10 ablation & Barlas extreme-condition scenarios, Stella–Python numerical concordance (`max abs diff <= 0.00049`), 3-step RK4 convergence (`dt = 0.25 / 0.125 / 0.0625 d`), Barlas unclamped boundary & flow-integration balance (`1.33e-15`), and SALib global Sobol sensitivity (`5,120` baseline + `1,792` joint policy-space runs, 95% bootstrap CIs).
- `concordancia_stella_python.csv`, `sobol_panel_a_dt_t2d.csv`, `sobol_panel_b_politicas_dt_t2d.csv`, `corridas_csv/` — Precomputed verified synthetic outputs.

## Ethics & Data Privacy Statement
Baseline initial states were parameterized from anonymized aggregate statistics of the UNAB *Empoderamiento Saludable* cohort (`N = 153`, UNAB CIEI approval, Colombian Resolution 8430/1993 and Personal Data Protection Law 1581/2012). **Zero individual-level records or personally identifiable data are included in this repository.**


Paso 2.3 — Activar GitHub Pages

Ve a Settings → Pages dentro de dt-t2d-digital-fatigue.

En Build and deployment: Source: Deploy from a branch | Branch: main | Folder: / (root) → Save.

Espera 1–2 minutos, recarga y verifica que abra tu simulador vivo en:
https://japarravalencia.github.io/dt-t2d-digital-fatigue/

PARTE 3: Campos Exactos para Subir a Zenodo (Copiar y Pegar)

Ingresa a https://zenodo.org → botón New upload (arriba a la derecha).
