# StateStub Open Data (2026)

Open CSV datasets indexing 2026 US state income tax withholding rules, mandatory employee payroll contributions, and a standardized $75,000 take-home pay ranking across 26 verified US states using official IRS Publication 15-T and state Department of Revenue withholding guides.

Every figure is computed directly from 2026 IRS federal withholding schedules, statutory FICA rates (6.2% Social Security + 1.45% Medicare), and primary state withholding tables verified in November 2026. Interactive paycheck, hourly, bonus, and state comparison calculators live at [statestub.com](https://statestub.com/).

## Datasets in this repository

| File | Coverage | Live report & calculator |
|---|---|---|
| [`data/state-income-tax-2026.csv`](data/state-income-tax-2026.csv) | 26 verified US states: tax structure (none / flat / graduated), 2026 rates, mandatory employee payroll taxes (SDI, PFML, SUI), local tax note, effective date, and official state DOR primary source URL | [US State Income Tax 2026 Report](https://statestub.com/reports/state-income-tax-2026/) / [Paycheck Calculator](https://statestub.com/) |
| [`data/take-home-pay-by-state-2026.csv`](data/take-home-pay-by-state-2026.csv) | 26-state take-home pay ranking on a **$75,000** single salary (2026 W-4): federal income tax, Social Security, Medicare, state income tax, mandatory state payroll contributions, annual net pay, and biweekly paycheck | [Take-Home Pay by State Report](https://statestub.com/reports/take-home-pay-by-state-2026/) / [Compare States Calculator](https://statestub.com/compare-states/) |

---

## 1. 2026 Take-Home Pay on a $75,000 Salary Across 26 States

All 26 states share the same federal baseline on a $75,000 single salary (`$7,670.00` federal income tax, `$4,650.00` Social Security, `$1,087.50` Medicare). State income tax and mandatory employee payroll contributions create a **$4,195.36/year** (**$161.36/biweekly**) gap between the top and bottom of the 26-state ranking:

| Rank | State | State income tax | Mandatory state payroll | Annual take-home | Biweekly paycheck |
|---:|---|---:|---:|---:|---:|
| 1 (tie) | FL, NV, NH, SD, TN, TX, WY | $0.00 | $0.00 | **$61,592.50** | **$2,368.94** |
| 24 | South Carolina (SC) | $3,843.84 | $0.00 | $57,748.66 | $2,221.10 |
| 25 | Massachusetts (MA) | $3,649.88 | $345.00 (PFML) | $57,597.62 | $2,215.29 |
| 26 | California (CA) | $3,220.36 | $975.00 (1.3% SDI) | **$57,397.14** | **$2,207.58** |

---

## 2. State Withholding & Mandatory Payroll Coverage

[`data/state-income-tax-2026.csv`](data/state-income-tax-2026.csv) documents:
- **9 no-wage-income-tax states:** AK (with 0.50% employee UI up to $54,200), FL, NV, NH, SD, TN, TX, WA (with PFML + WA Cares Fund), WY.
- **17 income-tax states:** CA, GA, IA, IL, IN, KY, MA, MO, NC, NJ, NY, OH, PA, SC, UT, VA, WI — including mandatory state disability/paid-leave deductions where applicable (CA 1.3% SDI, MA 0.46% PFML, NJ SUI/SDI/FLI, NY PFL + DBL, PA SUI).

---

## Primary Official Sources

- IRS: [Publication 15-T (Federal Income Tax Withholding Methods)](https://www.irs.gov/pub/irs-pdf/p15t.pdf), [Publication 15 (Circular E)](https://www.irs.gov/pub/irs-pdf/p15.pdf), [Form W-4](https://www.irs.gov/pub/irs-pdf/fw4.pdf)
- State agencies (all 26 links listed row-by-row inside `data/state-income-tax-2026.csv`), including California EDD Method B, NY NYS-50-T-NYS, Massachusetts Circular M, Illinois IL-700-T, Pennsylvania REV-415, and Ohio Employer Withholding Tables.

## Interactive Calculators and Embeds

- US Paycheck Calculator (26 states): https://statestub.com/
- Hourly Paycheck Calculator: https://statestub.com/hourly-paycheck-calculator/
- Compare Take-Home Pay Across Two States: https://statestub.com/compare-states/
- Bonus Tax & Raise Calculators: https://statestub.com/bonus-tax-calculator/ · https://statestub.com/raise-calculator/
- Federal Withholding Calculator (IRS Pub 15-T): https://statestub.com/federal-withholding-calculator/
- Lightweight iframe embeds: `https://statestub.com/embed/paycheck/`, `https://statestub.com/embed/hourly/`

## License and Citation

Licensed under [CC-BY-4.0](LICENSE). Citation metadata is in [`CITATION.cff`](CITATION.cff).

```text
StateStub (2026). StateStub Open Data 2026: US State Income Tax Withholding Rules and $75,000 Take-Home Pay Ranking Across 26 States [Dataset]. https://statestub.com/reports/ (CC-BY-4.0).
```
