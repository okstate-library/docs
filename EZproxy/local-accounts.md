### Creating Local Accounts
EZproxy uses OSU's central authentication to authenticate most of its users. For special case, e.g., temporary programs or students in remote programs, etc., we create local users.

#### Boundaries
The process begins when a patron who does not have typical OKEY credentials needs access to library resources.

#### Outputs
Local accounts in EZproxy and temporary accounts in Alma. A user should use the same username and password across all library resources.

#### Inputs
1. Access to EZproxy's `LocalAccounts.txt` file.
2. A role in Alma that allows for the creation of temporary accounts.

#### Roles
- EZproxy administrator
- Program coordinator
  - There are currently several different programs that need this service including GPIDEA and the Ph.D. in Business for Executives program.

#### Activities

```
For this process, all activities are done by the EZproxy administrator.
```

1. Obtain the list of new users and associated email addresses from the respective program coordinator.
2. Create an Excel spreadsheet with the following columns: first (name), last (name), email/username, and password.
3. Use the users' email address as their username.
4. Use a password generator to generate secure passwords and put them in the sheet.
5. Begin a new section at the end of the `LocalAccounts.txt` file by creating a comment. This consists of a `#` character followed by an easy-to-understand description, e.g., "# Local accounts Fall 2019 Exec PhD candidates." Follow this line with your initials in parenthesis, so others know who created the entry.
6. Below this opening line, create a line for each user with the following format: `<username>:<password>:IfBefore=<date access ends>`. Do not type in `<` or `>`. This is my notation telling you to type the content enclosed within those brackets.
7. Restart EZproxy. See the head of the DRDS department for the URL where EZproxy can be restarted.
8. Log into Alma and click on the following menus: *Fulfillment*, *Manage Patron Services*. Complete steps nine through nineteen for each new user.
9. Click *Register New User*.
10. Enter the user's first and last names.
11. Change the *Primary identifier* to the user's EZproxy username.
12. Select *Stillwater* for *Campus*.
13. Select *AFFILIATEZ* for the *User group*.
14. Set both the *Expiration date* and *Purge date* to the last day the user has access.
15. Set the user's password to the same as their EZproxy password. **Manually type in the password to both password fields. Alma will grab extra characters from the clipboard if you try to copy and paste the password into these fields.**
16. Check *School* under *Email types* and enter the user's email address.
17. Check *School* under *Address types* and enter `Distance Learning` in *Address line 1*.
18. Click *Update User*.
19. Click *Done*.
20. Password protect the Excel file using a password made with a password generator.
21. Place the file's password in an encrypted LastPass file for safe keeping.
22. Email the usernames and passwords to the program coordinator.
23. Call the program coordinator and tell them the password over the phone.
