# **Managing a Migration**

This document provides a detailed guide for managing a migration as part of customer onboarding.

---

## **Overview of the Migration Process**

1. [Pre-Migration](#pre-migration)
2. [Metadata Mapping](#metadata-mapping)
3. [Migration Document Preparation](#migration-document-preparation)
4. [Testing Sample Data](#testing-sample-data)
5. [Completing the Migration](#completing-the-migration)
6. [Migration Approval](#migration-approval)
7. [Post-Migration Activities](#post-migration-activities)

---

## **1. Pre-Migration**

### **Objective**:
Define the migration scope and align on expectations.

- Migrations can be:
  - A **standalone project**
  - Part of a **Video Cloud onboarding**
- For standalone migrations:
  - Schedule a Kick-Off session to clarify goals, deliverables, and timelines.

---

## **2. Metadata Mapping**

### **Objective**:
Align metadata requirements between systems.

- **Actions**:
  - Schedule meetings to discuss:
    - Metadata mapping using `Migration Metadata Mapping.xlsx`.
    - Ingest profiles.
    - Data transfer methods (MRSS feed or CSV file).
    - Timeline and deadlines.
  - Revise the mapping document iteratively.

- **Customer To-Do**:
  - Ensure media URLs are publicly accessible or hosted in an S3 bucket ([Learn more](https://apis.support.brightcove.com/dynamic-ingest/general/using-dynamic-ingest-s3.html#setPolicy)).
  - Provide 10–15 sample entries in a Google Drive folder.

---

## **3. Migration Document Preparation**

### **Objective**:
Document migration specifics and secure necessary credentials.

- **OEM Responsibilities**:
  - Generate API credentials ([API Guide](https://apis.support.brightcove.com/general/managing-api-authentication-credentials.html)).
  - Update the `Master Migration Metadata` spreadsheet with:
    - Metadata mapping details.
    - Publisher ID.
    - API credentials.
  - Confirm document completion and placement in the customer’s folder.

---

## **4. Testing Sample Data**

### **Objective**:
Validate the migration process with sample data.

- **Steps**:
  - Prepare a [Test Document Template](https://docs.google.com/document/d/1c1iCAJWW0lRQNgFIU0o2TE1Bcdz2ZGmASa5CE5WOx7M/edit).
  - Share sample assets with the customer.
  - Conduct spot checks to validate data quality.

---

## **5. Completing the Migration**

### **Objective**:
Execute the migration and ensure data integrity.

- **Steps**:
  - Confirm customer completion of the migration document with:
    - Reference ID
    - Video ID
    - Video Name
  - Notify support to proceed with production migration.

---

## **6. Migration Approval**

### **Objective**:
Obtain final customer approval for the migration.

- **Steps**:
  - Retrieve the ingested assets spreadsheet from support ([Asset Tracking Template](https://docs.google.com/document/d/11EJL4S_RK8wgKLF4v_8DhVA3mmfrHDeKN_y59-0zMbk/edit)).
  - Cross-check the ingested assets for accuracy.
  - Address discrepancies and seek final customer approval.

---

## **7. Post-Migration Activities**

### **Objective**:
Wrap up the migration process and collect feedback.

- **Steps**:
  - Send a close-out email summarizing the migration.
  - Share a survey link for customer feedback.

---

## **References and Resources**

- [Using Dynamic Ingest with S3](https://apis.support.brightcove.com/dynamic-ingest/general/using-dynamic-ingest-s3.html#setPolicy)
- [API Authentication Guide](https://apis.support.brightcove.com/general/managing-api-authentication-credentials.html)
- [Test Sample Document Template](https://docs.google.com/document/d/1c1iCAJWW0lRQNgFIU0o2TE1Bcdz2ZGmASa5CE5WOx7M/edit)
- [Asset Tracking Template](https://docs.google.com/document/d/11EJL4S_RK8wgKLF4v_8DhVA3mmfrHDeKN_y59-0zMbk/edit)

For additional support, visit the [Brightcove Support Center](https://brightcove.atlassian.net/wiki/spaces/CO/pages).