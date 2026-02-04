---
description: How to check out and check in assets temporarily using the Asset Management module
---

# 🔄 Check-in/Check-out

The **Check-in/Check-out** feature lets you temporarily assign assets to staff or clients with an expected return date. Perfect for equipment loans, project-based use, or short-term assignments.

---

## 📌 Check-out vs. Allocation

| Feature | Check-out | Allocation |
|---------|-----------|------------|
| **Duration** | Temporary (has return date) | Long-term/permanent |
| **Use Case** | Laptops for travel, projectors for meetings | Assigned desk, company phone |
| **Overdue Alerts** | ✅ Yes | ❌ No |
| **Return Tracking** | ✅ Yes (condition, date) | Via Revocation |

---

## 1. 📍 Access Check-in/Check-out

**Navigation:** **Assets** → **Check-in/out** from the sidebar.

---

## 2. 📤 Check Out an Asset

### Steps

1. Click **Check Out Asset** or **New Checkout**
2. Select **Asset** from the dropdown
3. Select **Checked Out To** (staff member or client/contact)
4. Enter **Quantity** (if multiple units)
5. Set **Expected Return Date** (recommended for overdue alerts)
6. Add **Checkout Notes** (optional) — e.g., "For conference in Berlin"
7. Select **Condition** (Excellent, Good, Fair, Poor) — default: Good
8. Click **Save**

### What Happens

- ✅ Asset's allocated quantity increases
- ✅ Checkout record is created with status `checked_out`
- ✅ Audit log entry is created
- ✅ Webhook `asset.checked_out` is triggered (if configured)
- ✅ If expected return date passes, status becomes `overdue` and notifications are sent (via cron)

---

## 3. 📥 Check In an Asset

### Steps

1. Go to **Assets** → **Check-in/out**
2. Find the checkout record (filter by status: Checked Out or Overdue)
3. Click **Check In** or the check-in action
4. Optionally add **Check-in Notes**
5. Select **Return Condition** (Excellent, Good, Fair, Poor, Damaged)
6. Click **Save**

### What Happens

- ✅ Asset's allocated quantity decreases
- ✅ Checkout status changes to `returned`
- ✅ Actual return date is recorded
- ✅ Audit log and webhook `asset.checked_in` are triggered

---

## 4. 🔔 Overdue Checkouts

When the **expected return date** has passed and the asset is not returned:

- Status automatically changes to **Overdue**
- **Cron job** sends notifications to configured recipients
- Webhook `alert.checkout_overdue` is triggered
- Dashboard shows **Overdue Checkouts** count

**Ensure your Perfex cron is running** for overdue alerts to work.

---

## 5. 📊 Viewing Checkouts

In **Assets** → **Check-in/out** you can see:

| Column | Description |
|--------|-------------|
| Asset | Asset name and code |
| Checked Out To | Staff or client |
| Checkout Date | When it was checked out |
| Expected Return | Due date |
| Status | Checked Out, Returned, Overdue |
| Quantity | Units checked out |

Filter by status to find active or overdue checkouts quickly.

---

## 💡 Best Practices

- ✅ **Always set expected return date** for better tracking
- ✅ **Record condition** at check-in to spot damage trends
- ✅ **Use notes** for project or purpose
- ✅ **Run overdue report** regularly to follow up
- ✅ **Configure notifications** so overdue items don't slip through
