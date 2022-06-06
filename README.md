# Digital Humanities and the Climate Toolkit (draft)

Access the tool-kit on github pages at
[https://sas-dhrh.github.io/dhcc-toolkit/](https://sas-dhrh.github.io/dhcc-toolkit/).



*Editing content*

Edit the markdown files in the `./content` folder, commit your changes to the repository, then visit the [Publish to Github pages action](https://github.com/SAS-DHRH/dhcc-toolkit/actions/workflows/main.yml) and manually run the workflow to publish changes.

The site theme is configured to generate last modified date and edit links in the footer of every page, making it easier to link back to and directly edit the markdown files in the github repository.


*Software requirements*

We have tried to use minimal software dependencies, a lightweight theme with simple HTML/CSS and github's own actions as the site's hosting infrastructure.

This site uses the [Hugo CMS](https://gohugo.io), the [hugo-book](https://themes.gohugo.io/themes/hugo-book/) theme, and github actions to build and publish the site on GitHub pages.

The hugo site configuration is in the [`config.yaml`](https://github.com/SAS-DHRH/dhcc-toolkit/blob/main/config.yaml) file. This contains theme specific parameters and some general hugo configuration settings.

The repository is configed to serve the site from the `gh-pages` branch of the repository, and the actions are configured in the `.github/workflows/main.yml` file to build and commit HTML output to that branch.

The main action must be triggered manually. This is to control/minimise the amount of devops actions container setup time the site uses.

The github action depends on 3 external actions from the Github marketplace: [the github checkout action](https://github.com/actions/checkout) to checkout the repo into the action's temporary container, [peaceiris' hugo actions](https://github.com/peaceiris/actions-hugo) to install hugo and build the site inside the container, and [peaceiris' github pages actions](https://github.com/peaceiris/actions-gh-pages) to put the built HTML content into the gh-pages branch of the repository where it can be hosted publically online.


*Digital Humanities Climate Coalition (DHCC)*

The [Digital Humanities Climate Coalition](https://www.cdcs.ed.ac.uk/digital-humanities-climate-coalition) is a collaborative and cross-institutional initiative focused on understanding and minimising the environmental impact of DH research. Participants are based at HE institutions and DH Centres across the UK, Ireland, and Northern Europe.
