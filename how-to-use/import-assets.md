---
description: How to bulk import assets from CSV in the Asset Management module
---

# 📥 Import Assets

Import multiple assets at once using a CSV file. The import feature creates groups, units, and locations automatically if they don't exist.

---

## 1. 📍 Access Import

**Navigation:** **Assets** → **Import** from the sidebar.

---

## 2. 📋 Import Steps

### Step 1: Download Template

1. Click **Download Template**
2. Open the CSV in Excel or a text editor
3. The template includes column headers and example rows

### Step 2: Fill in Your Data

Add one row per asset. Use the columns described below.

### Step 3: Upload

1. Click **Select CSV File**
2. Choose your completed CSV file
3. Click **Import** or **Upload**
4. Review the import summary (imported count, failed count, errors)

---

## 3. 📝 Expected Columns

| Column | Description | Required |
|--------|-------------|----------|
| `asset_code` or `code` | Unique code. Auto-generated if empty | No |
| `asset_name` or `name` | Asset name | Yes |
| `quantity` or `amount` | Quantity. Default: 1 | No |
| `unit` | Unit name (e.g., Pieces). Created if not exists | No |
| `group` or `category` | Asset group. Created if not exists | No |
| `location` | Location. Created if not exists | No |
| `purchase_date` or `date_buy` | YYYY-MM-DD format | No |
| `warranty_months` or `warranty_period` | Warranty in months | No |
| `price` or `unit_price` | Unit price | No |
| `depreciation_months` or `depreciation` | Depreciation period in months | No |
| `supplier` or `supplier_name` | Supplier name | No |
| `description` | Asset description | No |
| `manufacturer` | Manufacturer | No |
| `model` or `model_number` | Model number | No |
| `serial` or `series` | Serial number | No |

---

## 4. 📄 CSV Format Tips

- **Encoding:** UTF-8 (with BOM for Excel compatibility)
- **Separator:** Comma (`,`)
- **Headers:** First row must contain column names
- **Dates:** Use `YYYY-MM-DD` (e.g., 2025-01-15)
- **Empty values:** Leave cell empty; defaults will apply

---

## 5. ✅ After Import

- **Imported count** — Number of assets successfully added
- **Failed count** — Rows that could not be imported
- **Errors** — List of errors (e.g., "Row 5: Missing asset name")

Fix errors in your CSV and re-import failed rows if needed.

---

## 6. 📊 Import History

The module stores import history:

- Filename
- Total rows, imported, failed
- Who imported, when
- Error details

Check **Settings** or **Import History** (if available) to review past imports.

---

## 💡 Best Practices

- ✅ **Test with a small file** first (5–10 rows)
- ✅ **Match column names** exactly to the expected format
- ✅ **Use consistent group/unit/location names** for proper categorization
- ✅ **Backup before large imports** — import cannot be easily undone
