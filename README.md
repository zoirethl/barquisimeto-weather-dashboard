## Barquisimeto Weather Dashboard

This repository contains a small, reproducible analysis and visualization of daily temperature records
for **Barquisimeto, Venezuela** using NASAPower data (2015–2025).

### Contents

- `data/barquisimeto_nasa_2015_2025.csv` – input dataset with columns `fecha`, `tmax_c`, `tmin_c`.
- `notebooks/BarquisimetoWeatherPatternPlot.ipynb` – Jupyter notebook that:
  - computes baseline record high/low temperatures for each day of the year (2015–2024),
  - identifies 2025 days that break those records,
  - produces a clean visualization suitable for dashboards.
- `docs/barquisimeto_temperature_records.png` – exported figure, ready to embed in a GitHub Pages dashboard.

### How to run locally

1. Create and activate a Python environment (optional but recommended).
2. Install dependencies:

```bash
pip install -r requirements.txt
```

3. Start Jupyter:

```bash
jupyter notebook
```

4. Open `notebooks/BarquisimetoWeatherPatternPlot.ipynb` and run all cells.

The notebook will read the CSV from `data/` and regenerate the figure in `docs/`.

### GitHub Pages

If you enable GitHub Pages to serve from the `docs/` folder, you can embed the PNG in an HTML/Markdown
dashboard using a relative link such as:

```markdown
![Barquisimeto temperature records](barquisimeto_temperature_records.png)
```

