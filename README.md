# A list of ideas/bullet points of what should be tested in monefy application. A list of test cases is representing the app structure. Every statement is a test.

When aplicable, the test cases are sorted by the priority.
| Priority      | Description      |
| ------------- |:----------------:|
| 🔥            | Topmost priority |
| 🛑            | High priority    |
| 🟡      | Normal priority  |
| 🟢         | Low priority  |

Note: From my understanding, the fields: "sum input", "date", "add note" in the "New Income", "New Expense" and "New Transfer" are the same fields, implemented in the same way. If that's the case, the then in order to avoid repeated test cases, it is necessary to conduct a number of checks of these fields only in the screens listed below.

### Checks for sum input field 🛑:
- An attempt to enter a negative value in the input field, for example - 55
- Values with + , for example +74
- Floating point numbers for example 99.9
- Entering the maximum number of characters
- Entering a zero value
- Entering the minimum number of characters
- Attempt to insert alphabetic characters
### Checks for add notes field 🛑:
- Entering the maximum number of characters
- Entering the minimum number of characters
- Entering special characters
- Entering numbers
### Checks for date field 🛑:
- Selection of the past date in the calendar
- Selection of a future date in the calendar
- Selection of the current date
### Also in the "New income" and "New expense" screens, if the choose category field is implemented the same way, then only on one of these screens it is necessary to perform the following check of this field 🟡:
- Pressing the button + selecting another category (Checking that when selecting another category, a screen is displayed with an offer to purchase the PRO version, since this function is only available for PRO users)

### Application Installation
- After downloading the application from the Apple Store / Google Play, the application is successfully installed, after clicking on the application icon, it starts and the onboarding screen opens. 🛑

### Onboarding 🛑:
- When opening the application, the "Get started" screen is displayed
-  Checking the "Privacy Policy" and "Terms" of Use links on the PRO Version purchase offer screen


## The main screen of the application:

### Balance:
- Balance button display (Balance button should display current balance positive/negative; with currency; display two decimals)🔥
- Go to the balance section by pressing the "Balance" button on the main screen 🛑
- Display of transaction history  🛑
- Closing the balance curtain by swiping down/ or pressing the expand balance screen button 🛑
- Sorting the balance history by date rate 🟡
- Sorting the balance history by category 🟡
- When clicking on an item from the history of the balance list, checking that a description of the income/expense received opens 🟡


### Left side menu filters :
- Opening the left side Filter menu by swiping to the left/clicking on the filter button in the upper left corner 🛑
- Changing the Cash/ Payment Card / All accounts account (checking that when you change the account on the main screen in the upper left corner, it changes in the side filters too) 🛑
- Change the balance display for the selected time 🛑
    - Day
    - Week
    - Month
    - Year
    - All
    - Interval
    - Choose Date

### Right side menu:
-  Opening the right side menu.(by swiping to the right/clicking on the vertical colon in the upper right corner)🛑

### New screen transfer:
- Check that when you press the button with two arrows on the main screen, the new translation screen opens 🛑
- Transfer from Cash -> Payment Card 🛑
- Transfer from Payment Card -> Cash 🛑
- Cancel a new transfer by clicking on the "Cancel" button 🛑
- Opening the keyboard 🟡
- Closing the keyboard by clicking on the arrow in the upper left corner 🟡
- Checking that after adding a new transfer, the transfer icon is displayed on the main screen (it should be displayed for the date that was specified when creating the new transfer) 🟡

### Interaction with categories on the home screen:
- Adding a new expense by clicking on the category icon 🛑
- Opening the category history by clicking on the color-highlighted area in the pie chart 🛑
- Checking the display of category icons around the chart 🟡


### Pie chart (Checking the correct construction of the pie chart):
- After adding a new expense, the chart is filled in and painted in a certain color 🟡
- When you click on a certain color section of the chart, a category is highlighted and the name of the category and the amount of costs are displayed in the middle of the chart 🟡
- The category and the colored section of the diagram are the same color 🟢

### Adding «New income» from main screen:
- Adding income by clicking on the "+" button 🔥
- Cancellation of income creation by clicking on the "Cancel" button 🟡 

### Adding an «New expense»:
- Adding an expense by clicking on the "-" button 🔥
- Cancellation of the expense creation by clicking on the "Cancel" button 🟡

### Search:
- Search by name 🛑
-  Closing the search bar by clicking on the Cancel button 🛑
- Deleting a previously entered value from the search bar by clicking on the "X" button 🛑
- Search using special characters/numbers/letters.  🟡
- Attempt to search by entering an empty value in the search bar 🟡
- Search by one character 🟡
- Entering the maximum number of characters in the search bar 🟡



## Left side menu:
### The "Categories" section:
- Opening the list of categories 🛑
- Closing the list of categories 🛑
- Editing the category name 🛑
- Deleting a category 🛑
- Cancellation of category deletion 🛑
- Disable/Enable categories (after you disabled a category it should appear in the list in gray font) 🛑
- Merge categories 🛑

### Accounts section:
- Opening the accounts section 🔥
- Adding a new account 🔥
- Adding a new account with Enabled/ Disabled switch "Included in the balance" 🛑
- Account deletion 🛑
- Add new transfer 🛑
- Checks for fields on the "New account" screen: 🟡
  - Entering the maximum number of characters in the name field 🟡
  - Leave the name field empty and try to create an account 🟡
  - Enter the maximum value/minimum value in the Initial account balance field
- Checks for date field 🟡:
    - Selection of the past date in the calendar
    - Selection of a future date in the calendar
    - Selection of the current date
- Cancellation of account creation 🟡
- Creating an account with an existing name 🟡

## Settings:
### Balance:
- Enabling/ Disabling Budget mode 🛑
- Enabling/ Disabling Carry Over 🛑
- Enabling/ Disabling Future recurring records 🛑
### General settings:
- Changing the language 🛑
- Change First day of week 🛑
- Change First day of month 🛑
  - Review application 🛑
- Export to file 🛑
- Create data backup 🛑
- Restore data 🛑
- Clear data 🛑


### Сases related to the PRO version:
- After passing the onboarding, a screen is displayed with an offer to purchase the PRO version 🔥
- Purchase of the Pro version via the settings menu 🔥
- Adding a schedule when creating an expense (after clicking on the add button, a screen with an offer to purchase the PRO version should be displayed) 🔥
- Adding a schedule when creating income (after clicking on the add button, a screen with an offer to purchase the PRO version should be displayed) 🔥
- Enabling Dark theme (After clicking on the Dark theme checkbox, the offer screen to become a PRO user should be displayed) 🟡
- Passcode protection (After clicking on Passcode protection, the offer screen to become a PRO user should be displayed) 🟡
- Currency change (After clicking on the Exchange rate button, the offer screen to become a PRO user should be displayed) 🟡
- Opening the Currencies section (After clicking on the Currencies section, the offer screen to become a Pro user should be displayed) 🟡
-  Adding income through the categories section (When you try to add income through the categories section, a screen with an offer to purchase the PRO version should be displayed) 🟡
-  Adding expense through the categories section (When you try to add expense through the categories section, a screen with an offer to purchase the PRO version should be displayed) 🟡
- SYNCHRONIZATION (When you try to enable synchronization with Google Drive Dropbox, the offer screen to purchase the PRO version should be displayed) 🟡



### List of bugs:  
1. If the account name is too long more than 50 characters, then it is not shortened in the side menu of filters 
2. In the search results, if the note had a long description of more than 50 characters, then it is also not abbreviated "..." in the search results
3. When changing the language of the application, if it is not reloaded, some of the elements are translated and some are not.
4. In the calendar, the month title is not placed in the center of the calendar, but is shifted to the left.
5. When entering the maximum number of characters in sum field and dividing it by two, the result is always 0, for example, if you enter 99999999/2 = 0. 
6. Drop down lists "First day of week", "First day of month" should have titles in the title.
7. You can choose the first day of the month on the 31st day, but there is not always a 31st day in the month. What will happen if there are 30 days in the month? There are no notifications for the user in this case. 
8. If there is too large a number in the pie chart, for example 9,867,281,515.91, then the currency is not separated from the amount there are no spaces rub9,867,281,515.91.
