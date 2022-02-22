# homepage

Jinntec Homepage

## Content

### Where to find the right markdown files...

| Content                   |      Path                                                                     | 
| ------------------------- | ----------------------------------------------------------------------------- |
| menu                      | `config/_default/params.toml`, `english/contact.md`, `german/contact.md`      |
| contact, logo             | `config/_default/menus.en.toml`, `config/_default/menus.de.toml`              |
| home                      | `english/_index.md`, `german/_index.md`                                       |
| about                     | `english/about.md`, `german/about.md`                                         |
| digital-editions          | `english/_index.md`, `german/_index.md`                                       |
| publishing                | `english/publishing.md`, `german/publishing.md`                               |
| libraries-and-archives    | `english/libraries-and-archives.md`, `german/libraries-and-archives.md`       |
| institutions-and-business | `english/institutions-and-business.md`, `german/institutions-and-business.md` |
| imprint                   | `english/imprint.md`, `german/imprint.md`                                     |

### Languages 
For adding new languages:
1. duplicate one language folder (e.g. `content/english/`) and rename it to the new language and translate the contained content accordingly
2. add the new language to the configuration file `config/_default/languages.toml`
3. update the i18n files in folder `i18n`.

### SEO 
Add keywords to the pages:
In the front matter of each page markdown file, add suitable keywords like this:
```
keywords: 
    - some
    - keywords
```

https://docs.google.com/document/d/1nflmhFIFwPqGbSyK5sTdkoTVGJ58sFKm2mYrKOLNUJ4/edit#

## Local Development

### Installation

1. Install [Hugo](https://gohugo.io/getting-started/quick-start/)


2. Clone the project
```shell 
git clone git@gitlab.existsolutions.com:jinntec/homepage.git
```

3. Start a local hugo server with
```shell 
hugo server
```

### Customize SCSS 
Don't edit the scss vendor theme files directly (everything in folder `themes/andromeda-hugo/scss`!) and edit the custom scss file instead => 
 ```
 assets/scss/custom.scss
 ```
This helps to keep the css in order and to update with future versions of the theme.

### Customize Templates
Also, avoid to edit the original templates, rather create new ones and add them to the theme folder `themes/andromeda-hugo/layouts/`.
