# Automation Coding Test

## Instructions
* Fork this repo
* Create a framework to perform the following tests
* Push to your forked repo and email me (blubecker@lifesize.com) that you have completed the tests.
* Take a well deserved break!

### Framework Information

For these tests, feel free to use whatever language you are most familiar with. That said, we use Javascript and webdriver.io
for our current projects, so it would be great to see your capabilities with working in that language.

Email me at blubecker@lifesize.com if you have any questions.

## Tests

I am going to use the gherkin syntax (as used in Cucumber) to describe these tests. You are by no means required to use
cucumber in your framework (I sure don't), but it should hopefully give you a clear idea of what to test.

Note: After logging in, you should see 3 text lines: email, url, and phone. Each one should
contain your extension you used when logging in.

### Test 1

```
Given I login to the application with an extension
Then the extension in email, url, and phone text should be the extension I logged in with
```

### Test 2

```
Given I login to the application with an extension
When I click on the build JSON button
Then the extension in email, url, and phone entries in the JSON output should be the extension I logged in with
```

### Bonus Round!

```
Given I login to the application with an extension
When I click on the show chats button
Then I should be able to parse the NEW chats data and return an array of JSON objects like this:

[
  {
    sender: 'User name',
    time: '10:03 PM',
    message: 'hey man, how are you doing?'
  },
  // more json objects...
]
```
