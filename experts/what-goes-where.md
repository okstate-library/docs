### Modifying the *What Goes Where* Table

##### Background
The *What Goes Where* table provides a list of scenarios for researchers to determine how to label different academic outputs when entering the information into the Experts Directory. This allows for consistent reporting data across all OSU departments. The table has three columns: *Professional Activity*, *Activity Type*, and *Field*. The first column contains descriptions of different activities done by researchers at OSU. The second column gives the general category that activity falls under. The third column contains the field the researcher should use within the Elements software to report that activity.

##### Implementation
The table is on the Experts Directory website in the [documentation section for researchers](https://info.library.okstate.edu/expert-researcher). It implements the [Bootstrap Flat Json Table](https://examples.bootstrap-table.com/#welcomes/flat-json.html#view-source). The HTML providing the table structure is on the LibGuide itself while the table contents are stored in a [JSON file](https://okstate-library.github.io/what-goes-where/whatgoeswhere.json) on GitHub. This implementation allows for live updating of the table as the project grows. **If the three-column structure of the table itself needs to be changed, this requires rewriting the JSON file and editing the html on the LibGuide.**

#### Boundaries
Whenever entries in the table need to be added or changed, someone can edit the JSON file on GitHub.

#### Outputs
Changes are automatically pushed to the *What Goes Where* table once the user refreshes their browser.

#### Inputs
A correctly formatted JSON file containing the table's contents. Formatting should follow the example below.

**JSON Formatting Example**
```json
```

#### Roles
There are potentially two roles. One person can keep the table's contents up to date by modifying the file on GitHub. A second person can serve as the implementation administrator, updating the Bootstrap table implementation when needed.

#### Activities
