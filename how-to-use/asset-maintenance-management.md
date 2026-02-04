---
description: >-
  How to send assets for maintenance, track service progress, and retrieve
  assets back to inventory using the Asset Management module for Perfex CRM
---

# 🔧 Asset Maintenance Management

When assets need repair, servicing, or preventive maintenance, the Asset Maintenance feature helps you manage the entire maintenance lifecycle from sending assets to service providers through completion and retrieval.

<figure><img src="../.gitbook/assets/Screenshot from 2025-06-03 16-41-25.png" alt=""><figcaption></figcaption></figure>

### 1. **Access Maintenance Feature**

**From Assets Section:** Navigate to the **Assets** section and click on the specific asset that needs maintenance. Look for maintenance options in the asset detail page.

**From Asset Maintenance Section:** Go directly to **Asset Maintenance** to view all maintenance records or create new maintenance requests.

### 2. **Create New Maintenance Request**

Click on the **New Maintenance** button to start documenting the maintenance request. This opens a comprehensive form for capturing all service details.

### 3. **Fill in Maintenance Details**

#### **Required Information**

* **Maintenance Code**: System automatically creates a unique code (MNT-00000001) for tracking purposes
* **Asset**: Select which asset needs maintenance service
* **Quantity**: Enter the exact number of units being sent for maintenance
* **Maintenance Start Date**: Set when the maintenance service begins
* **Maintenance Cost**: Enter the expected or quoted cost for the service

#### **Service Information**

* **Expected Completion Date**: When you expect the maintenance to be finished
* **Service Provider**: Name of the company or person performing the maintenance
* **Maintenance Type**: Choose from:
  * **Preventive**: Scheduled maintenance to prevent issues
  * **Corrective**: Repairs to fix existing problems
  * **Emergency**: Urgent repairs for critical failures

#### **Additional Details**

* **Reason**: Why the asset needs maintenance (e.g., "Regular service", "Equipment malfunction", "Safety inspection")
* **Description**: Detailed information about the work to be performed, specific issues, or service requirements

#### **Reference Information**

* **Remaining Quantity**: Shows current available/total quantity to understand inventory impact

### 4. **Save the Maintenance Request**

Click **Save** to complete the maintenance request. The system will:

* Generate a unique maintenance code for tracking
* Update the asset's status history to "maintenance"
* Send notification to the asset owner/company
* Create a permanent maintenance record
* Link the request to the asset for complete tracking

### 5. **Maintenance Lifecycle Management**

#### **Active Maintenance Tracking**

**Status Monitoring**

* **Pending**: Maintenance is scheduled or in progress
* **Retrieved**: Asset has been returned from maintenance

**Automatic Follow-ups**

* System automatically sends follow-up notifications for overdue maintenance
* Follow-ups triggered when expected completion date passes
* Notifications sent to asset company/owner for action

#### **Maintenance Retrieval Process**

<figure><img src="../.gitbook/assets/Screenshot from 2025-06-03 16-42-15 (1).png" alt=""><figcaption><p>Maintenance Retrieval</p></figcaption></figure>



**When Assets Are Ready**

1. Navigate to the asset's detail page
2. Go to the **Maintenance** tab
3. Find the active maintenance record
4. Click **Retrieve Asset** action
5. Asset status updates to "retrieved"
6. Available quantity is restored to inventory
7. Maintenance completion is recorded in asset history

### 6. **What Happens During Maintenance**

#### **Notifications System**

**Initial Notification**

* Asset owner/company receives notification when asset sent to maintenance
* Includes maintenance details and expected completion

**Follow-up Notifications**

* Automatic reminders sent after expected completion date
* Helps ensure timely retrieval of serviced assets
* Prevents assets from being forgotten at service providers

### 💡 **Key Features**

#### **Comprehensive Tracking**

* **Unique maintenance codes** for each service request (MNT-00000001, MNT-00000002, etc.)
* **Complete cost tracking** for budgeting and reporting
* **Service provider records** for vendor management
* **Maintenance type categorization** for analysis

#### **Automated Management**

* **Inventory updates** automatically when assets sent/retrieved
* **Status history tracking** for complete audit trail
* **Notification system** for proactive follow-up
* **Integration** with asset lifecycle management

### 🔍 **Viewing Maintenance Records**

#### **Maintenance Overview**

* **Maintenance Code**: Unique identifier for each service
* **Asset**: Which asset is being serviced
* **Quantity**: How many units are in maintenance
* **Start Date**: When maintenance began
* **Cost**: Service cost for budgeting

### 📋 **Best Practices**

#### **Planning Maintenance**

* **Schedule preventive maintenance** during low-usage periods
* **Get quotes** before entering maintenance costs
* **Confirm service provider** availability and timeline
* **Document specific issues** clearly in descriptions

#### **Information to Include**

* **Detailed problem description** for corrective maintenance
* **Service requirements** and specifications
* **Warranty information** if applicable
* **Special handling instructions** for delicate equipment
* **Contact information** for coordination

#### **Follow-up Actions**

* **Monitor expected completion dates** regularly
* **Contact service providers** for status updates
* **Retrieve assets promptly** when maintenance completes
* **Review maintenance costs** against budgets
* **Update maintenance schedules** based on service results

### 🚨 **Important Reminders**

#### **System Behavior**

* Each maintenance request gets a permanent, unique tracking code
* Assets in maintenance are unavailable for allocation
* Automatic notifications require proper company/user setup
* Maintenance records cannot be easily deleted to maintain audit trail
* Retrieved assets automatically restore inventory availability

