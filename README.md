### NewFlowBuilder
Resources for the new SF Flow Builder


Intend:

Self-learning of the new flow builder specially loops and record choice sets (that allows you to select dynamically between records based on certain criteria).

Test a business case: guide user thoroughly to prevent them from creating duplicate contacts and/or accounts. If contacts are already existing using some matching criteria defined by the business case, let them select which one they want to update. If multiple accounts are found with the entered account name, provide them a list where they can pick the right account. If the account doesn't exist, create the account as well.

In all cases provide the user a way to exit the procedure at contact creation/update and account creation or selection. Provide them also a way to start again from scratch.

 

This is how it looks like:

No alt text provided for this image
Lessons learned:

-use screen element to debug your flow (especially to make sure your variables values are correct). Keep them afterward as disconnected elements should you want to update your flow. Start their labels with "Debug".

-if you use counter in loops, set them first to zero using an assignment screen. I find it more handy to handle in decision screens, ie count = 0 instead of "count" "is null" "globalcontstanttrue".

-remember that if a field is mandatory at page layout level, your flow will still work if you ignore it (but it would be a good idea to integrate that field in your flow)

-you are going to end up with a lot of choices, decision outcomes, variables and screen components. Make sure you use a consistent naming convention otherwise you are going to end up quite confused by what you’ve created. For the screen components especially, use two strings (at least) to differentiate between user inputs vs pure explanation texts (I used Inp_ vs Txt_ in the api name...)

-if you are using record choice set, create a formula that concatenates several meaningful fields for the users, so that he can choose between records clearly. Natively, record choice set allows you to use only one field to display, so in my contact selection process, I've concatenated first name, last name, account name, email and birthday.

 

Conclusions:

The flow tool is extremely powerful but it takes some times to understand and can be quite frustrating at first. I took a very good course on Udemy, but unfortunately it's on the old version. That course will still allow you to understand the general principles governing flow creation. I found the new version much simpler to use and it allowed me to create business process that I could never imagined before. So if you are looking for a way to automate furthermore those for your clients and you are not a programmer, I would definitively take a closer look to the new flow builder.

If you like this article, please also vote for those great flows builder ideas…

https://success.salesforce.com/ideaView?id=0873A000000CZGZQA4

https://success.salesforce.com/ideaView?id=08730000000l2hoAAA

https://success.salesforce.com/ideaView?id=08730000000ZWp7AAG

https://success.salesforce.com/ideaView?id=08730000000ku4TAAQ

https://success.salesforce.com/ideaView?id=08730000000keEFAAY

https://success.salesforce.com/ideaView?id=0873A000000ECGHQA4

https://success.salesforce.com/ideaView?id=0873A0000003cNMQAY

https://success.salesforce.com/ideaView?id=0873A000000EDKpQAO

https://success.salesforce.com/ideaView?id=0873A000000CYQ1QAO

https://success.salesforce.com/ideaView?id=0873A000000ECokQAG

https://success.salesforce.com/ideaView?id=0873A0000003c11QAA

https://success.salesforce.com/ideaView?id=0873A0000003cL1QAI

https://success.salesforce.com/ideaView?id=0873A000000EC6kQAG
