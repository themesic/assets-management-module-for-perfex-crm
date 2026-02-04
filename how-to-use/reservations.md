---
description: How to create and manage asset reservations in the Asset Management module
---

# 📅 Reservations

The **Reservations** feature lets you book assets in advance for a specific time period. Reservations can be pending, approved, or rejected, and the system checks availability to prevent double-booking.

---

## 1. 📍 Access Reservations

**Navigation:** **Assets** → **Reservations** from the sidebar.

---

## 2. ➕ Create a New Reservation

### Steps

1. Click **New Reservation** or **Make Reservation**
2. Select **Asset**
3. Set **Start Date** and **End Date** (and time if applicable)
4. Enter **Quantity** (how many units to reserve)
5. Select **Reserved By** (staff member)
6. Add **Purpose** (optional) — e.g., "Client presentation"
7. Add **Notes** (optional)
8. Click **Save**

### Validation

- The system checks that the requested quantity is **available** during the selected period
- It considers existing **approved** reservations and current **allocations**
- If not available, you'll see an error message

---

## 3. 📋 Reservation Statuses

| Status | Description |
|--------|-------------|
| **Pending** | Awaiting approval |
| **Approved** | Confirmed — asset is reserved |
| **Rejected** | Denied |
| **Cancelled** | Cancelled by user |
| **Completed** | Reservation period has ended |

---

## 4. ✅ Approve or Reject Reservations

**For admins/managers:**

1. Go to **Assets** → **Reservations**
2. Find reservations with status **Pending**
3. Click **Approve** or **Reject**
4. If rejecting, optionally add a **Rejection Reason**

### What Happens on Approval

- Status changes to **Approved**
- Asset is reserved for that period
- Notification is sent to the requester (if configured)
- Webhook `asset.reservation_approved` is triggered

### What Happens on Rejection

- Status changes to **Rejected**
- Notification is sent to the requester
- Webhook `asset.reservation_rejected` is triggered

---

## 5. 📅 Calendar View

Some interfaces offer a **Calendar View** to see reservations visually. Use it to:

- Spot conflicts
- Plan resource allocation
- See when assets are free

---

## 6. 🔍 Availability Check

The system calculates availability as:

```
Available = Total Quantity - Allocated - Reserved (approved, overlapping period)
```

When creating a reservation, the system ensures:

- No overbooking
- Quantity requested ≤ available during the period

---

## 💡 Best Practices

- ✅ **Approve or reject promptly** so requesters know their status
- ✅ **Use purpose/notes** for context and reporting
- ✅ **Check calendar** before approving to avoid conflicts
- ✅ **Set up notifications** so users are informed of approval/rejection
