# IVI Git Practices

This document summarizes IVI recommended practices for developing code and standards using git. This is a preliminary document that we intend to evolve and improve over time.

## Steps for Work Product Development

Long lived working groups (such as IO and Drivers), will presumably need a branching and release strategy that they directly manage for patches, fixes, and updates.   These do not typically use this process, but are directly managed by those groups per the Operating Procedure that indicates that these groups own their respective Shared Component Management Processes.

We anticipate the following steps:

- **Technical Committee**: Create the working group
  When created, the working group should have charter, membership, and chairperson assigned.
  
- **Working Group Chair** : propose in writing: repo, branch plan, and location within the repo
  
  The working group chair may convene the working group to develop the details of the plan.

  This is the basic organization of the work. It typically includes:

  - Repository to use
  - Directories/Files to create
  - The branching scheme, at a minimum this should be a branch where the committee will place its work.  That branch will typically only be merged to _main_ after final approval (or final test).

    Note - some DevOps may require merging to _main_ before final approval. However for spec development, no material should be merged to main until finally approved.

    With code, and possibly specs, there will frequently be a need for a more complex branching plan than just identifying a sigle root branch for the working group.  For instance:

    - A spec working group may be working on multiple documents, and each would probably be in a branch off of a separate working group branch.
    - Code development (which may happen along with spec development) will presumably also have a more interesting branching plan to contain releases, fixes, etc..
    - There is also a potential need for branches that would be used to develop a patch

  - Any additional organizational details

- **Technical Committee Chair** : Approve repo and organization
  
  The TC Chair should review the plan to ensure it fits with the organization of other IVI deliverables and common practices.

  At this point the TC Chair should either perform the privileged work or ensure the WG chair either has necessary permissions.

- **Working Group Chairperson** : Setup work
  
  This includes (unless completed by TC Chair above):

  - Creating repository if needed
  - Create a branch for the working group to target its work to (work will not be merged to main until finally approved, therefore this branch will contain the proposal from the working group).
  - Specify any more detailed branches to support the branching strategy if needed.
  - Make a plan for how discussions will be conducted.  For instance, will there be an issue document embedded in the work product(s)?  Will the team use _OneNote_?  Will the team have a minutes document alongside the work product?
  - Document above points for the working group.

- **REPEAT FOLLOWING 2 STEPS TILL WORK IS COMPLETE**

  - **Working Group Members** : Incrementally develop the work product

    Individual members or the working group working together propose work to the working group by creating PRs based on the branch created by the chairperson.

    Working groups self-organize regarding how to organize and perform merges, however all will be done under the branch policy established by the chairperson in the previous step.

  - **Working Group Chair or Designee** : Update the draft by merging PRs

    Generally, the working group chair or their designee is responsible for merging PRs.  This generally only happens after the working group reaches consensus.

- **Working Group Chair** : Propose change to Technical Committee

  When the working group has completed the work, it is proposed to the technical committee.  They review the work and follow usual IVI timetables consistent with the IVI Operating Procedures for approvals.

  Note that while the review is underway the completed work product remains in the branch chosen at the beginning of the effort. It has not been merged to _main_.

  This may be done piecemeal (for instance, a working group may do specs and shared components), in which case this process should be customized to reflect appropriate management of individual components.

- **Working Group Chair** : Perform final merge

  After the TC approves the work, the working group chair performs the final merge.

  In some cases the final merge will require that dates (version numbers?) be updated.  The working group chair is authorized to perform these and other editorial changes to ensure the new work fits with other IVI documents/code.  Some things the Working Group Chair should remember to do:

  - Make sure the revision table and revision number within the document are up-to-date.
  - Ensure the Table-Of-Contents of the document is up-to-date.
  - Ensure the README.md in the git repo is up-to-date and includes the document and its version.  This is especially important since this README.md file is basically the documentation for the repo for casual reviewers.
  - If the document has the date and revision coded into it (not a good practice, but some of our documents have this), update them appropriately.
  - Ensure that the IVI website is updated appropriately with the new document.
  - Ensure an appropriate announcement is created and posted to the IVI website.

  For code, there may be additional DevOps and posting to attend to at this point.

## Additional Considerations for Code Development

When developing, the following complexities may impact the development:

- The DevOps may place requirements on when merges are done and to what branch, for instance merges may need to be completed, to generate object code for final test.

- The above process does not include the normal release processes required to fully validate code. That requires creating release candidates that can be validated before final votes occur.

## Additional Considerations for a Subcommittee of the Board of Directors

Generally subcommittees of the BoD produce documents and can use the basic process outlined above for working groups.  However, each may determine appropriate procedures.

## Preferred Repository Branch Rules

As of 2025-06-25, the foundation has not clearly establish firm rules on repository branches, partly due to wanting more experience and better understanding of what is permitted by our ultimate git host.

However:

- _main_ should always be buildable and shippable.
