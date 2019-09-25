### Modifying the *What Goes Where* Table

##### Background
The *What Goes Where* table provides a list of scenarios for researchers to determine how to label different academic outputs when entering the information into the Experts Directory. This allows for consistent reporting of data across all OSU departments. The table has three columns: *Professional Activity*, *Activity Type*, and *Field*. The first column contains descriptions of different activities done by researchers at OSU. The second column gives the general category that activity falls under. The third column contains the field the researcher should use within the Elements software to report that activity.

##### Implementation
The table is on the Experts Directory website in the [documentation section for researchers](https://info.library.okstate.edu/expert-researcher). It implements the [Bootstrap HTML Table](https://examples.bootstrap-table.com/#welcomes/from-html.html).

#### Boundaries
Whenever entries in the table need to be added or changed, someone can edit the file on GitHub. This keeps the table version controlled. It also allows editors to roll back changes. HTML is pasted from GitHub to the LibGuide widget on the Experts site.

#### Outputs
An updated *What Goes Where* table.

#### Inputs
- Administrative access to the Experts LibGuide.
  - The table is on the Experts Directory website in the [documentation section for researchers](https://info.library.okstate.edu/expert-researcher).
- Push access to the [html file](https://github.com/okstate-library/experts-website/blob/master/content/what-goes-where.html) on GitHub.
- [Preview page](https://okstate-library.github.io/experts-website/content/what-goes-where). The table will not have all the styling it has on the live website hosted through LibGuides. The content administrator can check content changes here before notifying the site administrator that the live site needs to be updated.

#### Roles
- Content Administrator: This person keeps the html table up to date on GitHub.
- Site Administrator: This person copies HTML from GitHub into the appropriate widget in the LibGuide.

`The entire workflow can be completed by one person if they have write priveledges in both LibGuides and GitHub.`

#### Activities
##### Updating Table
1. The content administrator updates the file on GitHub.
1. The content administrator notifies the site administrator there is new content.
1. The site administrator copies the HTML into the widget on the LibGuide.

#### Adding Rows
When adding a row to the HTML table, please use the following syntax so the search capability works properly.

```html
<tr id="tr-id-ROWNUMBERHERE" class="tr-class-ROWNUMBERHERE">
      <td id="td-id-ROWNUMBERHERE" class="td-class-ROWNUMBERHERE">
        PROFESSIONAL ACTIVITY HERE
      </td>
      <td>CATEGORY HERE</td>
      <td>FIELD HERE</td>
    </tr>
```
