---
description: >-
  How to revoke assets from users and return them to inventory using the Asset
  Management module for Perfex CRM
---

# 🔄 Asset Revocation Management

When assets need to be recalled from users, returned to inventory, or reassigned to different personnel, the Asset Revocation feature helps you manage the complete return process with proper documentation and notifications.

### 1. **Access Revocation Feature**

**From Assets Section:** Navigate to the **Assets** section and click on the specific asset that needs to be revoked. Look for revocation options in the asset detail page.

**From Asset Revocations Section:** Go directly to **Asset Revocations** to view all revocation records or create new revocation requests.

### 2. **Create New Revocation Request**

Click on the **New Revocation** button to start documenting the asset return. This opens a comprehensive form for capturing all revocation details.

### 3. **Fill in Revocation Details**

#### **Required Information**

* **Revocation Code**: System automatically creates a unique code (RV-00000001) for tracking purposes
* **Asset**: Select which asset is being revoked from current user
* **Revoked By**: Choose the person/administrator initiating the revocation
* **Quantity**: Enter the exact number of units being revoked
* **Revoke Time**: Set the date and time when the revocation takes effect

#### **User Information**

* **Revoked From**: Select the user who currently has the asset and must return it
* **Notification**: System automatically sends notification to the user about the revocation

#### **Location Information**

* **Asset Location**: Where the asset is currently located (user's office, department, etc.)
* **Handover Location**: Where the asset should be returned or collected

#### **Additional Details**

* **Reason**: Provide clear explanation for the revocation, such as:
  * Employee termination or transfer
  * Asset reassignment to different user
  * Equipment recall for maintenance
  * Policy compliance requirements
  * Asset upgrade or replacement

#### **Reference Information**

* **Remaining Quantity**: Shows current available/total quantity after revocation

### 4. **Save the Revocation Request**

Click **Save** to complete the revocation request. The system will:

* Generate a unique revocation code for tracking
* Send automatic notification to the user being revoked from
* Update the asset's status history
* Record the revocation in the asset lifecycle

### 5. **What Happens After Revocation**

#### **Automatic Notifications**

* **User Notification**: The user losing access receives immediate notification
* **Email Details**: Includes revocation code, asset details, and return instructions

#### **Asset Status Updates**

* Asset status history updated with revocation record
* Asset becomes available for new allocations

### 💡 **Key Features**

#### **Comprehensive Tracking**

* **Unique revocation codes** for each request (RV-00000001, RV-00000002, etc.)
* **User identification** for both revoker and revokee

### 🔍 **Viewing Revocation Records**

#### **Revocations Overview**

* **Revocation Code**: Unique identifier for each revocation
* **Asset**: Which asset was revoked
* **Quantity**: How many units were returned
* **Revoked From**: User who returned the asset
* **Revoked By**: Administrator who initiated the revocation
* **Revoke Time**: When the revocation took place
