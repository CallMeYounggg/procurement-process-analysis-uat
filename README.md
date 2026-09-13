# Procurement Process Analysis & UAT Support

> Portfolio simulation project demonstrating Procure-to-Pay (P2P) process analysis, business requirements documentation, User Acceptance Testing (UAT), defect management, retesting and procurement process improvement.

---

## 📌 Project Overview

This project simulates the analysis and User Acceptance Testing of an end-to-end Procure-to-Pay (P2P) procurement workflow within an ERP environment.

The project focuses on understanding business requirements, documenting procurement processes, developing UAT test scenarios, identifying defects and recommending process improvements.

**Project Type:** Portfolio Simulation
**Industry Context:** Healthcare / Procurement
**Process:** Procure-to-Pay (P2P)
**System Context:** ERP / SAP Ariba concepts

---

## 🎯 Project Objectives

* Analyze an end-to-end P2P procurement workflow
* Document business and system requirements
* Develop structured UAT test cases
* Validate positive and negative business scenarios
* Identify and document process/system defects
* Perform defect retesting
* Recommend procurement process improvements
* Demonstrate ERP functional analysis and UAT capabilities

---

## 🔄 Procure-to-Pay Process

The project covers the following workflow:

```text
Purchase Requisition
        ↓
PR Approval
        ↓
Purchase Order
        ↓
PO Approval
        ↓
Supplier Delivery
        ↓
Goods Receipt
        ↓
Supplier Invoice
        ↓
Three-Way Matching
        ↓
Invoice Approval
        ↓
Payment
```

---

## 📋 Business Requirements

The project defines business requirements covering:

| ID     | Requirement                                 | Priority |
| ------ | ------------------------------------------- | -------- |
| BR-001 | User can create a Purchase Requisition      | High     |
| BR-002 | Mandatory PR fields must be validated       | High     |
| BR-003 | Approved PR can be converted into a PO      | High     |
| BR-004 | PO information must be accurate             | High     |
| BR-005 | Goods Receipt can be recorded against PO    | High     |
| BR-006 | Excess receiving should be controlled       | Medium   |
| BR-007 | Invoice should be matched against PO and GR | High     |
| BR-008 | Invoice mismatches should be flagged        | High     |

---

## 🧪 User Acceptance Testing

UAT was designed to validate whether the procurement workflow satisfies defined business requirements.

Testing includes:

* Positive test scenarios
* Negative test scenarios
* Approval workflow testing
* Purchase Order validation
* Goods Receipt validation
* Invoice verification
* Three-way matching
* Exception handling

### Example UAT Scenario

**Test Case:** TC-006

**Scenario:** Invoice amount exceeds the Purchase Order amount.

**Expected Result:**
The system should identify the mismatch and place the invoice into an exception/review state.

**Initial Result:**
Invoice mismatch was not automatically flagged.

**Status:** Failed

**Defect:** DEF-001

---

## 🐛 Defect Management

Three simulated defects were identified during UAT.

| Defect  | Description                                      | Severity | Status |
| ------- | ------------------------------------------------ | -------- | ------ |
| DEF-001 | Invoice mismatch was not automatically flagged   | High     | Closed |
| DEF-002 | Goods Receipt allowed excessive quantity         | High     | Closed |
| DEF-003 | Cost Centre was not mandatory during PR creation | Medium   | Closed |

---

## 🔁 Retesting

Following corrective actions, the identified defects were retested.

| Defect  | Corrective Action                   | Retest Result |
| ------- | ----------------------------------- | ------------- |
| DEF-001 | Updated invoice matching validation | Passed        |
| DEF-002 | Added quantity validation           | Passed        |
| DEF-003 | Made Cost Centre mandatory          | Passed        |

**Final Retest Pass Rate: 100%**

---

## 💡 Process Improvement Recommendations

The analysis identified several opportunities for procurement process improvement:

### 1. Mandatory Field Validation

Reduce incomplete Purchase Requisitions by enforcing required procurement information.

### 2. Automated Approval Workflow

Reduce manual routing and improve approval visibility.

### 3. Automated Three-Way Matching

Improve invoice processing by automatically comparing:

```text
Purchase Order
      +
Goods Receipt
      +
Supplier Invoice
```

### 4. Quantity Controls

Prevent or flag Goods Receipts that exceed the Purchase Order quantity.

### 5. Standardized P2P Processes

Establish common procurement workflows and controls across business units.

---

## 📊 UAT Results

| Metric                 | Result |
| ---------------------- | -----: |
| Business Requirements  |      8 |
| UAT Test Cases         |     20 |
| Initial Passed         |     16 |
| Initial Failed         |      3 |
| Blocked                |      1 |
| Initial Pass Rate      |    80% |
| Defects Identified     |      3 |
| Defects Retested       |      3 |
| Final Retest Pass Rate |   100% |

---

## 🛠️ Tools & Skills

* Notion
* Microsoft Excel
* SQL
* Power BI
* Process Mapping
* User Acceptance Testing
* Requirements Analysis
* Defect Management
* ERP Procurement Processes
* Procure-to-Pay
* SAP Ariba Concepts

---

## 📁 Project Documentation

| Document                                               | Description                              |
| ------------------------------------------------------ | ---------------------------------------- |
| [Project Overview](docs/project-overview.md)           | Project background, objectives and scope |
| [Business Requirements](docs/business-requirements.md) | Procurement business requirements        |
| [P2P Process Analysis](docs/p2p-process-analysis.md)   | End-to-end process analysis              |
| [UAT Strategy](docs/uat-strategy.md)                   | UAT approach and testing scope           |
| [UAT Summary](docs/uat-summary.md)                     | Testing results and conclusions          |
| [Process Improvements](docs/process-improvements.md)   | Recommended procurement improvements     |

---

## 🔗 Portfolio

A detailed version of this project is documented in Notion.

**Notion Project:** [Add your Notion link here]

---

## ⚠️ Disclaimer

This is a portfolio simulation project created for demonstration and learning purposes. It does not represent confidential information, proprietary processes or actual SAP Ariba implementation activities performed for a real organization.
