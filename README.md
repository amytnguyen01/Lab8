# Lab8_Starter

## Check your understanding q's (FILL OUT)
1. In your own words: Where would you fit your automated tests in your Bujo project development pipeline? (just write the letter)

2. Would you use a unit test to test the “message” feature of a messaging application? Why or why not? For this question, assume the “message” feature allows a user to write and send a message to another user.

No, we would not use a unit test to test the "message" feature of a messaging application. The reason why is because the messaging feature is likely to consist of many smaller parts that should be tested individually. The point of unit testing is to test individual, smaller components.

3. Would you use a unit test to test the “max message length” feature of a messaging application? Why or why not? For this question, assume the “max message length” feature prevents the user from typing more than 80 characters

Yes, I would use a unit test to test the "max message length" feature of a messaging application. This is because this feature likely does not consist of multiple components and is a smaller component of the program. Therefore, a unit test would be a good way to test this because the test can be measured easily. 

4. What do you expect to happen if we run our puppeteer tests with the field “headless” set to true?

If we run our puppeteer tests with headless set to true, that means the tests will run without opening the browser UI. 

5. What would your beforeAll callback look like if you wanted to start from the settings page before every test case?

beforeAll(async () => { await page.goto('http://127.0.0.1:5500'); await page.waitForTimeout(500); await page.click('img'); });
