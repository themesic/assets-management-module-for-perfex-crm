---
description: >-
  How to assign assets to users and track their usage using Asset Management
  module for Perfex CRM
---

# 🎯 Allocating Assets

When you need to assign assets to users (like giving laptops to employees or allocating equipment to departments), the Asset Allocation feature helps you track who has what, when they received it, and manage the entire allocation lifecycle.

### 1. **Access Asset Allocation**

**From Assets Section:** Navigate to the **Assets** section and click on the specific asset you want to allocate. In the asset detail page, you'll find allocation-related options.

**From Asset Allocations Section:** Go directly to **Asset Allocations** to view all current allocations across all assets or create new ones.

### 2. **Create New Allocation**

Click on the **New Allocation** button to start the allocation process. This opens a comprehensive form for recording asset assignment details.

### 3. **Fill in Allocation Details**

#### **Required Information**

* **Allocated To**: Select the user who will receive the asset from the user dropdown
* **Allocation Code**: System auto-generates unique code (AL-00000001), but you can modify if needed
* **Asset**: Choose which asset is being allocated (if not pre-selected)
* **Quantity**: Enter the number of units being allocated to this user
* **Allocation Time**: Set the date and time when the asset is being handed over

#### **Location Information**

* **Asset Location**: Current location of the asset before allocation
* **Handover Location**: Where the asset will be handed over to the user

#### **Additional Details**

* **Reason**: Document why this allocation is being made (e.g., "New employee onboarding", "Equipment replacement", "Temporary project assignment")

#### **Reference Information**

* **Remaining Quantity**: Shows available/total quantity (e.g., "15 / 20" - 15 available out of 20 total)

### 4. **Allocation Validation**

The system automatically validates several aspects:

**Quantity Validation**

* Ensures requested quantity doesn't exceed available quantity
* Prevents over-allocation of assets
* Shows real-time remaining quantity

**Asset Validation**

* Confirms the selected asset exists and is available
* Checks asset status and allocation eligibility
* Validates user permissions for allocation

### 5. **Save the Allocation**

Click **Save** to complete the allocation. The system automatically:

* **Updates available quantity** (reduces by allocated amount)
* **Records allocation history** in asset timeline
* **Sends notification email** to the allocated user
* **Creates status history** entry for audit trail
* **Links user to asset** for easy tracking

### 6. **What Happens After Allocation**

#### **System Updates**

* **Available quantity decreases** by allocated amount
* **User receives email notification** about asset assignment

#### **Tracking Benefits**

* **Complete audit trail** of who has what asset
* **Email notifications** keep users informed
* **Status history** tracks all allocation events
* **Quantity management** prevents over-allocation

### 💡 **Important Features**

#### **Email Notifications**

* **Automatic emails** sent to users when assets are allocated
* **Allocation details** included in notification
* **Asset information** and pickup instructions provided

#### **Quantity Management**

* **Real-time availability** checking
* **Prevents over-allocation** with validation
* **Accurate inventory** tracking maintained

### 🔍 **Viewing Allocations**

#### **Asset Allocations List**

* **Allocation Code**: Unique identifier for each allocation
* **Asset**: Which asset was allocated
* **Quantity**: How many units allocated
* **Allocated To**: User who received the asset
* **Allocation Time**: When the allocation was made

### 📋 **Best Practices**

#### **Documentation**

* **Always specify reason** for allocation
* **Include handover location** for clarity
* **Set accurate allocation time** for proper tracking

#### **Communication**

* **Verify user email** before allocation for notifications
* **Confirm handover details** with the user
* **Document any special instructions** in reason field

#### **Quantity Management**

* **Check available quantity** before allocation
* **Plan allocations** to avoid shortages
* **Monitor remaining inventory** regularly

#### **Record Keeping**

* **Use meaningful allocation codes** if customizing
* **Maintain consistent location naming**
* **Regular review** of active allocations

### 🚨 **Important Notes**

**Validation Rules**

* Quantity must be positive integer
* Cannot exceed available quantity
* User and asset must exist in system
* Allocation time is required

**System Behavior**

* **Immediate inventory update** upon allocation
* **Email sent automatically** if user has valid email
* **Status history recorded** for compliance
* **Transaction wrapped** for data integrity

**Permissions**

* Users need appropriate permissions to create allocations
* Asset module must be active
* Some fields may be restricted based on user role
