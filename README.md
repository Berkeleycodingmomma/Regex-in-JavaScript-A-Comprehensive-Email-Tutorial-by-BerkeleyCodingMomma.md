# Regex-in-JavaScript-A-Comprehensive-Email-Tutorial-by-BerkeleyCodingMomma.md
#
# Matching an Email Regex, Understanding the Components
#
## Description 
I created a tutorial and publised it in a Github gist. Through this tutorial we will consistently refer to the provided regular expression (regex) for the purpose of analyzing each regex component. This approach aims to facilitate a comprehensive understanding for both beginners and experts, ensuring clarity in comprehending the material. The regex components covered in this guide comprise Anchors, Quantifiers, Grouping Constructs, Bracket Expressions, Character Classes, and finally Character Escapes. By thoroughly examining these elements, readers will gain a solid grasp of the topic.
#
* [Github Gist Link](https://gist.github.com/Berkeleycodingmomma/851fe71eee01ee7483f2a8c3efdcaeb7)

## Visual image of a "raw" portion of the Github Gist turorial
#

<img width="1437" alt="Screen Shot 2023-05-18 at 8 02 00 PM" src="https://github.com/Berkeleycodingmomma/Regex-in-JavaScript-A-Comprehensive-Email-Tutorial-by-BerkeleyCodingMomma.md/assets/127444682/6d3bb6d1-cb19-46d7-b408-862d38eeee96">

#

## Technology Used 

| Technology Used         | Resource URL           | 
| ------------- |:-------------:| 
* JavaScript.info - Form Validation: https://javascript.info/forms-validation
This website offers tutorials and examples on JavaScript form validation, including email validation.
* McGill University. (n.d.). Teaching and Learning Services - Teaching Dossier: https://www.mcgill.ca/tls/teaching-dossiers
This website provides resources and guidance on creating teaching dossiers.
* Regular-Expressions.info - Regex Tutorial: https://www.regular-expressions.info/
Regular-Expressions.info offers comprehensive tutorials and examples on regular expressions, covering a wide range of topics.
* OpenRefine Tutorial - Regular Expressions (Regex) Activity: https://datacarpentry.org/openrefine-socialsci/05-regex/
Data Carpentry provides a tutorial on using regular expressions with OpenRefine, similar to the University of Toronto Libraries' tutorial.
* Purdue University. (n.d.). Oral Presentation Tips: https://owl.purdue.edu/owl/subject_specific_writing/professional_technical_writing/technical_presentations/index.html
Purdue University's Online Writing Lab (OWL) offers tips and advice on delivering effective oral presentations, similar to the University of Toronto's Advice on Academic Writing page.
* freeCodeCamp. (n.d.). Web Design - CS50's Web Programming Course: https://www.freecodecamp.org/news/cs50s-web-programming-course/
freeCodeCamp provides a web programming course similar to CS50's Web Programming with Python and JavaScript from Harvard University.

#
## Video Preview link of the final tutorial
#
* [Youtube](https://youtu.be/3Mm9cNflXwk)
#

## Examples of the "raw" Github Gist
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

--------------------------------------------------------------------------------------------------------------------------------------------------------

```sh

**Example:** Consider the following two email addresses:
1. `amanda.val@bootcamp.edu` **(valid)**
2. `amanda@inval@bootcamp.edu` **(invalid)**

In the regex pattern /^([a-z0-9_.-]+)@([\da-z.-]+).([a-z.]{2,6})$/, we utilize the backslash to escape the dot (.) within the pattern. Specifically, . is employed to match a literal period character within an email address. This approach guarantees the accurate identification of valid email addresses, as demonstrated in the email address amanda.val@bootcamp.edu (valid), while correctly dismissing invalid email addresses, as illustrated in the email address amanda@inval@bootcamp.edu (invalid).

If the dot (.) were not escaped, it would function as a wildcard character, potentially matching any character in its place. Consequently, the regex would erroneously identify invalid email addresses.

By appropriately escaping the dot (.) with a backslash (i.e., .), we establish that the regex only matches valid email addresses that contain literal periods in the appropriate positions. This practice prevents the dot from behaving as a wildcard and ensures more precise pattern matching.

    
```

--------------------------------------------------------------------------------------------------------------------------------------------------------

```sh
  
### Escape sequences: 
In order to represent characters that cannot be directly typed or represented in a string, we use escape sequences. These sequences begin with a backslash () followed by one or more letters. In the context of the email regex, the escape sequence \d is used to represent any digit from 0 to 9. It acts as a shorthand notation for the character class [0-9]. By utilizing escape sequences, we can conveniently include these special characters in our regular expressions.

**Example:** Consider the following email addresses:
1. `amanda.val2023@bootcamp.com` **(valid)**
2. `amanda123_val@bootcamp.com` **(valid)**
3. `aval@bootcamp7.com` **(valid)**
4. `amanda.val@2023bootcamp.com` **(invalid)**

Throughout the example, the regex accurately matches valid email addresses that contain digits, such as the 1st, 2nd, and 3rd email addresses mentioned above. The use of the escape sequence \d allows the regex to represent any digit from 0 to 9, serving as a shorthand notation for the character class [0-9]. This enables the regex to identify valid email addresses containing digits in both the username and domain parts.

However, the 4th email address, amanda.val@2023bootcamp.com, is considered invalid because it starts with a digit immediately after the @ symbol. This violates the regex pattern provided, which does not allow domain names to start with a digit. Therefore, the regex fails to match the 4th email address and labels it as invalid.


```

--------------------------------------------------------------------------------------------------------------------------------------------------------

## Author Info

### Amanda Gray

* [Linkedin](https://www.linkedin.com/in/amanda-gray-831a65254/)
* [Github]()
* [Github-Gist](https://gist.github.com/Berkeleycodingmomma/851fe71eee01ee7483f2a8c3efdcaeb7)

## Credits

Shout out to all the TA's and Google Search!

GOOGLE!  Seriously, thank you google search!





© 2023 edX Boot Camps LLC. Confidential and Proprietary. All Rights Reserved.










