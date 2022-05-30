This is a [Next.js](https://nextjs.org/) project bootstrapped with [`create-next-app`](https://github.com/vercel/next.js/tree/canary/packages/create-next-app).

## Getting Started

First, run the development server:

```bash
npm install
npm run dev
# or
yarn dev
```

Open [http://localhost:3000](http://localhost:3000) with your browser to see the result.

## Available validations in each form

1. Active tab:
    - From and To field can't be empty and should be +ve numeric values.
    - Asset drop down can't be empty.
    - Start time should be after the current time.
    - To Time should be after the start time.
    - Maximum submission test:
        - A maximum limit will be placed on the date/times allowed in each submission. From 05:00 to 11:00 local time the Submission Maximum Date is set equal to the end of the current + 4 days. From 11:00 to 05:00 local time the Submission Maximum Date is equal to the end of the current Day + 5 days. (The current day runs from 05:00 to 05:00 local time). If single record within the submission extends beyond the date, display error message: “To Date and Time must before the maximum submission date”.
2. Tomorrow Tab:
    - Asset drop down can't be empty.
    - Verify that the single-sided submission is allowed i.e either offer only or bid only can be submitted.
    - Check that no null values are allowed for offer and Bid value.
    - Offer Price must be greater than Offer Undo.
    - Offer Undo must be greater than Bid Price.
    - Offer Price must be greater then Bid Undo.
    - Offer price and Bid Price should be in greater then equal to -99999 && less than equal to 99999.




Framework Overview
---------------------
1. Framework - Mocha
2. Assertion Library - Chai
3. Design Pattern - Page Object Model

Steps to build and test
--------------------------
1. npm install
2. npm run cy:open (for headed test)
3. npm run cy:e2e:test (for headless execution of api & back-end tests)

Assumptions
-------------
1. Dev and QA team will share the same code repository
2. API and UI tests will use the same framework
3. HTML reports will be published in CI/CD
4. Tests will be running on localhost

Obstacles
-----------
1. No challenges faced


==========How to Run============================
1. Framework used cypress mocha for both frontend and backend 
2. Install nodejs in your system >>>https://nodejs.org/en/download/
3. Verify after install node js installed successfully using example:node -v
4. Install visual sudio code -code editor latest one --https://code.visualstudio.com/
5. Create a folder with Cypressautomation in any drive C or D 
6. Open the cmd with created folder and type npm init  example :  C:\Cypressautomation>npm init
7. Open the project folder in Visual code  project name : SDET_TAKE HOME TEST
8. Make sure Project file directory is up to sdet_test in the  vs code terminal 
9. Type the command in VS code Terminal   >>  npm install cypress --save-dev
10. After install cypress successfully 
11.Type the command   npm run cypress:open  or npx run cypress open or npm run cy:open
12. Cypress.io UI will open with all the testsuits 
13. Run the testcases from the cypress window 
14. If you want to run only frontend case use this command >>npm run cy:frontend:test
15. If you want to run only Backed cases use this command >>npm run cy:cy:backend:test
16. If you want to run all testcases  use this command >> npm run cy:e2e:test




