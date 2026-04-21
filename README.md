# SAP ABAP Capstone Project — Custom ALV Report (ZSOLIST)

**Name:** Afiyah Firdous
**Roll Number:** 2306092
**School:** School of Computer Engineering, KIIT University
**Program:** SAP ABAP
**Topic:** Real ABAP Development Scenario — Custom ALV Report (Topic vi)
**Submission Deadline:** April 21, 2026

---

## Project Overview

This project implements a custom SAP ABAP ALV Grid report (`ZSOLIST`) that retrieves and displays Sales Order header and item data from the SAP SD module. The report fetches data from the `VBAK` (Sales Order Header) and `VBAP` (Sales Order Item) tables using an INNER JOIN and presents it in an interactive, formatted ALV Grid on a custom Dynpro screen.

---

## Files in this Submission

| File | Description |
|------|-------------|
| `SAP_Capstone_Project_Report.pdf` | Full project documentation (Title, Problem Statement, Solution, Tech Stack, Steps, Code, Unique Points, Future Improvements) |
| `ZSOLIST_Source_Code.txt` | Complete ABAP source code for the custom ALV report program |
| `ZSSODATA_Structure.txt` | Data Dictionary structure definition for the custom output structure used by the ALV grid |
| `README.md` | This file — project overview and submission details |

---

## SAP Objects Created

| Object | Type | Transaction |
|--------|------|-------------|
| `ZSSODATA` | Dictionary Structure | SE11 |
| `ZSOLIST` | ABAP Executable Program | SE38 |
| Screen 100 | Dynpro Screen | SE51 |
| `SOLIST` | GUI PF-Status | SE41 |
| `SOL` | Title Bar | SE41 |

---

## How to Run

1. Create the `ZSSODATA` structure in SE11 using the field definitions in `ZSSODATA_Structure.txt`
2. Create and activate the report `ZSOLIST` in SE38 using the code in `ZSOLIST_Source_Code.txt`
3. Create Screen 100 with a Custom Control named `SOLIST` in SE51
4. Create PF-Status `SOLIST` and Title Bar `SOL` in SE41
5. Execute the report via SE38 → F8

---

## Technology Stack

- **Language:** ABAP (Advanced Business Application Programming)
- **ALV Class:** `CL_GUI_ALV_GRID` (Object-Oriented ALV)
- **Container:** `CL_GUI_CUSTOM_CONTAINER`
- **DB Tables:** `VBAK`, `VBAP`
- **Screen:** Dynpro (Module Pool) — Screen 100
- **Platform:** SAP ERP / SAP S/4HANA
