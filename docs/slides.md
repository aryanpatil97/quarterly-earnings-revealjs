# Financial Formulas (Markdown slide)

We use standard valuation and risk models:

- **Present Value (PV)**: $$ PV = \frac{FV}{(1 + r)^n} $$
- **Net Present Value (NPV)**: $$ NPV = \sum_{t=0}^{T} \frac{CF_t}{(1 + r)^t} $$
- **CAPM (Expected Return)**: $$ E[R_i] = R_f + \beta_i (E[R_m] - R_f) $$

Note: Briefly explain assumptions for discount rate selection and cash-flow timing.

---

## Code Sample with Syntax Highlighting

```python
def npv(rate, cashflows):
    """Compute NPV given a discount rate and a list of cash flows.
    cashflows[0] is typically the initial investment (negative)."""
    return sum(cf / ((1 + rate) ** t) for t, cf in enumerate(cashflows))

r = 0.12  # 12% discount rate
cashflows = [-5_000_000, 1_200_000, 1_800_000, 2_200_000, 2_600_000]
print("NPV:", round(npv(r, cashflows), 2))
```

Note: Point out sign convention and sensitivity to the discount rate.

---

## Risks & Mitigations (Markdown)

<span class="fragment">FX volatility impacting overseas revenue translation.</span><br>
<span class="fragment">Interest rate risk affecting funding costs.</span><br>
<span class="fragment">Credit risk in loan book; provisions updated.</span><br>
<span class="fragment">Operational risk: cybersecurity and fraud monitoring.</span>

Note: Reveal each risk, then map it to specific mitigation steps.

---

## Next Steps & Contact

- Publish to GitHub Pages and share with stakeholders.
- Open in Speaker View with <kbd>s</kbd> to see notes.
- Email: **23f1000968@ds.study.iitm.ac.in**

Note: Close by confirming follow-ups and responsible owners.
# Contact Information

23f1000968@ds.study.iitm.ac.in

Note: This is the official email address included for the assignment check.
