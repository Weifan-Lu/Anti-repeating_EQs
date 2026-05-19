# Anti-Repeating Earthquake Dataset – README

This dataset contains information on **anti‑repeating earthquakes** (also known as waveform‑inverse repeating earthquakes) detected in the NN seismic network. The data are organized into two CSV files and one PDF document that illustrates the most significant earthquake families.

## Files

| File | Description |
|------|-------------|
| `NV_anti_repeating_qs_catalog.csv` | List of all 37 anti‑repeating earthquakes. |
| `NV_anti_repeating_eqs_pairs.csv` | List of the 42 anti‑repeating earthquake pairs, including the stations that recorded each pair. |
| `families.pdf` | A PDF figure showing the most significant anti‑repeating families. |

---

## File Formats

### 1. `NV_anti_repeating_qs_catalog.csv`

- **Rows:** 37 earthquakes, each identified by a unique sequential number.
- **Columns:**
  - **Column 1:** Event index (1‑based, corresponding to descriptions in the PDF file).
  - **Columns 2+:** Descriptive information for each event (e.g., origin time, location, magnitude).

> The event index in the first column links this file to the pairs file and to the families illustrated in `family.pdf`.

### 2. `NV_anti_repeating_eqs_pairs.csv`

- **Rows:** 42 pairs of earthquakes that exhibit anti‑repeating behaviour (waveforms are opposite in polarity).
- **Columns:**
  - Each row contains the two event indices that form an anti‑repeating pair.
  - **`station`** lists the seismic station(s) of the **NN** network that recorded this pair. Multiple stations may be listed per row.

> All data come from the **NN** seismic network.

---

## Significant Families (from `families.pdf`)

The PDF file highlights the most prominent families of anti‑repeating earthquakes. A **family** is defined as a group of events where every member shows waveform inversion with respect to a reference event or with other members.

Examples given in `families.pdf`:

- **Family (a)** – centred on **event 8**  
  *Waveform‑inverse relationships:*  
  Event 8  ↔  events 7, 9, 10, 17

- **Family (c)** – centred on **event 19**  
  *Waveform‑inverse relationships:*  
  Event 19  ↔  events 12, 18, 16, 9, 10, 20

These examples illustrate how families are defined. Additional families can be identified by analysing the full pair list and the earthquake descriptions.


---

## Contact / Citation

If you use this dataset, please cite the original data source (as described in the accompanying publication or metadata). For questions, refer to the authors of the dataset.

*Last updated: 2026‑05‑19*
