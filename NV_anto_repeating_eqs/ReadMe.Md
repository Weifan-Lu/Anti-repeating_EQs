# Anti-Repeating Earthquake Dataset – README

This dataset contains information on **anti‑repeating earthquakes** (also known as waveform‑inverse repeating earthquakes) detected in the NN seismic network. The data are organized into two CSV files and one PDF document that illustrates the most significant earthquake families.

## Files

| File | Description |
|------|-------------|
| `anti_repeating_earthquakes.csv` | List of all 37 anti‑repeating earthquakes. |
| `anti_repeating_pairs.csv` | List of the 42 anti‑repeating earthquake pairs, including the stations that recorded each pair. |
| `family.pdf` | A PDF figure showing the most significant anti‑repeating families, with examples of waveform‑inverse relationships. |

---

## File Formats

### 1. `anti_repeating_earthquakes.csv`

- **Rows:** 37 earthquakes, each identified by a unique sequential number.
- **Columns:**
  - **Column 1:** Event index (1‑based, corresponding to descriptions in the PDF and pairs file).
  - **Columns 2+:** Descriptive information for each event (e.g., origin time, magnitude, location – exact fields depend on the original data).

> The event index in the first column links this file to the pairs file and to the families illustrated in `family.pdf`.

### 2. `anti_repeating_pairs.csv`

- **Rows:** 42 pairs of earthquakes that exhibit anti‑repeating behaviour (waveforms are opposite in polarity).
- **Columns:**
  - Each row contains the two event indices that form an anti‑repeating pair.
  - An additional column named **`station`** lists the seismic station(s) of the NN network that recorded this pair. Multiple stations may be listed per row.

> All data come from the **NN** seismic network.

---

## Significant Families (from `family.pdf`)

The PDF file highlights the most prominent families of anti‑repeating earthquakes. A **family** is defined as a group of events where every member shows waveform inversion with respect to a reference event or with other members.

Examples given in `family.pdf`:

- **Family 1** – centred on **event 8**  
  *Waveform‑inverse relationships:*  
  Event 8  ↔  events 7, 9, 10, 17

- **Family 2** – centred on **event 19**  
  *Waveform‑inverse relationships:*  
  Event 19  ↔  events 12, 18, 16, 9, 10, 20

These examples illustrate how families are defined. Additional families can be identified by analysing the full pair list and the earthquake descriptions.

---

## How to Use the Data

1. **Load the CSV files** into your preferred analysis environment (Python, MATLAB, R, etc.).
2. **Match event indices** between the two CSV files to obtain full descriptive information for each pair.
3. **Consult `family.pdf`** to understand the manually identified significant families.
4. **Use the station information** to explore the spatial distribution and network response for each anti‑repeating pair.

---

## Notes

- An **anti‑repeating earthquake** is characterised by a waveform that is the inverse (opposite polarity) of another earthquake at the same station(s), usually indicating a similar source mechanism but reversed slip direction.
- The total number of individual anti‑repeating events is **37**.  
  The total number of confirmed pairs (mutual inverse relationships) is **42**.
- All data are from the **NN** seismic network. Station codes are provided as they appear in the original recordings.

---

## Contact / Citation

If you use this dataset, please cite the original data source (as described in the accompanying publication or metadata). For questions, refer to the authors of the dataset.

*Last updated: 2026‑05‑19*
