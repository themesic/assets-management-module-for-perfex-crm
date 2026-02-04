---
description: How to report broken or damaged assets in the Asset Management module
---

# ⚠️ Reporting Broken Assets

When an asset is damaged or broken (but not lost), use the **Report Broken** feature to document the incident, track repair status, and maintain accurate inventory counts.

---

## 1. 🚨 When to Report Broken

- Asset is damaged and unusable
- Equipment has malfunctioned
- Physical defect discovered
- Asset needs repair (not yet sent for warranty)

**Note:** Broken assets remain in your total count but are tracked separately. Use **Warranty** when sending for repair under warranty.

---

## 2. 📍 Access the Feature

**From Asset List:**
1. Go to **Assets** → **Assets**
2. Click on the asset
3. Use the **Broken** or **Report Broken** action

**From Asset Detail:**
- Open the asset and find the **Report Broken** button in the actions menu

---

## 3. 📝 Fill in Broken Report Details

### Required Information

| Field | Description |
|-------|-------------|
| **Broken Code** | Auto-generated (e.g., BRK-00000001) — editable if needed |
| **Quantity** | Number of units that are broken |
| **Broken Time** | Date and time of the incident or discovery |

### Optional Information

| Field | Description |
|-------|-------------|
| **Description** | What happened, extent of damage, location, etc. |

### Reference

- **Remaining Quantity** — Shows current available vs. total (read-only)

---

## 4. ✅ Save the Report

Click **Save**. The system will:

- ✅ Generate a unique broken report code
- ✅ Update `total_damages` for the asset
- ✅ Record the event in inventory history
- ✅ Log the action in the audit log
- ✅ Trigger webhook `asset.broken` (if configured)
- ❌ **Does NOT** reduce total quantity — broken items stay in inventory until liquidated or repaired

---

## 5. 🔄 What Happens Next

- **Broken count** is tracked separately from available quantity
- You can send the asset for **Warranty** repair (reduces broken count when processed)
- Use **Liquidation** if the asset is disposed of
- **Reports** will show broken vs. available vs. allocated

---

## 💡 Best Practices

- 📸 **Document damage** — Add photos as attachments if possible
- 📋 **Describe clearly** — Help future audits and insurance claims
- 🔗 **Link to warranty** — If under warranty, use the Warranty feature next
- 📊 **Review regularly** — Run reports to see broken asset trends
