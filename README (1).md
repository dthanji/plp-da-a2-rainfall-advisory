# plp-da-a2-rainfall-advisory

## Project summary

A farmer-support NGO sends SMS planting advice in five Kenyan counties (Nairobi, Nakuru, Kisumu, Mombasa, Machakos). This project cleans a hand-typed Machakos rainfall row, then uses NumPy to calculate annual totals, monthly averages, the wettest month, dry-month counts (below 50 mm) and the best two-month planting window for each county. Results are saved to `rainfall_summary.csv`.

## Files

- `rainfall_analysis.ipynb` - the full analysis, with outputs, a "Planting Advisory" section and a "Data Quality Notes" section
- `rainfall_summary.csv` - one row per county: `county, annual_total_mm, wettest_month, dry_months, planting_window`
- `requirements.txt` - Python libraries used (`numpy`; `csv` is part of the standard library)

## How to run the notebook

1. Clone the repository and open a terminal in its folder.
2. Install the requirements: `pip install -r requirements.txt` (and `pip install notebook` if you do not have Jupyter).
3. Start Jupyter with `jupyter notebook` and open `rainfall_analysis.ipynb`.
4. Choose **Kernel > Restart & Run All**. The notebook regenerates `rainfall_summary.csv` in the same folder.

## Planting advisory

- Nairobi, Nakuru, Kisumu and Mombasa farmers should plant in April-May, when the long rains peak, and Kisumu is the most reliable county with no dry months.
- Machakos farmers should plant in November-December during the short rains, and should use water harvesting and drought-tolerant crops because the county has six months below 50 mm.
- Two Machakos readings were missing and estimated at 68 mm, so Machakos totals are approximate and everyone should confirm the rains' onset with the local forecast before sowing.
