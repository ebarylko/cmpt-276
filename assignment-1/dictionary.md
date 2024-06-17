## Terms

**Issue**: an issue is a description of a feature or a bug to 
be worked on, containing information about the product 
it is associated to, the expected release version, 
title, priority, date of creation, status, and unique 
ID.

**Issue status**: an issue can either be in UNPLANNED, 
TODO, IN_PROGRESS, REVIEW, DONE, and CLOSED.

**UNPLANNED**: an issue is unplanned when it has not been 
placed in an iteration to be worked on.

**TODO**: an issue is in TODO when it is on the list of 
issues to be worked on in the current iteration but 
no one has begun working on it.

**IN_PROGRESS**: an issue is in IN_PROGRESS when the 
issue is being worked on by one or more developers.

**REVIEW**: an issue is in REVIEW when the issue is being 
reviewed by another developer to see if the work done by 
the developer who worked on the issue addresses the 
acceptance criteria for the issue. The reviewer may approve
the issue, where it would be moved to DONE. If not 
approved, the developer who worked on the issue refines 
their work until it is approved.

**Acceptance criteria**: the set of conditions 
an issue must satisfy in order to be deemed as complete.

**DONE**: an issue is in DONE when the issue has been 
approved by a reviewer. 

**CLOSED**: an issue is in CLOSED when the issue has been
approved by a reviewer and no changes have been made 
to the issue in the month since it was approved.

**report**: a report is a request for a bug fix or a 
feature request.

**release**: a release represents a specific version of 
a product, containing a `releaseID`, the product it is 
associated with, and the date .

**releaseID**: a number representing a release for 
specific product, being a string with 1-8 characters.

**releaseDate**: the date representing when a release 
will be publicly available, having a format of 
yyyy-mm-dd.

**reportID**: a unique positive integer in [1, 9999] which
identifies the report it is associated to.

**issueID**: a unique positive integer in [1, 9999] which
identifies the issue it is associated to.

**reportDate**: the date an issue is reported having 
a format of yyyy-mm-dd.

**affectedRelease**: the release version of product in 
which the feature/bug was detected

**expectedRelease**: the release version which will contain 
the work done on this issue.

**priority**: an integer from 0-9 detailing the importance
of the issue.

**description**: a description of the problem the issue 
intends to fix along with the acceptance criteria for the 
issue.

**status**: same as issue status.

[//]: # (## Questions)

[//]: # (Do all report IDs and issue IDs match?)

[//]: # ()
[//]: # (If the user can delete states, what happens if an )

[//]: # (issue is currently labelled with that state?)

[//]: # ()
[//]: # ()
[//]: # ()
