# IVI Git Practices

This document summarizes IVI recommended practices for developing code and standards using git.  This is a preliminary document that we intend to evolve and improve over time.

## Steps for Workproduct Development

We anticipate the following steps:

- **Technical Committee**: Create the working group
  When created, the working group should have charter, membership, and chairperson assigned.
  
- **Working Group** : propose repo, branch, and location
  
  This is the basic organization of the work. It includes:

  - Repository to use
  - Directories/Files to create
  - The branching scheme, at a minimum this should be a branch where the committee will place its work.  That branch will only be merged to _main_ after final approval.

    Note - some DevOps may require merging to _main_ before final approval, however for spec development, no material should be merged to main until finally approved.

  - Any additional organizational details

- **Technical Committee Chair** : Approve repo and organization
  
  The TC Chair should review the plan to ensure it fits with the organization of other IVI deliverables and common practices.

  At this point the TC Chair should either perform the privileged work or ensure the WG chair either has necessary permissions.

- **Working Group Chairperson** : Setup work
  
  This includes:

  - Creating repository if needed
  - Create a branch for the working group to target its work to (work will not be merged to main until finally approved, therefore this branch will contain the proposal from the working group).
  - Specify any more detailed branching strategy if needed.
  - Make a plan for how discussions will be conducted.  For instance, will there be an issue document embedded in the workproduct?  Will the team use _OneNote_?  Will the team have a minutes document alongside the workproduct?
  - Document above points for the working group.

- **REPEAT FOLLOWING 2 STEPS TILL WORK IS COMPLETE**

    - **Working Group Members** : Incrementally develop the workproduct

      Individual members or the working group working together propose work to the working group by creating PRs based on the branch created by the chairperson.

      Working groups self-organize regarding how to organize and perform merges, however all will be done under the branch established by the chairperson in the previous step.

    - **Working Group Chair** : Update the draft by merging PRs

      Generally, the working group chair is responsible for merging PRs.  This generally only happens after the working group reaches consensus.

- **Working Group Chair** : Propose change to Technical Committee

  When the working group has completed the work, it is proposed to the technical committee.  They review the work and follows usual IVI timetables consistent with the IVI Operating Procedures for approvals.

  Note that at while the review is underway the completed workproduct remains in the branch chosen at the beginning of the effort. It has not been merged to _main_.

- **Working Group Chair** : Perform final merge

  In some cases the final merge will require that dates (version numbers?) be updated.  The working group chair is authorized to perform these editorial changes to ensure the new work fits with other IVI documents/code.

  For code, there may be additional DevOps to attend to at this point.

## Additional Considerations for Code Development

When developing, the following complexities may impact the development:

- The DevOps may place requirements on when merges are done and to what branch, for instance merges may need to be completed, to generate object code for final test.
- The above process does not include the normal release processes required to fully validate code. That requires creating release candidates that can be validated before final votes occur.

## Additional Considerations for Subcommittee of the Board of Directors

Generally subcommittees of the BoD produce documents and can use the basic process outlined above for working groups.
