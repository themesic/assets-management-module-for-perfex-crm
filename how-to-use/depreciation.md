---
description: How to manage asset depreciation and view depreciation reports
---

# 📉 Asset Depreciation Management

The Assets module tracks depreciation for accounting and financial reporting. Set depreciation periods when creating assets, and use the **Depreciation** section to view schedules and export reports.

---

## 1. 📍 Access Depreciation

**Navigation:** **Assets** → **Depreciation** from the sidebar.

---

## 2. ⚙️ Setting Depreciation on Assets

When creating or editing an asset, configure:

| Field | Description |
|-------|-------------|
| **Depreciation (Months)** | Number of months over which the asset depreciates (e.g., 36 for 3 years) |
| **Unit Price** | Purchase price per unit |
| **Purchase Date** | Start date for depreciation calculation |
| **Salvage Value** | Optional — expected value at end of life |

**Formula (straight-line):**

```
Monthly Depreciation = (Total Value - Salvage Value) / Depreciation Months
Depreciation to Date = Monthly Depreciation × Months Since Purchase
Residual/Book Value = Total Value - Depreciation to Date
```

---

## 3. 📊 Depreciation Dashboard

The **Depreciation** page typically shows:

- **Original Value** — Total purchase value of assets
- **Total Depreciation** — Accumulated depreciation to date
- **Current Book Value** — Original minus depreciation
- **Depreciation Schedule** — Per-asset breakdown

---

## 4. 📈 Depreciation Report

1. Go to **Assets** → **Reports**
2. Select **Depreciation Report**
3. Apply filters (group, location, status)
4. Choose format: **PDF**, **Excel**, or **CSV**
5. Click **Generate Report**

### Report Contents

- Asset code and name
- Purchase date
- Original value
- Depreciation period (months)
- Months used
- Depreciation value to date
- Residual value
- Depreciation percentage

---

## 5. 📋 Depreciation Schedule Table

In **Assets** → **Depreciation** you may see a table with:

- Asset details
- Opening value
- Depreciation amount
- Closing value
- Period (e.g., monthly or yearly)

---

## 💡 Best Practices

- ✅ **Set depreciation** when creating assets for accurate reporting
- ✅ **Use consistent periods** (e.g., 36 months for IT equipment)
- ✅ **Export reports** for accounting and tax filing
- ✅ **Review fully depreciated assets** for disposal decisions
