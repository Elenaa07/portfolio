# **Running a Metadata Migration**

This guide provides step-by-step instructions for conducting a metadata migration, focusing on updating metadata for a large set of videos already present in an account.

---

## **Introduction**

A metadata migration is essential for updating video information at scale. Common use cases include:
- Adding cue points to multiple videos.
- Updating or adding custom fields or video metadata.

---

## **Process Overview**

1. [Pre-Migration Preparation](#1-pre-migration-preparation)
2. [Metadata Mapping](#2-metadata-mapping)
3. [Formatting to JSON](#3-formatting-to-json)
4. [Using the Metadata Migration Tool](#4-using-the-metadata-migration-tool)
5. [Validation](#5-validation)
6. [Migration Approval](#6-migration-approval)
7. [Post-Migration Activities](#7-post-migration-activities)

---

## **1. Pre-Migration Preparation**

### **Objective**
Ensure all required metadata fields are correctly prepared for migration.

### **Steps**
1. Use the provided metadata ingest sheet template to structure your data.
2. Copy necessary fields for the migration into a new sheet.
3. Populate columns with customer-provided metadata.
4. Export the sheet as a **CSV** file for further processing.

### **Tip**
Use consistent column headers to simplify conversion to JSON in the next step.

---

## **2. Metadata Mapping**

### **Objective**
Convert the metadata CSV file into JSON format compatible with the CMS API.

### **Steps**
1. Use a [CSV to JSON converter](https://www.convertcsv.com/csv-to-json.htm) to format the CSV data.
2. Ensure the JSON includes the following fields:
   - Start date
   - Tags
   - Custom fields
   - Cue points
3. Wrap numerical custom fields in quotation marks (option available in the converter).

### **Tip**
Save the JSON file securely for reuse or troubleshooting.

---

## **3. Formatting to JSON**

### **Objective**
Prepare JSON data for submission through the Metadata Migration Tool.

### **Steps**
1. Access the Metadata Migration Tool.
2. Use migration credentials from the **Master Migration Metadata Sheet**.
3. Paste the JSON data into the tool.
4. Limit the migration to **500 assets per batch** to ensure smooth processing.
5. Submit the migration and monitor for errors.

### **Error Handling**
If errors occur:
- Review and adjust the metadata or JSON formatting.
- Resubmit the migration.

---

## **4. Using the Metadata Migration Tool**

### **Objective**
Verify the metadata migration results.

### **Steps**
1. In **Video Cloud**, search for videos updated during the migration.
2. Export a CSV of the updated videos.
3. Compare the updated data with the original metadata CSV using a [list differentiation tool](http://www.listdiff.com/compare-2-lists-difference-tool).

### **Validation Checklist**
- Confirm updated fields are accurate.
- Verify all intended videos were updated.

---

## **5. Validation**

### **Objective**
Ensure the migration meets quality standards before customer review.

### **Steps**
1. Review the updated metadata export.
2. Document any notes or issues encountered during migration.
3. Send the export and notes to the customer.

---

## **6. Migration Approval**

### **Objective**
Obtain customer confirmation of a successful migration.

### **Steps**
1. Share the updated metadata export with the customer.
2. Address any issues or feedback.
3. Secure formal approval.

---

## **7. Post-Migration Activities**

### **Objective**
Complete the migration process and gather feedback.

### **Steps**
1. Send a close-out email summarizing the migration process.
2. Share a migration survey to collect customer feedback for process improvement.

---

## **Resources**

- [CSV to JSON Converter](https://www.convertcsv.com/csv-to-json.htm)
- [CMS API Reference](https://apis.support.brightcove.com/cms/references/reference.html#tag/Videos/operation/GetVideos)
- [List Differentiator Tool](http://www.listdiff.com/compare-2-lists-difference-tool)

---

By following this guide, you can ensure a seamless metadata migration process while maintaining data accuracy and customer satisfaction. If you need additional assistance, consult the relevant resources or contact support.