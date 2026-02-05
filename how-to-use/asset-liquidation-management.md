---
description: >-
  How to liquidate assets and track disposal proceeds using Asset Management
  module for Perfex CRM
---

# 💰 Asset Liquidation Management

When assets reach end-of-life, become obsolete, or need to be disposed of for other reasons, the Asset Liquidation feature helps you document the disposal process, track financial recovery, and maintain complete records for accounting and compliance purposes.

### 1. **Access Asset Liquidation**

**From Assets Section:** Navigate to the **Assets** section and click on the specific asset you want to liquidate. Look for liquidation options in the asset detail page.

**From Asset Liquidations Section:** Go directly to **Asset Liquidations** to view all completed liquidations across all assets or create new liquidation records.

### 2. **Create New Liquidation**

Click on the **New Liquidation** button to start documenting the asset disposal process. This opens a comprehensive form for recording all details about the liquidation transaction.

### 3. **Fill in Liquidation Details**

#### **Required Information**

* **Liquidation Code**: System auto-generates unique code (LQ-00000001), but you can modify if needed for your organization's tracking system
* **Asset**: Select which asset is being liquidated (if not pre-selected)
* **Quantity**: Enter the exact number of units being liquidated or disposed of
* **Liquidation Amount**: Enter the total amount received from the sale or disposal (can be 0 for donations/disposals)
* **Liquidation Time**: Set the date and time when the liquidation was completed

#### **Documentation Details**

* **Description**: Provide comprehensive details about the liquidation method, buyer information, disposal reasons, and any relevant circumstances

#### **Reference Information**

* **Remaining Quantity**: Shows current available/total quantity (e.g., "15 / 20" - helps track inventory impact)

### 4. **Liquidation Validation**

The system automatically validates several aspects:

**Asset Validation**

* Confirms the selected asset exists and is available for liquidation
* Checks current asset status and availability
* Validates user permissions for liquidation operations

**Financial Validation**

* Ensures liquidation amount is numeric and not negative
* Allows zero amounts for donations or disposal without proceeds

**Quantity Validation**

* Ensures liquidated quantity is positive integer
* Prevents liquidating more quantities than available
* Validates against current asset inventory levels

**Data Integrity**

* Requires all mandatory fields to be completed
* Ensures liquidation time is valid date

### 5. **Save the Liquidation**

Click **Save** to complete the liquidation record. The system automatically:

* **Generates unique liquidation code** for tracking and financial reporting
* **Updates asset status history** with liquidation transaction details
* **Records financial transaction** with amount and timestamp
* **Links liquidation to parent asset** for complete audit trail
* **Validates all data** through secure database transaction
* **Creates permanent record** for accounting and tax purposes

### 6. **What Happens After Liquidation**

#### **System Updates**

* **Status history updated** with liquidation details and financial information
* **Liquidation appears** in liquidations list with unique tracking code

#### **Financial Tracking Benefits**

* **Complete audit trail** of all asset disposals and proceeds
* **Compliance records** for regulatory and audit requirements

### 💡 **Important Features**

#### **Unique Code Generation**

* **Sequential numbering** (LQ-00000001, LQ-00000002, etc.)
* **Automatic generation** prevents duplicates and ensures tracking
* **Customizable prefix** if needed for accounting integration

#### **Financial Documentation**

* **Liquidation amount tracking** for accurate financial records
* **Zero amount support** for donations or disposals without proceeds

#### **Comprehensive Record Keeping**

* **Detailed description field** for disposal method and circumstances
* **Date/time tracking** for accurate transaction timeline
* **Quantity specification** for inventory impact assessment
* **Asset linkage** for complete lifecycle documentation

#### **Status History Integration**

* **Automatic status recording** when liquidations are processed
* **Timeline maintenance** for complete asset lifecycle
* **Historical reference** for future disposal decisions

### 🔍 **Viewing Liquidations**

#### **Liquidations List View**

* **Liquidation Code**: Unique identifier for each disposal transaction
* **Asset**: Which asset was liquidated
* **Quantity**: Number of units disposed of
* **Liquidation Amount**: Financial proceeds from disposal
* **Liquidation Time**: When the disposal was completed

### 🚨 **Important Notes**

**Validation Rules**

* Liquidation code must be unique across all transactions
* Quantity must be positive integer minimum 1
* Liquidation amount must be numeric and cannot be negative
* Liquidation time is required and must be valid date

**Financial Considerations**

* **Zero amounts allowed** for donations or disposals without proceeds
* **Negative amounts not permitted** - use separate expense tracking

**System Behavior**

* **Database transaction** ensures complete data integrity
* **Status history automatically updated** for compliance tracking
