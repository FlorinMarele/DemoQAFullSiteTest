# DemoQA_Full_Site_Test
This is a personal project where I practice testing the demoqa.com website

1. DemoQA – manual testing (in progress)

Manual testing of the practice website demoqa.com, done the way I would approach a real web application: test plan first, then test cases, execution, and documentation of the results.

Current stage: the Text Box component (demoqa.com/text-box) is tested. I'm continuing with other parts of the site, and the plan is to automate the stable flows afterwards (see the roadmap below).

What's in the test plan:

Scope: what is and isn't tested, and what each group of tests checks
Test environment: Windows 11, Chrome 140
42 test cases with ID, title, description, preconditions, steps, test data, expected result, actual result, status, severity, proof (screenshot) and notes
Coverage: field display, order and focus, valid and invalid input, short and long input, special and unusual characters, email validation, submit speed, and basic SQL/HTML injection checks

Results so far (updated 7 November 2026):

Status	Count
Pass	32
Failed (deviation from my expected result)	6
Blocked	1
In progress	3
Total	42

Findings (all severity Low):

Test case	What I observed	Screenshot
TC05	Submitting empty fields registers nothing and shows no message	TC05
TC11	A name with symbols (^@%) is accepted	TC11
TC14	A name with digits (J0hn D03) is accepted	TC14
TC33	A random string of letters and numbers is accepted as a name	TC33
TC36	Same as TC33, together with a Current Address	TC36
TC37	Same as TC33, together with a Permanent Address	TC37


Roadmap
 Test plan and test cases for the DemoQA Text Box component
 Execution and documentation of results, with screenshots
 Finish the remaining test cases (TC38–TC40)
 Extend manual testing to other DemoQA components
 Automate the stable flows with Selenium
 Basic API checks with Postman, where the site offers an API

 GitHub shows .xlsx files only as downloads, so a read-only copy of the test plan is also available here: https://docs.google.com/spreadsheets/d/1__8-OPU5JGfSdVEcj3f6s8EWY-yvnH-JPpj6VzmVVPw/edit?gid=0#gid=0
