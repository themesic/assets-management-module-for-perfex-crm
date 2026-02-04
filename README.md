---
description: >-
  Complete asset management for Perfex CRM: track allocations, check-in/out,
  maintenance, depreciation, reservations, webhooks, and more.
cover: .gitbook/assets/header.png
coverY: 0
---

# 🏭 Assets Management Module for Perfex CRM

**Version 1.2.0** — The complete solution for managing your company's assets directly within Perfex CRM. Track allocations, monitor maintenance, handle depreciation, manage checkouts & reservations, and stay compliant with full audit trails.

---

## ✨ What's New in Version 1.2

| Feature | Description |
|---------|-------------|
| 📊 **Dashboard** | Real-time analytics, KPIs, and quick actions |
| 🔄 **Check-in/Check-out** | Temporary asset checkout with due dates & overdue alerts |
| 📅 **Reservations** | Calendar-based reservation system with approval workflow |
| 🚚 **Transfers** | Move assets between locations and departments |
| 📉 **Depreciation** | Dedicated depreciation tracking and schedules |
| 📈 **Reports** | Export to PDF, Excel, CSV (assets, depreciation, maintenance, audit) |
| 📥 **Import** | Bulk import assets from CSV |
| 📋 **Audit Log** | Complete activity trail for compliance |
| 🔗 **Webhooks** | Integrate with external systems (Zapier, APIs) |
| 🏷️ **Custom Fields** | Extend asset data with custom properties |
| 📁 **Project Integration** | Assign assets to projects |
| 🔔 **Smart Notifications** | Warranty expiry, maintenance due, overdue checkouts |
| 📱 **Client Portal** | Clients can view their allocated assets |

---

## 🎯 Core Features

### ✅ Complete Asset Lifecycle Management

- **Create & Track Assets** — Add assets with name, code, category, price, purchase date, warranty, depreciation
- **Upload Images** — Attach photos for easy identification
- **QR Codes & Barcodes** — Generate on demand via button in the asset view for physical verification
- **Categorize** — Use groups (subcategories), units, and locations
- **Assign to Clients** — Link assets to customers with client portal visibility

### 📋 Allocation & Revocation

- **Allocate to Staff** — Assign assets to team members with quantity tracking
- **Revoke Assets** — Return assets to inventory with full documentation
- **Real-time Availability** — Monitor allocated vs. available quantities
- **Automated Notifications** — Users notified on allocation and revocation

### 🔄 Check-in / Check-out

- **Temporary Checkouts** — Check out assets to staff or clients with expected return dates
- **Overdue Alerts** — Automated notifications when items are overdue
- **Condition Tracking** — Record condition at checkout and return
- **Quantity Support** — Check out multiple units at once

### 📅 Reservations

- **Reserve in Advance** — Book assets for future use
- **Approval Workflow** — Pending → Approved/Rejected
- **Availability Check** — Prevents double-booking
- **Calendar View** — Visual reservation overview

### 🔧 Maintenance Management

- **Schedule Maintenance** — Preventive, corrective, inspection, calibration
- **Recurring Maintenance** — Auto-schedule next maintenance after completion
- **Vendor Tracking** — Store vendor name and contact
- **Cost Tracking** — Record maintenance costs
- **Due Alerts** — Notifications 7 days before scheduled maintenance

### 📊 Financial Tracking & Depreciation

- **Depreciation Periods** — Set depreciation in months
- **Salvage Values** — End-of-life calculations
- **Book Values** — Track accumulated depreciation automatically
- **Depreciation Reports** — Export for accounting

### 📈 Reports & Analytics

- **Assets List Report** — Export all assets (PDF, Excel, CSV)
- **Depreciation Report** — Original value, depreciation, residual value
- **Maintenance Report** — Schedule and history
- **Checkout Report** — Check-in/out history
- **Audit Report** — Complete activity trail
- **Utilization Report** — Asset usage statistics

### 🔗 Webhooks & Integrations

- **20+ Events** — asset.created, asset.allocated, asset.checked_out, alerts, etc.
- **HMAC Signature** — Secure payload verification
- **Logs & Retry** — View webhook logs and retry failed calls
- **Connect to Zapier, Make, or custom APIs**

### 📋 Audit Log

- **Every Action Logged** — Created, updated, allocated, revoked, transferred, etc.
- **IP & User Agent** — Full traceability
- **Old vs. New Values** — See what changed
- **Filter by Asset** — Focus on specific assets

---

## 🧭 Quick Start Guide

### 1. 📦 Create Your First Asset

1. Go to **Assets** → **Assets** from the sidebar
2. Click **New Asset**
3. Fill in: Name, Code, Category, Quantity, Unit, Price, Purchase Date
4. Optionally add: Location, Warranty, Depreciation, Supplier, Image
5. Click **Save** — then open the asset and use the **Generate QR Code** or **Generate Barcode** button in the asset view when needed

### 2. ⚙️ Configure Settings

1. Go to **Assets** → **Settings**
2. Add **Asset Groups** (e.g., Laptops, Furniture)
3. Add **Units** (pieces, sets, meters)
4. Add **Locations** (Warehouse, Office A, etc.)

### 3. 🎯 Allocate or Check Out

- **Allocation** — Permanent assignment to staff (Assets → Allocation)
- **Check-out** — Temporary use with return date (Assets → Check-in/out)

### 4. 📊 Monitor Your Assets

- **Dashboard** — Overview of totals, overdue items, maintenance due
- **Reports** — Export data for accounting and audits

---

## 💡 Common Use Cases

| Use Case | How the Module Helps |
|----------|----------------------|
| 🖥️ **IT Equipment** | Track laptops, monitors; allocate to new hires; schedule updates |
| 🪑 **Office Furniture** | Manage desks, chairs; track assignments by department |
| 🚗 **Vehicle Fleet** | Track vehicles; schedule maintenance; monitor insurance |
| 🏭 **Manufacturing** | Schedule preventive maintenance; track utilization |
| 📱 **Mobile Devices** | Check out phones/tablets; track returns and condition |

---

## 🚀 Best Practices

- ✅ **Set up groups, units, and locations first** before creating assets
- ✅ **Use consistent naming** for assets and codes
- ✅ **Enable notifications** for warranty expiry and maintenance due
- ✅ **Generate and print QR codes/barcodes** (via button in asset view) and attach to physical assets
- ✅ **Run regular reports** for compliance and audits
- ✅ **Configure webhooks** to sync with your other tools

---

## 📚 Documentation Index

- [⚡ Requirements](getting-started/requirements.md)
- [🛠️ Activating the Module](getting-started/activating-the-module.md)
- [⚙️ Predefined Settings](predefined-settings-of-assets.md)
- [📦 Creating an Asset](how-to-use/creating-an-asset.md)
- [➕ Adding Additional Asset](how-to-use/adding-additional-asset.md)
- [🎯 Allocating Assets](how-to-use/allocating-assets.md)
- [🔄 Revoking Assets](how-to-use/asset-revocation-management.md)
- [🔄 Check-in/Check-out](how-to-use/check-in-check-out.md)
- [📅 Reservations](how-to-use/reservations.md)
- [🚚 Transfers](how-to-use/transfers.md)
- [🔧 Maintenance](how-to-use/asset-maintenance-management.md)
- [📉 Depreciation](how-to-use/depreciation.md)
- [⚠️ Reporting Broken](how-to-use/reporting-broken-assets.md)
- [🔍 Reporting Lost](how-to-use/reporting-lost-assets.md)
- [💰 Liquidation](how-to-use/asset-liquidation-management.md)
- [🛡️ Warranty](how-to-use/asset-warranty-management.md)
- [📈 Reports & Export](how-to-use/reports-and-export.md)
- [📥 Import Assets](how-to-use/import-assets.md)
- [📋 Audit Log](how-to-use/audit-log.md)
- [🔗 Webhooks](how-to-use/webhooks.md)
- [🏷️ Custom Fields](how-to-use/custom-fields.md)
- [📁 Project Integration](how-to-use/project-integration.md)
- [📊 Dashboard & Analytics](how-to-use/dashboard-and-analytics.md)

---

Need help? Contact your system administrator or refer to [Perfex CRM documentation](https://codecanyon.net/item/perfex-powerful-open-source-crm/14058437) for technical support.
