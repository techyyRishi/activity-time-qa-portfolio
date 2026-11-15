# Activity Time – Quick Edit Feature Analysis

## Project Overview

This document showcases a detailed functional analysis of the **Quick Edit functionality** in the Activity Time platform.

The analysis focuses on two major listing workflows:

- **Edit Listing:** Evaluating how the Quick Edit menu and individual listing sections behave when modifying an existing published listing.
- **Duplicate Listing:** Evaluating how the Quick Edit menu and listing sections behave when creating a new listing by duplicating an existing one.

The objective was to understand feature behaviour across both workflows, validate consistency, identify functional gaps, and highlight opportunities to improve the overall user experience.

## Objective

To perform a structured, scenario-based analysis of the Quick Edit functionality and ensure that listing modifications and duplication workflows behave consistently and reliably.

Key objectives included:

- Validate existing data retention when editing or duplicating listings.
- Analyse field editability and restricted configurations.
- Verify navigation between sections through Quick Edit, Next, Back, and Dashboard actions.
- Evaluate input validation, boundary conditions, and mandatory field behaviour.
- Verify Save Changes and Save Draft functionality.
- Validate data persistence after browser refresh and reopening.
- Compare Edit Listing and Duplicate Listing behaviour.
- Identify functional inconsistencies and potential UX improvements.

## My Contribution

I independently performed feature-level analysis and prepared detailed scenario coverage for both Edit Listing and Duplicate Listing workflows.

My contributions included:

1. **Workflow Analysis:** Analysed both listing workflows independently to understand their behaviour and identify differences in functionality.

2. **Scenario Design:** Created structured test scenarios covering existing data retention, field modifications, restricted fields, validation, navigation, and publishing.

3. **Business Logic Validation:** Evaluated age restrictions, date and time configurations, pricing rules, deposit validation, discounts, space capacity, and listing policies.

4. **Quick Edit Navigation Analysis:** Verified direct section navigation and consistency while moving between different listing sections.

5. **Data Persistence Analysis:** Checked whether modified information remained consistent after saving, refreshing, reopening, and publishing listings.

6. **Comparative Analysis:** Compared the behaviour of Edit Listing and Duplicate Listing to identify inconsistencies in similar functionalities.

7. **Gap Identification:** Documented observed issues, weak validations, save-state inconsistencies, and areas requiring further requirement clarification.

8. **Expected Behaviour Definition:** Documented expected outcomes alongside actual application behaviour to make observations actionable for development and product discussions.

## Analysis Coverage

### 1. Edit Listing Workflow

Analysed the following sections:

- Categories
- Activity Type / Subcategories
- Title
- In-person / Online
- Age
- Photos
- Description
- What to Bring
- Days & Time
- Pricing
- Number of Spaces
- Policies
- Publish

### 2. Duplicate Listing Workflow

Analysed the corresponding sections during listing duplication, including:

- Retention of original listing information.
- Modification of duplicated listing information.
- Restricted field behaviour.
- Validation and boundary conditions.
- Save Draft and Review & Publish behaviour.
- Quick Edit navigation.
- Data persistence and publishing consistency.

## Key Observations & Improvement Opportunities

The analysis highlighted several areas requiring attention.

| Area | Observation |
|---|---|
| Title Validation | Minimum character and special character validation require improvement in certain flows. |
| Description | Weak minimum character validation and inconsistent space handling were observed. |
| Photos | Deleted images reappeared after refresh in the Edit Listing flow. |
| Save State | Save Changes and Save Draft button states showed inconsistencies in certain sections. |
| Date & Time | Editing ongoing listings could block progression when existing dates were not modified. |
| Pricing | Free listing conversion and invalid deposit combinations required further validation. |
| Discount Logic | Early Bird and Sibling Discount calculations displayed inconsistent savings information in a booking scenario. |
| Capacity | Configured total spaces and remaining spaces were not consistently represented in the editing configuration. |
| Duplicate Flow | Consent persistence and Save Draft behaviour required additional attention. |

These observations were documented with current behaviour, expected behaviour, results, and remarks in the supporting scenario document.

## Analysis Approach

I followed a structured analysis approach:

1. Understand the existing listing workflow.
2. Identify individual sections and available actions.
3. Define positive, negative, boundary, and navigation scenarios.
4. Execute scenarios against the application.
5. Compare current behaviour with expected behaviour.
6. Record observations and improvement opportunities.
7. Compare Edit Listing and Duplicate Listing workflows.
8. Document findings for further review and discussion.

## Supporting Evidence

The following document contains the detailed scenario analysis prepared during this activity.

**Quick Edit – Edit Listing & Duplicate Listing Scenario Analysis**

[View Quick Edits Scenario Analysis (PDF)](./Quick%20Edits_scenarios.pdf)

The PDF includes:

- Scenario descriptions
- Actions and button interactions
- Current application behaviour
- Expected behaviour
- Execution results
- Remarks and improvement observations

## Skills Demonstrated

- Functional Testing
- Requirement & Feature Analysis
- Test Scenario Design
- Positive & Negative Testing
- Boundary Value Analysis
- Business Logic Validation
- Regression Testing
- Workflow & Navigation Validation
- Data Persistence Testing
- UI/UX Improvement Identification
- Comparative Feature Analysis
- Defect Identification & Documentation

## Professional Impact

This analysis demonstrates my approach to understanding application behaviour beyond basic happy-path testing.

By evaluating both existing listing modifications and listing duplication workflows, I focused on identifying inconsistencies, validating business rules, and documenting actionable improvement opportunities.

My goal is to contribute to better product reliability, improved user experience, and stronger functional quality through structured analysis and risk-focused testing.

---

**Role:** Software QA Engineer – Manual & Automation Testing  
**Project:** Activity Time  
**Focus:** Quick Edit – Edit Listing & Duplicate Listing Analysis
