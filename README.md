# cyber-project
Project: Password Strength Checker
Objective
To check how strong a password is based on several criteria, such as:
-Length
-Use of lowercase letters
-Use of uppercase letters
-Inclusion of numbers
-Inclusion of special characters

------Code Explanation
import re

This imports the regular expressions module to check for specific character patterns.
Function check_password_strength(password)
Takes a password string and checks it against 5 criteria using regular expressions.

------Criteria Checked:
length_error: Checks if the password has at least 8 characters.
lowercase_error: Uses re.search to look for at least one lowercase letter.
uppercase_error: Looks for at least one uppercase letter.
digit_error: Checks for digits.
special_char_error: Looks for special characters.
Score Calculation:
Subtracts the number of failed checks from 5 to get a score from 0 to 5.
Strength Classification:
Based on the score, the password is labeled from "Very Weak" to "Very Strong".
Return Value:
A dictionary with the score, the strength, and details about each rule.
