# Release Notes

## Version 1.0.4 - Sept 11, 2023

- Refactored for simpler code
- Simplified grid by removing left column subtitles
- Reworded each input to start with a clearer action step desired from the user (i.e. Enter Your Name vs Employee ID)

## Version 1.0.3 - Sept 11, 2023

- Added "THIS IS A PROOF OF CONCEPT WEBSITE NOT INTENDED FOR MEDICAL USE" in bold red font at the top
- Made the disclaimer accordion label in bold, red, all caps font
- Removed patiet name and date of birth
- Added write in space for patient name and date of birth on the PDF
- Added disclaimer acknowledgement checkbox
- Require patient medical record number, residual renal function, date of first vancomycin dose, created by, and disclaimer acknowledgement to generate confirmation box, which leads to generating the PDF
- Updated the disclaimer for data and PDF storage liability mitigation
- Reset all values OnSubmit
- Added a timer to reset form data every 3 minutes
- Per conversation with Anie, updated "Go to Clinic" so that if metric is > 1, then go to clinic on day 2 and not day 3
- Since alert stops the reset timer, removed the alert functionality and replaced it with a feedback message that renders if fields weren't filled in.

## Met with Cybersecurity Team - Step 11, 2023

## Version 1.0.2 - Sept 11, 2023

- Moved “Created by…” and “Created on…” to the top-right of the PDF
- Changed “draw blood level for Vancomycin, “Get follow-up cell count” to “Go to clinic for lab tests”
- Changed “Draw blood level for Vancomycin if dose changes” to “If dose changed, go to clinic for lab tests”
- Fixed January 29,30,31 y coordinate bug
- Refactored getCell.ts
- Added input validation for Residual Renal Function Kt/V and Date of First Vancomycin Dose fields

## Met with Ramiro and Anie - Step 10, 2023

## Version 1.0.1 - Sept 9, 2023

- Issue: Ensure correct patient
- Added Patient Identification Inputs (name, date of birth, and medical record number)

- Issue: Identify who made the schedule
- Added Employee Information Input

- Issue: If multiple schedules from the same person, identify a difference between schedules
- Added a time stamp to the PDF

- Updated to enhance the disclaimer

## Version 1.0.0 - Sept 3, 2023

- Built a PDF generator
- 2 Inputs: Residual Renal Function Kt/V and Date of First Vancomycin Dose
- 1 Output: PDF showing dose schedule and lab tests
- Added a disclaimer
