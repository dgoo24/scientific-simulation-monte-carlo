markdown
# Numerical Simulation: Monte-Carlo-Modellierung mikroskopischer Systeme

Ein wissenschaftliches Programmierprojekt zur Simulation und statistischen Analyse mikroskopischer Systeme in der Festkörperphysik (Kondensierte Materie). Inspiriert von den Forschungsarbeiten im Condensed Matter Laboratory (LMC).

## 📊 Projektübersicht

Dieses Projekt nutzt den **Metropolis-Algorithmus (Monte-Carlo-Methode)**, um das thermische Verhalten und die Energiekonvergenz in einem zweidimensionalen Gittersystem zu simulieren. Es demonstriert die Transformation physikalischer Gesetzmäßigkeiten in hocheffizienten, numerischen Python-Code.

### Kernfeatures:
* **Stochastische Modellierung:** Implementierung von Zufallsprozessen zur Vorhersage makroskopischer Zustandskräfte aus mikroskopischen Interaktionen.
* **Algorithmen-Effizienz:** Nutzung von NumPy zur schnellen Berechnung periodischer Randbedingungen (Gitter-Topologien).
* **Statistische Datenaufbereitung:** Systematische Erfassung und statistische Filterung von Labormessdaten zur Rauschreduzierung.


## 🛠️ Technologie-Stack

* **Programmiersprache:** Python 3.12
* **Bibliotheken:** NumPy (Numerik), Matplotlib (Wissenschaftliche Visualisierung)
* **Datenaufbereitung:** MS Excel / Python-Datenstrukturen

## 🚀 Simulations-Workflow

1. **System-Initialisierung:** Generierung eines stochastischen $20 \times 20$ Gitters zur Darstellung von Teilchenzuständen.
2. **Metropolis-Kriterium:** Iterative Zustandsevaluierung basierend auf der Energieänderung $\Delta E$ und der thermodynamischen Wahrscheinlichkeit (Boltzmann-Faktor):
   $$P = e^{-\frac{\Delta E}{T}}$$
3. **Konvergenz-Analyse:** Kontinuierliche Überwachung der Systemenergie zur Bestimmung des thermodynamischen Gleichgewichts.



## 📈 Ergebnisse (Simulation Output)

Die Simulation generiert nach $50.000$ Iterationsschritten eine klare Konvergenzkurve, die den Übergang des Systems in den energetischen Grundzustand fehlerfrei dokumentiert (gespeichert als `monte_carlo_convergence.png`).



## 📂 Repository-Struktur

bash
├── monte_carlo_simulation.ipynb  # Jupyter Notebook mit dem Simulationscode
├── monte_carlo_convergence.png   # Generierte Grafik der Energiekonvergenz
└── README.md                     # Projektdokumentation (Deutsch)


## 🔧 Installation & Ausführung

1. **Abhängigkeiten installieren:**
bash
pip install numpy matplotlib

2. **Simulation starten:**
Führen Sie das Notebook `monte_carlo_simulation.ipynb` in Ihrer Jupyter-Umgebung aus.