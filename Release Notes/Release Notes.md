# Release Notes
>[!IMPORTANT]
> I wrote these release notes few years ago for a software application that is now made redundant due to changes in regulation. I have only used generic information and removed any specific details. The release and ticket numbers used are for reference purpose only and do not have any meaning in real scenario.

## Platform Release Changes - Enhancements
Below is a list of all enhancments that have been included in 2.3.0 release:

### JiraEnhan-001 - File History displays upload history of more days
The File History folder has been enhanced to now display the uploaded history for 180 days. Previously, it was set to display history for just 90 days.

### JiraEnhan-002 - True/False values displayed in Complete Reports and Current Report columns
Folders will now display True/False values for Boolean field, which is consistent to the XML output.
This is applied to both Complete Reports and Current Reports columns.

### JiraEnhan-003 - XXX Validations - Enhanced validation details in GUI error message
The error message displayed on the error screen when the 'validate' button is clicked has been enhanced for xxx validation exceptions. This error message now includes field names that the error is referring to.

## Platform Release Changes - Defect Fixes
### JiraDefect001 - XXX Validations Error When the Fund has no Reporting Requirement
**Issue**

xx validation assumes that the mandatory fields within the funds are populated. However, when reporting for a fund that has no reporting requirement for a period, you need to only populate the header section.
Currently, a FCA validation error is displayed when the mandatory fields of a fund with no reporting requirement are left blank.

**Resolution**

The xxx validation is now amended, which has fixed this issue. 

### JiraDefect002 - Rates Static Lookup
**Issue**
The Rates static table is referred to in the creation of number of fields. Currently, it is linked via the date equalling the last day of the reporting period. However, the static table only has rates for weekdays. 
**Resolution**
The code has been changed, such that if the last day of a reporting period is a weekend, the last week of the reporting period is used.



