---
description: How to configure webhooks to integrate the Assets module with external systems
---

# 🔗 Webhooks

Webhooks send real-time notifications to your external systems when asset events occur. Use them with Zapier, Make, custom APIs, or inventory systems.

---

## 1. 📍 Access Webhooks

**Navigation:** **Assets** → **Settings** → **Webhooks** tab.

---

## 2. ➕ Create a Webhook

1. Click **New Webhook**
2. Enter **Webhook Name** (e.g., "Sync to ERP")
3. Enter **Webhook URL** — your endpoint (must accept POST requests)
4. Select **Events** to subscribe to (or select all)
5. Optionally set **Secret Key** for HMAC signature verification
6. Optionally add **Custom Headers** (e.g., API key)
7. Set **Active** to Yes
8. Click **Save**

---

## 3. 📡 Available Events

### Asset Lifecycle

| Event | When Triggered |
|-------|----------------|
| `asset.created` | New asset created |
| `asset.updated` | Asset updated |
| `asset.deleted` | Asset deleted |

### Allocation & Assignment

| Event | When Triggered |
|-------|----------------|
| `asset.allocated` | Asset allocated to staff |
| `asset.revoked` | Allocation revoked |

### Check-in/Check-out

| Event | When Triggered |
|-------|----------------|
| `asset.checked_out` | Asset checked out |
| `asset.checked_in` | Asset checked in |

### Reservations

| Event | When Triggered |
|-------|----------------|
| `asset.reserved` | Reservation created |
| `asset.reservation_approved` | Reservation approved |
| `asset.reservation_rejected` | Reservation rejected |

### Maintenance & Transfers

| Event | When Triggered |
|-------|----------------|
| `asset.maintenance_scheduled` | Maintenance scheduled |
| `asset.maintenance_completed` | Maintenance completed |
| `asset.transferred` | Transfer completed |

### Loss, Damage, Disposal

| Event | When Triggered |
|-------|----------------|
| `asset.lost` | Asset reported lost |
| `asset.broken` | Asset reported broken |
| `asset.warranty` | Asset sent for warranty |
| `asset.liquidated` | Asset liquidated |

### Alerts (via Cron)

| Event | When Triggered |
|-------|----------------|
| `alert.warranty_expiring` | Warranty expiring in 30 days |
| `alert.maintenance_due` | Maintenance due in 7 days |
| `alert.checkout_overdue` | Checkout overdue |
| `alert.low_stock` | Stock below threshold |

---

## 4. 📦 Payload Format

Each webhook sends a JSON payload:

```json
{
  "event": "asset.created",
  "timestamp": "2025-02-04T12:00:00+00:00",
  "source": "perfex_assets_module",
  "asset_id": 123,
  "asset": { ... },
  "data": { ... }
}
```

- **event** — Event name
- **timestamp** — ISO 8601 format
- **asset_id** — ID of the asset (null for deleted)
- **asset** — Asset data (or extra data for deleted)
- **data** — Event-specific data (e.g., allocation details)

---

## 5. 🔐 Signature Verification

The module sends an HMAC-SHA256 signature in the header:

```
X-Asset-Webhook-Signature: <signature>
X-Asset-Webhook-Timestamp: <unix_timestamp>
X-Asset-Webhook-Event: <event_name>
```

Verify in your endpoint:

```
signature = HMAC-SHA256(secret_key, request_body)
```

---

## 6. 📋 Webhook Logs

- View **Webhook Logs** to see delivery status
- **Response Code** — 2xx = success, 4xx/5xx = failure
- **Retry** — Some interfaces allow retrying failed deliveries
- Logs are typically cleaned after 30 days

---

## 7. 🧪 Test Webhook

Use **Test Webhook** to send a test payload. Useful to verify your endpoint is reachable and correctly configured.

---

## 💡 Best Practices

- ✅ **Use HTTPS** for webhook URLs
- ✅ **Verify signature** to ensure requests are from the module
- ✅ **Respond quickly** (e.g., 200 OK) — timeout is ~30 seconds
- ✅ **Handle duplicates** — same event may be retried
- ✅ **Monitor logs** for failed deliveries
