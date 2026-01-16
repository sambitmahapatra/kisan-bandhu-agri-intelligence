# kisan-bandhu-agri-intelligence

Key columns include:
- `date`
- `actual_price`
- `expected_price`
- `p10_price`, `p50_price`, `p90_price`
- `residual`
- `residual_z`
- `rolling_vol`

This file is treated as **read-only** by V2.

---

## Performance Summary (Indicative)

Walk-forward results over 2018–2025:

- MAE ≈ ₹130  
- RMSE ≈ ₹320  
- MAPE ≈ 4.5%  
- R² ≈ 0.90  

Uncertainty band coverage:
- P10–P90 ≈ 80–85% (intentionally calibrated)

These metrics indicate a **stable, non-overfit baseline**.

---

## Known Limitations (Explicit)

V1 cannot:
- explain price spikes or crashes  
- detect market regimes  
- incorporate weather, supply, or policy signals  
- provide farmer advisories  

These are **not bugs** — they motivate V2.

---

## Role of V1 in V2

V1 acts as a **counterfactual anchor**:

> “What price would we expect if the market were behaving normally?”

V2 builds on this to:
- detect abnormal regimes  
- attribute plausible causes  
- generate farmer-safe advisories  

Once frozen, V1 is **never modified**.

---

## Repository Structure (Suggested)


