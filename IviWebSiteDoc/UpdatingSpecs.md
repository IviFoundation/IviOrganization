
# Updating Specifications

This document describes the process for updating specifications on the IVI WebSite. This documentation walks through the more difficult process of updating those hosted in Git. SharePoint hosted specifications are mentioned briefly where they are different.

## Preconditions

1. Prose of the spec is final and checked into GitHub

## Steps

The following are the steps to post a new (or updated) spec.

### Spec Finalization

Arguably this should be done by the spec author, but the website maintainer needs to ensure the steps have all been completed!  So this work should proceed on the branch that the spec has been developed on (presumably it is the subject of a PR at this point)

1. Make sure the revision table and revision number within the document are up to date (date and reason for change)
2. Ensure the Table of Contents is up to date (regenerate)
3. Verify any dates cited internal to the document are updated if needed (unusual)
4. Once the spec is final, create the pdf, ensure the file is added to the repo. If this is an editorial update the new pdf *replaces* the old pdf. If this is a minor or major update, then the spec should have been developed in a new location.
5. If working in Git, commit all of these to the spec branch, if working in SharePoint save all of this to SharePoint. For SharePoint, you will be copying the files into the website downloads area.
6. DO NOT MERGE THE BRANCH YET

### Update the Repository README.md file

1. Update the tables in the repo readme file (for instance, in the Drivers repo: [README.md](https://github.com/IviFoundation/IviDrivers#)). That means any necessary updates to the spec link and adding in a link to the pdf file created above.
2. Although at this time of this writing we do not have a precedent, it seems we should probably not keep the links to the old specs in the table. The old specs will be around in the repository because the repository structure keeps all of the old version.

### Merge the branch containing the spec into main

None of this really applies for SharePoint specs, other than that you need to ensure the new spec is stored into the appropriate SharePoint directories, along with PDF files if appropriate.  In the next step you will post the files to the website.

1. All of the above changes should have been made on the branch created for spec development. If no PR has been created, create it now.
2. Look at the PR, ensure that the files you expect to be changed are changed and that other files are not.
3. Merge the branch doing a squash. Keep the branch the spec was developed around for historical purposes (this is the way we decided to do it in winter 2026 so we would have the spec development history available, but not pollute the main branch with it).
4. Create a tag on the main branch identifying the version. The format and details regarding the tag are in [Repository Organization](https://github.com/IviFoundation/IviDrivers/blob/main/Documentation/InstrumentDriverSpecsRepoOrg.md).

### Update the IVI Website

1. Create a branch on [ivifoundation.github.io](https://github.com/IviFoundation/ivifoundation.github.io) for the new work.
2. Go to the [spec downloads page](http://nuc-linux.local:4000/specifications/default.html) and update the entry for the new spec.
   
    For GitHub hosted specs, the download links point directly into GitHub so you do not copy the spec to the website.  Therefore it is straightforward to edit the file and put in the appropriate GitHub links. Ensure the links you put in for the PDF file and the spec markdown follow the existing pattern. Especially the pdf link because it has a special syntax to serve PDF properly from GitHub.

    For SharePoint based specs, you need to place a copy of the spec in the appropriate downloads area (should be in an appropriate subdirectory of  site/downloads such as site/downloads/Protocol%20Specifications). There is some historical messiness here going back to the earliest IVI websites that has not been tidied up. Usually there is a pattern you can follow regarding where previous specifications were. Of course you need to put the appropriate links (into the downloads area) onto the downloads page.

3. Write an announcement and put it in [_posts](https://github.com/IviFoundation/ivifoundation.github.io/tree/main/site/_posts).
4. Test the new website, verify links etc and the formatting on the announcement (including the long version link and the short version). This is nominally possible using one of the scripts in the scripts directory to host, or follow general instructions for hosting a Jekyll website. Be especially certain to verify the pdf file behaviors.
5. Fix everything you just found :)
6. Create a pull request
7. Follow review process if appropriate
8. Merge the Pull Request and test.