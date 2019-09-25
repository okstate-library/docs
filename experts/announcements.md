### Announcements

##### Background
The *Announcements* page provides announcements and updates on the Experts Directory. The implementation team will endeavor to provide weekly updates on this page.

##### Implementation
Announcements are posted on the [Experts Directory website](https://info.library.okstate.edu/experts). Content is stored in a [GitHub page](https://github.com/okstate-library/experts-website/blob/master/content/announcements.html).

#### Boundaries
When it's time for a new announcement.

#### Inputs
- Administrative access to the Experts LibGuide.
  - Announcements are posted on the [Experts Directory website](https://info.library.okstate.edu/experts).
- Push access to the [html file](https://github.com/okstate-library/experts-website/blob/master/content/announcements.html) on GitHub.
- The preview page hosted on [GitHub](https://okstate-library.github.io/experts-website/content/announcements). This page will not have all the styling as the live site hosted on LibGuides. The content administrator can check content here and change it within GitHub before pushing it onto the live site.

#### Roles
- Content Administrator: This person keeps the announcements up to date.
- Site Administrator: This person copies HTML from GitHub into the appropriate widget in the LibGuide.

`The entire workflow can be completed by one person if they have write priveledges in both LibGuides and GitHub.`

#### Activities
1. The content administrator updates the file on GitHub.
1. The content administrator notifies the site administrator there is new content.
1. The site administrator copies the HTML into the widget on the LibGuide.

#### Adding Rows
1. The content administrator posts a new announcement on GitHub.
1. The content administrator notifies the site administrator of new content.
1. The site administrator pastes the HTML from GitHub onto the appropriate widget on LibGuides.

##### HTML Syntax

The HTML Syntax for the announcements is as below. The most recent announcement goes at the top of the list. Add the three-part announcement enclosed in `<li></li>` tags just before the topmost list item.

```html
<div class="container mt-5 mb-5">
	<div class="row">
		<div class="col-md-6 offset-md-3">
			<h4>Latest Announcements</h4>
			<ul class="timeline">
				<li>
					<h5>TOP ANNOUNCEMENT HERE</h5>
					<h6>DATE</h6>
					<p>TEXT</p>
				</li>
				<li>
					<h5>NEXT ANNOUNCEMENT DOWN</h5>
					<h6>DATE</h6>
					<p>TEXT</p>
				</li>
				<li>
					<h5>THIRD ANNOUNCEMENT DOWN</h5>
					<h6>DATE</h6>
					<p>TEXT</p>
				</li>
			</ul>
		</div>
	</div>
</div>
```
