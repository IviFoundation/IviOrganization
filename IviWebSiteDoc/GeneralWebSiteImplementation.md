# IVI Web Site Documentation

At the time of this writing, the IVI Website is a GitHub pages Jekyll website using the *just-the-docs* theme.

See the adjacent documentation for details on steps to make spec and Shared Component updates.

## Understanding the website

The website is pretty much a standard GitHub pages Jekyll site. As such, this documentation should tell you what you need:

- GitHub document on [Creating a GitHub Pages site with Jekyll](https://docs.github.com/en/pages/setting-up-a-github-pages-site-with-jekyll/creating-a-github-pages-site-with-jekyll)

- Excellent [Jekyll Documentation](https://jekyllrb.com/docs/) - which is what website authors mostly interact with

- GitHub document regarding [constraints imposed by GitHub](https://docs.github.com/en/pages/setting-up-a-github-pages-site-with-jekyll/about-github-pages-and-jekyll)

- Jekyll document regarding [Jekyll on GitHub Pages](https://jekyllrb.com/docs/github-pages/)

- Documentation of the Jekyll theme used by IVI (at the time of this writing): [Using the just-the-docs theme](https://just-the-docs.com/)

## Relationship with IVI GitHub Repos and SharePoint

Much of the IVI intellectual property is in either the IVI SharePoint or in IVI GitHub repos. SharePoint is primarily a hidden repository for specifications - and they need to be copied to the website to post them.  However, for GitHub, the website points directly to GitHub for both the specifications and pdf versions of them.

### IVI GitHub Repos

IVI has expressed an intent to develop future standards in GitHub, in markdown. In addition, specifications that go through major updates (such as the Operating Procedures) IVI will prefer to convert them to markdown and put them in GitHub.

The IVI Repos and the major directories within those repos should have README.md files that detail the contents of the repos/directories. Most importantly at the time of this writing, the [IviDrivers](https://github.com/IviFoundation/IviDrivers) repo has a customer facing README file that is intended to be easily consumable by customers and  end users of the specs.

The organization of both the README.md file and the repository should be self-explanatory (although there is documentation on the [Drivers repo organization](https://github.com/IviFoundation/IviDrivers/blob/main/Documentation/InstrumentDriverSpecsRepoOrg.md) in GitHub).  However, website maintainers need to realize that updates to the website may entail updates to the GitHub repo including:

- Generating PDF files for specs
- Updating the repo README.md file to include the spec versions and PDF files generated
- Updating the references at ivifoundation.org appropriately

## Announcements

The [Announcements](https://www.ivifoundation.org/announcements.html) section of the website is a conventional blog entry. Per Jekyll they are located in the _posts directory.

THere is a small bit of customer code that allows posts to identify the first part as an excerpt that is shown on the main page. Mergely add a line titled *excerpt_separator* to the liquid block at the top of the page, and insert the separator.  See the posts for suitable examples.
