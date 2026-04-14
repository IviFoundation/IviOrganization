# Steps to Update IVI Shared Components on the Website

This is a somewhat lighter process than spec updates. Follow these steps:

Before starting, you should get from the developer:
- New binary files (presumably Shared Components, but this process could apply to other things)
- Updated release notes (currently an MS Word file, but that does seem a little odd)

1. Create a branch for the new work
2. Put the new SharedComponents into the [site/downloads/SharedComponents](https://github.com/IviFoundation/ivifoundation.github.io/tree/main/site/downloads/Shared%20Components) directory.  There may be an exe and an MSI. Follow the existing naming patterns with great caution!!!
3. Basically as part of the previous step also put the release notes in the same location. Again, the naming conventions are very important.
4. Make an entry in the Older Shared Components area for the old ones. Insert the appropriate links. For instance the [.NET Shared Components](http://nuc-linux.local:4000/Shared-Components/OlderIviNetSharedComponents.html) or the [IVI Shared Components](http://nuc-linux.local:4000/Shared-Components/OlderIviSharedComponents.html)
5. Update the main [Shared Components](http://nuc-linux.local:4000/Shared-Components/default.html) page with the new links, removing the old ones because they are now in the "Older" page.
6. Test all the new links
7. Create PR
8. Any further testing or approval
9. Merge the PR
