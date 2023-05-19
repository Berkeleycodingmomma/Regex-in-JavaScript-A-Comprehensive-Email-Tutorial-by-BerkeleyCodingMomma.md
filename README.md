# Regex-in-JavaScript-A-Comprehensive-Email-Tutorial-by-BerkeleyCodingMomma.md
#
# Matching an Email Regex, Understanding the Components
#
## Description 
I created a tutorial and publised it in a Github gist. Through this tutorial we will consistently refer to the provided regular expression (regex) for the purpose of analyzing each regex component. This approach aims to facilitate a comprehensive understanding for both beginners and experts, ensuring clarity in comprehending the material. The regex components covered in this guide comprise Anchors, Quantifiers, Grouping Constructs, Bracket Expressions, Character Classes, and finally Character Escapes. By thoroughly examining these elements, readers will gain a solid grasp of the topic.
#
## Visual image of the Github gist turorial
#
<img width="1437" alt="Screen Shot 2023-05-18 at 8 02 00 PM" src="https://github.com/Berkeleycodingmomma/Regex-in-JavaScript-A-Comprehensive-Email-Tutorial-by-BerkeleyCodingMomma.md/assets/127444682/6d3bb6d1-cb19-46d7-b408-862d38eeee96">
#

## Technology Used 

| Technology Used         | Resource URL           | 
| ------------- |:-------------:| 
* JavaScript.info - Form Validation: https://javascript.info/forms-validation
This website offers tutorials and examples on JavaScript form validation, including email validation.

#

## Video of the final tutorial
#
* [Youtube](https://youtu.be/3Mm9cNflXwk)
#

## Code examples of the project

#
--------------------------------------------------------------------------------------------------------------------------------------------------------

 ```sh

**Example:** Consider the following email address: `amanda_1278-@berkeleybootcamp.edu`

The local part, of the username, is `amanda_1278-`.

The local part of the email address, representing the username, is amanda_1278-.

Now, let's break it down based on the bracket expression [a-z0-9_\.-]:

- `amanda` consists of lowercase letters a, m, a, n, d, and a, matching the a-z part of the expression.
- `_` is an underscore character, matching the _ part of the expression.
- `1278` consists of digits 1, 2, 7, and 8, matching the 0-9 part of the expression.
- `_`is a hyphen character, matching the - part of the expression.
- `.` is a literal period (dot) character, matching the \. part of the expression.

Therefore, the updated breakdown of the email address amanda_1278-@berkeleybootcamp.edu aligns with the bracket expression and its respective components.

```

**(ABOVE)- 

--------------------------------------------------------------------------------------------------------------------------------------------------------

```sh

  


```

**(ABOVE)- 

--------------------------------------------------------------------------------------------------------------------------------------------------------

```sh

**Example:** Consider the following two email addresses:
1. `amanda.val@bootcamp.edu` **(valid)**
2. `amanda@inval@bootcamp.edu` **(invalid)**

In the regex pattern /^([a-z0-9_.-]+)@([\da-z.-]+).([a-z.]{2,6})$/, we utilize the backslash to escape the dot (.) within the pattern. Specifically, . is employed to match a literal period character within an email address. This approach guarantees the accurate identification of valid email addresses, as demonstrated in the email address amanda.val@bootcamp.edu (valid), while correctly dismissing invalid email addresses, as illustrated in the email address amanda@inval@bootcamp.edu (invalid).

If the dot (.) were not escaped, it would function as a wildcard character, potentially matching any character in its place. Consequently, the regex would erroneously identify invalid email addresses.

By appropriately escaping the dot (.) with a backslash (i.e., .), we establish that the regex only matches valid email addresses that contain literal periods in the appropriate positions. This practice prevents the dot from behaving as a wildcard and ensures more precise pattern matching.

    
```

**(ABOVE)- 

--------------------------------------------------------------------------------------------------------------------------------------------------------

```sh
  




```
**(ABOVE)- 

--------------------------------------------------------------------------------------------------------------------------------------------------------

## Author Info

### Amanda Gray

* [Linkedin](https://www.linkedin.com/in/amanda-gray-831a65254/)
* [Github]()

## Credits

Shout out to all the TA's and Google Search!

GOOGLE!  Seriously, thank you google search!





© 2023 edX Boot Camps LLC. Confidential and Proprietary. All Rights Reserved.










