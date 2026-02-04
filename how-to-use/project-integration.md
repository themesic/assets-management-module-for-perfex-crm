---
description: How to assign assets to projects in Perfex CRM
---

# 📁 Project Integration

The Assets module integrates with Perfex CRM **Projects**. Assign assets to projects directly from the project view and track which assets are used for each project.

---

## 1. 📍 Where to Find It

When viewing a **Project** in Perfex CRM:

1. Open the project
2. Look for the **Assets** tab (alongside Overview, Tasks, etc.)
3. Click the **Assets** tab

---

## 2. ➕ Assign an Asset to a Project

1. In the project's **Assets** tab, click **Assign Asset**
2. Select the **Asset** from the dropdown
3. Enter **Quantity** (default: 1)
4. Add **Notes** (optional)
5. Click **Assign**

### What Happens

- Asset is linked to the project
- Assignment is recorded with date
- Asset appears in the project's Assets tab
- You can remove the assignment later if needed

---

## 3. 🗑️ Remove Asset from Project

1. In the project's **Assets** tab, find the asset
2. Click the **Remove** or **Delete** action
3. Confirm — the asset is unlinked from the project (not deleted)

---

## 4. 📊 What You See

In the project Assets tab:

| Column | Description |
|--------|-------------|
| Asset Code | Unique code |
| Asset Name | Name |
| Quantity | Assigned quantity |
| Assigned Date | When it was assigned |
| Actions | Remove |

---

## 5. 🔐 Permissions

- **Assign** — Requires `assets` create or edit permission
- **Remove** — Requires `assets` edit permission
- **View** — Requires `assets` view permission

---

## 💡 Use Cases

- **Project-based equipment** — Laptops, projectors for specific projects
- **Cost tracking** — Link asset usage to project costs
- **Resource planning** — See which assets are committed to which projects
- **Client projects** — Assign assets to client projects for billing or reporting
