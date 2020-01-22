### Creating Local Accounts
EZproxy uses OSU's central authentication to authenticate most of its users. For special case, e.g., temporary programs or students in remote programs, etc., we create local users.

#### Boundaries
The process begins when a patron does not have OKEY credentials and needs access to library resources.

#### Outputs
This process produces local accounts in EZproxy and temporary accounts in Alma. A user should use the same username and password across all library resources.

#### Inputs
1. Access to EZproxy's `LocalAccounts.txt` file.
1. A role in Alma that allows for the creation of temporary accounts.
1. The Python script `local_accounts.py` from [this repository](https://github.com/okstate-library/local_accounts).

#### Roles
- EZproxy administrator
- Program coordinator
  - There are currently several different programs that need this service including GPIDEA and the Ph.D. in Business for Executives program.

#### Activities

```
For this process, all activities are done by the EZproxy administrator.
```

#### Setting Up Accounts
1. Obtain the list of new users and associated email addresses from the respective program coordinator. This is usually provided as an Excel spreadsheet.
1. Using Excel, create the following columns (all lower-case): `first`, `last`, and `email`. Delete other columns.
1. Save the Excel file as `local.csv`. Use this exact (all lower-case) name and make sure to save in CSV format.
1. Download the Python script `local_accounts.py` from [this repository](https://github.com/okstate-library/local_accounts).
1. Place `local.csv` and `local_accounts.py` in the same directory and run `local_accounts.py` with a Python3 interpreter.
1. When prompted, input the appropriate values. The script will ask for your initials, the name of the program (GPIDEA, Executive Ph.D. Program, etc.), the expiration year (four-digit year when the temporary account ends), the expiration month (two-digit month when the temporary account ends), and the expiration day (two-digit day when the temporary account ends).
1. The script will produce three files in the directory: `alma_accounts.csv`, `ezproxy_accounts.txt`, `special_accounts.csv`.
1. Open `ezproxy_accounts.txt` in a plain-text editor and copy the contents to the end of the `LocalAccounts.txt` file on the EZproxy server. Accounts are entered using the following format: `<username>:<password>:IfBefore=<date access ends>`.
1. Remove old accounts from `LocalAccounts.txt` that have already expired.
1. Restart EZproxy
1. Log into Alma and click on the following menus: *Fulfillment*, *Manage Patron Services*.
1. Open `alma_accounts.csv` and use the values to complete the following steps for each user **(Manually type in the password to both password fields. Alma will grab extra characters from the clipboard if you try to copy and paste the password into these fields.)**:
1. Click *Register New User*.
1. Enter the user's first and last names.
1. Change the *Primary identifier* to the user's EZproxy username.
1. Select *Stillwater* for *Campus*.
1. Select *AFFILIATEZ* for the *User group*.
1. Set both the *Expiration date* and *Purge date* to the last day the user has access.
1. Type the user's password. **Manually type in the password to both password fields. Alma will grab extra characters from the clipboard if you try to copy and paste the password into these fields.**
1. Check *School* under *Email types* and enter the user's email address.
1. Check *School* under *Address types* and enter `Distance Learning` in *Address line 1*.
1. Click *Update User*.
1. Click *Done*.

#### Clean Up
1. Do a spot check by randomly picking several accounts and testing that they work in both [Primo Affiliated Users](https://okla-am.hosted.exlibrisgroup.com/pds?func=load-login&pds_handle=&calling_system=primo&institute=01OKSTATESTILL_OKSTAT&url=https://okla-am.hosted.exlibrisgroup.com:443/primo_library/libweb/pdsLogin?targetURL=https%3A%2F%2Fokla-am%2Ehosted%2Eexlibrisgroup%2Ecom%2Fprimo-explore%2Faccount%3Fvid%3DOKSTAT&section=overview&lang=en%5FUS&from-new-ui=1&authenticationProfile=PDS+Stillwater) and [EZproxy](https://library.okstate.edu/using-the-library/anywhere-library-access).
1. Open `special_accounts.csv` in Excel.
1. The CSV contains passwords. Use Excel to save the sheet as a password-protected Excel sheet.
1. Save the master password for the sheet in a password manager for safe keeping.
1. Email the password-protected sheet to the program coordinator.
1. Call the program coordinator and give them the password over the phone.
1. Destroy old copies of CSVs and Excel Sheets.
