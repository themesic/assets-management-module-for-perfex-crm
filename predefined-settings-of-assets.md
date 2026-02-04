---
description: >-
  Configure asset groups, units, locations, custom fields, webhooks, and
  notifications for the Assets Management Module.
icon: gear-complex
---

# ⚙️ Predefined Settings of Assets

The **Assets Settings** section lets you configure the foundational elements of your asset management system. Set these up before creating assets for the best experience.

---

## 1. 🗂️ Accessing Assets Settings

**Navigation:** Go to **Assets** → **Settings** from the sidebar menu.

The Settings page includes tabs for:

- **Asset Groups** (Categories/Subcategories)
- **Asset Units** (Units of measurement)
- **Asset Locations** (Storage/usage locations)
- **Custom Fields** (Extend asset data)
- **Webhooks** (External integrations)
- **Notifications** (Alert preferences)

---

## 2. 📁 Asset Groups

Asset groups are your main categories (e.g., IT Equipment, Furniture, Vehicles).

### Add a Group

1. Go to **Asset Groups** tab
2. Click **New Asset Group**
3. Enter **Group Name** (e.g., "Laptops", "Office Furniture")
4. Click **Save**

### Use Cases

- Filter assets by category
- Run reports by group
- Apply custom fields to specific groups
- Organize depreciation by asset type

---

## 3. 📏 Asset Units

Units define how you measure quantity (pieces, sets, meters, etc.).

### Add a Unit

1. Go to **Asset Units** tab
2. Click **New Asset Unit**
3. Enter **Unit Name** (e.g., "Pieces", "Sets", "Meters", "Boxes")
4. Click **Save**

### Examples

| Unit | Use Case |
|------|----------|
| Pieces | Laptops, monitors, chairs |
| Sets | Desk + chair combos |
| Meters | Cables, fabric |
| Boxes | Consumables, spare parts |

---

## 4. 📍 Asset Locations

Locations are physical places where assets are stored or used.

### Add a Location

1. Go to **Asset Locations** tab
2. Click **New Asset Location**
3. Enter **Location** (e.g., "Warehouse A", "Office Floor 2", "Remote")
4. Click **Save**

### Use Cases

- Track where assets are stored
- Use in transfers (from/to location)
- Filter assets by location
- Support multi-site organizations

---

## 5. 🏷️ Custom Fields

Add custom fields to capture data specific to your business.

### Field Types

| Type | Description |
|------|-------------|
| Text | Single-line text |
| Textarea | Multi-line text |
| Number | Numeric value |
| Date | Date picker |
| Select | Dropdown (options separated by \|) |
| Checkbox | Yes/No |
| URL | Web link |

### Add a Custom Field

1. Go to **Custom Fields** tab
2. Click **New Custom Field**
3. Enter **Field Name**
4. Select **Field Type**
5. For Select: add options like `Option1|Option2|Option3`
6. Optionally: **Applies to Groups** — leave empty for all, or select specific groups
7. **Required** — Check if the field must be filled
8. **Show on Table** — Check to display in asset list
9. Click **Save**

---

## 6. 🔗 Webhooks

Configure webhooks to send asset events to external systems (Zapier, Make, custom APIs).

### Add a Webhook

1. Go to **Webhooks** tab
2. Click **New Webhook**
3. Enter **Webhook Name** (e.g., "Sync to Inventory System")
4. Enter **Webhook URL** (your endpoint)
5. Select **Events** to subscribe to (or select all)
6. Optionally set **Secret Key** for HMAC signature verification
7. Click **Save**
8. Use **Test Webhook** to verify it works

### Available Events

- `asset.created`, `asset.updated`, `asset.deleted`
- `asset.allocated`, `asset.revoked`
- `asset.checked_out`, `asset.checked_in`
- `asset.reserved`, `asset.reservation_approved`, `asset.reservation_rejected`
- `asset.maintenance_scheduled`, `asset.maintenance_completed`
- `asset.transferred`, `asset.lost`, `asset.broken`, `asset.warranty`, `asset.liquidated`
- `alert.warranty_expiring`, `alert.maintenance_due`, `alert.checkout_overdue`, `alert.low_stock`

---

## 7. 🔔 Notifications

Configure when and how you receive alerts.

### Notification Types

| Type | Default | Description |
|------|---------|-------------|
| Warranty Expiry | 30 days before | Asset warranty ending soon |
| Insurance Expiry | 30 days before | Insurance policy ending |
| Maintenance Due | 7 days before | Scheduled maintenance upcoming |
| Checkout Overdue | 1 day after | Checked-out asset not returned |
| Reservation Reminder | 1 day before | Upcoming reservation |
| Low Stock | When threshold met | Asset quantity below minimum |
| Asset End of Life | 30 days before | Expected end-of-life date |

### Configure Notifications

1. Go to **Notifications** tab
2. For each type: enable/disable, set **Days Before**, choose **Recipients**
3. If no recipients selected, admins receive notifications
4. Click **Save**

### ⚠️ Cron Job Required

Notifications are sent via Perfex CRM's cron job. Ensure your cron is set up:

```
* * * * * php /path/to/perfex/index.php cron/index
```

---

## 📋 Best Practices

- ✅ **Set up groups, units, and locations first** before creating assets
- ✅ **Use consistent naming** across your organization
- ✅ **Create custom fields** for data you need in reports
- ✅ **Test webhooks** before going live
- ✅ **Configure notifications** so nothing falls through the cracks
