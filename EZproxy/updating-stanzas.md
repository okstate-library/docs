### Updating and Adding EZproxy stanzas
#### Boundaries
This process begins when a new resource is added to the library's collection and a new stanza is needed or when a current stanza is outdated and causes a catalog configuration error. If a patron or library employee notifies you of a configuration error, the error page lists the URL for the resource.

#### Outputs
Access for off-campus patrons for a given resource via EZproxy.

#### Inputs
- The [Online Computer Library Center (OCLC)](https://help.oclc.org/Library_Management/EZproxy/Database_stanzas) attemps to maintain an up-to-date list of stanzas on their webpage. If a resource's stanza is not listed on OCLC's webpage you will need to [create a new stanza]() yourself.
- Resource URL. The configuration error page will contain a URL for the resource (see below). This is helpful for testing.

![Config Error](https://okstate-library.github.io/docs/EZproxy/example_config_error.jpg)

- Administrative access to EZproxy
- `main_stanzas.txt` from the [GitHub repo](https://github.com/okstate-library/EZproxy)
- Push access to the [GitHub repo](https://github.com/okstate-library/EZproxy)

#### Roles
- EZproxy admin

#### Activities
1. Find the stanza on [OCLC's webpage](https://help.oclc.org/Library_Management/EZproxy/Database_stanzas). If OCLC does not have the stanza, you will need to [create one yourself]().
1. If you are updating a current stanza, locate the stanza in [main_stanza.txt](https://github.com/okstate-library/EZproxy/blob/master/main_stanzas.txt).
1. Edit the content on GitHub by clicking the little pencil at the top, righthand side of [main_stanza.txt](https://github.com/okstate-library/EZproxy/blob/master/main_stanzas.txt).
1. If you are adding a new stanza, copy the OCLC stanza to the beginning of `main_stanzas.txt`. If you are updating a stanza, overwrite the old stanza with the new stanza copied from OCLC.
1. Click the green "Commit changes" button at the bottom (feel free to add a comment).
1. [Download a copy](https://github.com/okstate-library/EZproxy/archive/master.zip) of the GitHub repo.
