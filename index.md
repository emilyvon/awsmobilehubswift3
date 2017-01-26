## TL;DR

I have been working as an iOS developer for less than half a year and I was asinged to build an app using AWS as backend. Working with [Firebase](https://firebase.google.com) previously was a breeze - the documentation and the SDK are very easy to use, and dealing with AWS seems like a daunting task when you are in a small team where you are basically on your own.

None of us in the team had used AWS before so we had to work and learn a lot of the services on the go. Before we even knew about the existence of the Mobile Hub, I implemented everything from scratch - from getting the session token from the successful sign-in of the user pool and refresh it manually, to mapping every single object returned from and pushed to DynamoDB, and the models to pesist data on the phone. Figuring out all the Cognito and the DynamoDB stuff is not the easiest task but still doable by looking at the objective-c SDK documentation. The worst part is when the schema has been changed not once but for a few times, doing all the mapping again and again seems to be a total waste of time and a torture to my brain.

Until one day we found out there was something called the [AWS Mobile Hub](https://aws.amazon.com/mobile/). But here comes two problems:
1. if you try to compile the sample project, it gives you at least 80 errors because it's not in Swfit 3. Here's what you would see:
![Image]()

2. if you download the custom source code(helper code), some of the functions in the model classes do not exists.


Without further ado, let's fix the prject!

### To be continued
<!--
Markdown is a lightweight and easy-to-use syntax for styling your writing. It includes conventions for

```markdown
Syntax highlighted code block

# Header 1
## Header 2
### Header 3

- Bulleted
- List

1. Numbered
2. List

**Bold** and _Italic_ and `Code` text

[Link](url) and ![Image](src)
```

For more details see [GitHub Flavored Markdown](https://guides.github.com/features/mastering-markdown/).

### Jekyll Themes

Your Pages site will use the layout and styles from the Jekyll theme you have selected in your [repository settings](https://github.com/emilyvon/awsmobilehubswiftsample.github.io/settings). The name of this theme is saved in the Jekyll `_config.yml` configuration file.

### Support or Contact

Having trouble with Pages? Check out our [documentation](https://help.github.com/categories/github-pages-basics/) or [contact support](https://github.com/contact) and we’ll help you sort it out.
-->
