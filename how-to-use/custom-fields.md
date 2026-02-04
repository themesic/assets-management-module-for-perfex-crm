---
description: How to add and use custom fields for assets
---

# 🏷️ Custom Fields

Custom fields let you extend asset data with properties specific to your business. Add fields like "License Key", "IP Address", "Contract End Date", or any other data you need to track.

---

## 1. 📍 Access Custom Fields

**Navigation:** **Assets** → **Settings** → **Custom Fields** tab.

---

## 2. ➕ Add a Custom Field

1. Click **New Custom Field**
2. Enter **Field Name** (e.g., "Software License")
3. Select **Field Type** (see below)
4. For **Select** type: add options separated by `|` (e.g., `Active|Expired|Pending`)
5. **Applies to Groups** — Leave empty for all groups, or select specific groups
6. **Required** — Check if the field must be filled when creating/editing assets
7. **Show on Table** — Check to display in the asset list
8. **Field Order** — Control display order
9. Click **Save**

---

## 3. 📋 Field Types

| Type | Description | Example |
|------|-------------|---------|
| **Text** | Single-line text | License key, serial number |
| **Textarea** | Multi-line text | Notes, specifications |
| **Number** | Numeric value | Capacity, version |
| **Date** | Date picker | Contract end, renewal date |
| **Select** | Dropdown | Status, priority |
| **Checkbox** | Yes/No | Is insured, requires calibration |
| **URL** | Web link | Manual, support page |

---

## 4. 🎯 Applies to Groups

- **Empty** — Field appears for all assets
- **Specific groups** — Field appears only for assets in selected groups

Example: Add "RAM (GB)" only to the "Laptops" group.

---

## 5. 📊 Using Custom Fields

### When Creating/Editing an Asset

- Custom fields appear in the form based on the asset's group
- Required fields must be filled before saving
- Values are stored per asset

### In Reports

- Fields with **Show on Table** appear in the asset list
- Export reports may include custom field values (depending on implementation)

---

## 💡 Best Practices

- ✅ **Use clear names** — "Software License Key" not "slk"
- ✅ **Limit options for Select** — Keep dropdowns manageable
- ✅ **Use groups** — Apply fields only where relevant
- ✅ **Show on table** for fields you filter or sort by often
