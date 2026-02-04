---
description: >-
  How to report and track damaged or non-functional assets using Asset
  Management module for Concord CRM
---

# ⚠️ Reporting Broken Assets

When assets become damaged, broken, or non-functional, the Asset Broken Report feature helps you document the incident, track affected quantities, and maintain accurate inventory records for proper asset lifecycle management.

<figure><img src="../.gitbook/assets/Screenshot from 2025-06-03 16-28-05.png" alt=""><figcaption><p>Asset Broken Report</p></figcaption></figure>

### 1. **Access Broken Report Feature**

**From Assets Section:** Navigate to the **Assets** section and click on the specific asset that has broken or damaged units. Look for broken report options in the asset detail page.

**From Asset Broken Reports Section:** Go directly to **Asset Broken Reports** to view all reported incidents across all assets or create new broken reports.

### 2. **Create New Broken Report**

Click on the **New Report** button to start documenting the broken asset incident. This opens a form specifically designed for capturing all relevant details about asset damage or malfunction.

### 3. **Fill in Report Details**

#### **Required Information**

* **Report Code**: System auto-generates unique code (BR-00000001), but you can modify if needed for your tracking system
* **Asset**: Select which asset has broken or damaged units (if not pre-selected)
* **Quantity**: Enter the exact number of units that are broken or damaged
* **Broken Time**: Set the date and time when the damage was discovered or occurred

#### **Detailed Documentation**

* **Description**: Provide comprehensive details about what happened, damage extent, potential causes, and any relevant circumstances

#### **Reference Information**

* **Remaining Quantity**: Shows current available/total quantity (e.g., "15 / 20" - helps understand impact on inventory)

### 4. **Report Validation**

The system automatically validates several aspects:

**Asset Validation**

* Confirms the selected asset exists in the system
* Checks asset availability and current status

**Quantity Validation**

* Ensures reported quantity is positive integer
* Prevents reporting more quantity than exist

**Data Integrity**

* Requires all mandatory fields to be filled
* Ensures broken time is valid date
* Maintains referential integrity with asset records

### 5. **Save the Report**

Click **Save** to complete the broken report. The system automatically:

* **Generates unique report code** for tracking and reference
* **Updates asset status history** with broken incident record
* **Links report to parent asset** for complete tracking
* **Validates data integrity** through database transaction
* **Creates permanent record** for insurance and reporting purposes

### 6. **What Happens After Reporting**

#### **System Updates**

* **Status history updated** with broken incident details
* **Report appears** in broken reports list with unique code
* **Inventory tracking** maintains broken unit records

#### **Record Keeping Benefits**

* **Complete audit trail** of all asset damage incidents
* **Historical tracking** for warranty and insurance claims
* **Compliance documentation** for regulatory requirements

### 💡 **Important Features**

#### **Unique Code Generation**

* **Sequential numbering** (BR-00000001, BR-00000002, etc.)
* **Automatic generation** prevents duplicates
* **Customizable prefix** if needed for organization standards
* **Easy reference** for insurance claims and reports

#### **Comprehensive Documentation**

* **Detailed description field** for incident specifics
* **Date/time tracking** for accurate timeline
* **Quantity specification** for inventory impact
* **Asset linkage** for complete history

#### **Status History Integration**

* **Automatic status recording** when reports are created
* **Timeline maintenance** for asset lifecycle
* **Audit compliance** with detailed change tracking
* **Historical reference** for future decision making

#### **Data Validation**

* **Required field enforcement** ensures complete documentation
* **Quantity validation** prevents data entry errors
* **Asset verification** confirms valid asset selection
* **Date validation** ensures realistic timing

### 🔍 **Viewing Broken Reports**

#### **Reports List View**

* **Report Code**: Unique identifier for each incident
* **Asset**: Which asset was affected
* **Quantity**: Number of broken units
* **Broken Time**: When incident occurred or was discovered
* **Description**: Summary of what happened

### 📋 **Best Practices**

#### **Incident Documentation**

* **Report immediately** when damage is discovered
* **Include detailed description** of circumstances and damage
* **Specify exact quantity** affected for accurate inventory
* **Set accurate date/time** for proper timeline tracking

#### **Description Guidelines**

* **What happened**: Clear explanation of the incident
* **Damage extent**: Specific details about what's broken
* **Potential cause**: If known, include likely reasons
* **Location**: Where the incident occurred
* **Discovery details**: How and when damage was found

#### **Inventory Management**

* **Regular monitoring** of broken reports for patterns
* **Trend analysis** to identify problematic assets
* **Warranty tracking** using report dates and details
* **Insurance documentation** with comprehensive records

#### **Compliance and Reporting**

* **Timely reporting** for insurance and warranty claims
* **Consistent reporting** across all asset types
* **Regular review** of broken asset trends

### 🚨 **Important Notes**

**Validation Rules**

* Report code must be unique across all reports
* Quantity must be positive integer minimum 1
* Broken time is required and must be valid date
* Asset must exist and be valid in the system

**System Behavior**

* **Database transaction** ensures data integrity
* **Status history automatically updated** for compliance
* **Module must be active** for functionality to work
* **Permissions required** for creating reports

**Record Permanence**

* **Cannot be easily deleted** once created for audit trail
* **Historical importance** for asset lifecycle management
* **Insurance and warranty** documentation requirements
* **Compliance and regulatory** record keeping needs
