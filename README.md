# Prison and Inmate Record Management System - Assembly

## Project Overview

The **Prison and Inmate Record Management System** is an assembly language-based project designed to manage basic prison operations such as inmate registration, sentence tracking, cell block assignment, incident reporting, parole checking and inmate transfers.

The system stores inmate records using arrays and applies validation logic to maintain accurate records, prevent duplicate inmate IDs, track cell occupancy and update release dates based on sentence changes or disciplinary incidents.

## Features

### Feature 1: Inmate Intake and Profile Creation

This feature allows the system to register new inmates by storing their basic information, including:

- Inmate ID
- Name
- Age
- Crime category
- Sentence duration

The system stores inmate names and crime categories in arrays and validates inmate IDs to prevent duplicate records.


### Feature 2: Sentence Tracking and Release Date Calculation

This feature calculates the expected release date of an inmate based on the intake date and sentence duration.

A dedicated reusable procedure is used for release date calculation. This procedure is called during:

- Initial inmate intake
- Sentence modification
- Penalty-based sentence extension

The system also flags inmates whose release date falls within the current simulated month.

---

### Feature 3: Cell Block Assignment and Occupancy Management

This feature assigns inmates to cell blocks based on crime severity and available capacity.

The system keeps track of occupancy for each cell block and prevents assigning inmates to a block that has already reached its maximum capacity.

---

### Feature 4: Incident Reporting and Penalty Extension

This feature records disciplinary incidents for inmates.

Each incident is linked to a specific inmate and can extend the inmate's sentence by a defined penalty period. After the penalty is applied, the inmate's release date is updated automatically.

---

### Feature 5: Parole Eligibility Checker

This feature checks whether inmates are eligible for parole based on predefined criteria, such as:

- Minimum required sentence time served
- No recent disciplinary incidents

Eligible inmates are displayed by the system and a parole recommendation list is generated.

---

### Feature 6: Inmate Transfer Between Cell Blocks

This feature processes internal inmate transfer requests between cell blocks.

Before transferring an inmate, the system checks whether the destination cell block has available capacity. If the transfer is valid, the system updates the occupancy records of both the original and destination cell blocks.

## Key Functionalities

- Inmate profile creation
- Duplicate ID validation
- Sentence duration tracking
- Release date calculation
- Cell block assignment
- Cell occupancy management
- Incident recording
- Sentence extension after incidents
- Parole eligibility checking
- Inmate transfer between blocks

## Technologies Used

- Assembly Language
- Array-based data storage
- Procedure-based modular programming
- Conditional branching and validation logic

## Purpose of the Project

The main purpose of this project is to demonstrate how prison and inmate record management operations can be implemented using low-level assembly language concepts. It focuses on structured data handling, modular procedures, validation and logical decision-making.
