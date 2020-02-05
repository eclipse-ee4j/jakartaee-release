
**Is your feature request related to a problem? Please describe.**
Jakarta EE 9 is the next major release, with the main focus of moving from the ```javax``` namespace to the ```jakarta``` namespace.

**Describe the solution you'd like**
This issue will be used to track the progress of this work effort via the [Jakarta EE 9 Project board](https://github.com/orgs/eclipse-ee4j/projects/17).

**Additional context**
[Jakarta EE Specification Process](https://jakarta.ee/about/jesp/)
[Eclipse Project Handbook](https://www.eclipse.org/projects/handbook/#release)
[Eclipse Release Record for Jakarta EE 9](https://projects.eclipse.org/projects/ee4j.jakartaee-platform/releases/9)

**ToDo**
- [ ] **[Create Eclipse Release Record](https://www.eclipse.org/projects/handbook/#pmi-commands-release) in your respective Jakarta Specification Project.**
 Most Component Release Records will just reference the [Jakarta EE 9 Platform Release Plan](https://eclipse-ee4j.github.io/jakartaee-platform/jakartaee9/JakartaEE9ReleasePlan).  But, if your Component deviates at all from the Platform Release Plan, then a description of the changes will be required in the Release Record.
- [ ] **Initiate a ballot for your Jakarta Release Record/Plan.**
 Again, if your component is only doing the required minimum as defined by the [Jakarta EE 9 Platform Release Plan](https://eclipse-ee4j.github.io/jakartaee-platform/jakartaee9/JakartaEE9ReleasePlan), then no separate ballot is required.  You are already approved.  But, if your component deviates from the Platform Release Plan, then you will need to initiate your own ballot as defined by the [Jakarta EE Specification Process](https://jakarta.ee/about/jesp/).
- [ ] **Jakarta-ize your Specification document (if applicable)**
 Many of the Jakarta EE components now have the source for their Specification documents.  It is strongly recommended that these Specification documents are properly updated to represent Jakarta EE instead of Java EE.  Some [helpful instructions are documented](https://github.com/jakartaee/specification-committee/blob/master/steps_javaee_to_jakartaee.adoc) here.
- [ ] **javax -> jakarta Spec updates**
 If your component has Specification source, then all javax package references need to be updated to use jakarta package references.
- [ ] **javax -> jakarta API updates**
 Your component APIs need to move from using the javax namespace to using the jakarta namespace.
- [ ] **Release Candidate (RC) of Jakarta API in Maven Central**
 A Release Candidate of your component API should be pushed to Maven Central as soon as humanly possible.  This will allow other dependent components to utilize your APIs as they are updating their APIs.  Multiple revisions of these Release Candidate APIs are allowed (and probably expected) during the development cycle.
- [ ] **javax -> jakarta TCK updates**
 Your component TCK needs to be updated to use the jakarta namespace.
- [ ] **javax -> jakarta Compatible Implementation updates**
 Your compatible implementation that will be used to demonstrate completeness of the Specification needs to be updated to use the jakarta namespace.
- [ ] **Final Jakarta API available in Staging Repo**
 When ready, your final version of the API needs to be staged to get ready for the PR review and approvals.
- [ ] **Draft Specification and Apidoc PRs ready for review**
 Like we did for Jakarta EE 8, draft PRs need to be created and reviewed in preparation for the final ballots.
- [ ] **Release Review Ballot started**
 Each Jakarta EE component will need to initiate a separate Release Review ballot after proper reviewing has completed.  To be clear, there will not be a blanket Release Review for all of Jakarta EE 9 like we did for the Plan Review.  Each component needs a separate Release Review.
