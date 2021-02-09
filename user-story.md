# Frontier Coding Test - Display Sorted Account Info

## Purpose

The business needs a view that displays user accounts by status.

## Feature Description

The new accounts view will display user accounts sorted by status. The view will pull data from the vendor's REST API. Account statuses, due dates and amounts due should be calculated by the vendor. This feature is only for US users, so a currency type of USD can be inferred.

## Scope

A template for the view has been provided, this template can be modified to fit the template engine of the framework generating the view. Responsive design is handled in another unassigned user story, this functionality can be implemented in this story if time permits. The business asks that this user story is time boxed to 1 hour.

## Marketing Notes

- A basic template has been provided using CSS grid and HTML 5. This template can be modified.
- Responsive design is not required at this time, but is considered a nice to have.
- Fields displayed include Name, Email, Phone Number, Amount Due and Payment Due Date
- Phone Number should be formatted as (###)-###-####
- Dates should be formatted as (##/##/####). We have no preference on leading zeros in days and months, but years should display all 4 digits.
- Name should be formatted as $"{LastName}, {FirstName}".
- Amount Due should be formatted as "$###.##" or "$##.##"
- Currency type of USD can be inferred.
- Empty due dates for inactive accounts should hide.

## Developer Notes

- Provided template seems to have issues if the content in the lists overflow into the footer. This is not in the acceptance criteria, but is marked as a known issue. If time permits, this is a nice to have fix.
- This solution should be completed in either vue.js, angular(v2+), react, .NET core, or .NET 5.

## Known  Issues

### Template

- Content overflows from lists into footer causes list content to render underneath the footer rather than pushing the footer down.
- Three column layout causes issues on mobile.

## Acceptance Criteria

- Solution is written in vue.js, angular(v2+), react, .NET core, or .NET 5.
- Accounts appear in the correct column by status
- All 7 Mock Data accounts appear
- Dates, Names, Amounts and Phone Numbers are formatted correctly
- Empty due dates hide field and label
- Data integrity between endpoint and view is preserved.
