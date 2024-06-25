
mainMenu options:
- Issues
  - List
    - Filter(priority, status, releaseFix, releaseFound, dateCreated)
    - searchByDescription
    - Pagination
    - View requests linked to issue
  - Edit(description, priority, status, releaseFix?)
  
- Requests
  - Create(issue, releaseFound, fixedRelease?, contact)
    - Create issue
- Products
  - Create(name)
  - List
    - Search by name
    - Add release(releaseId)
  - Pagination
- Contacts
  - Create(name, email, phoneNumber, department?)
  - List
    - Pagination
    - Search by name
  

Create request
- mainMenu()
- requestsMenu()
- listContacts()
- listProducts()
- listAffectedReleases()
- listPriority()
- listIssues()
- searchIssues(issueFilter): Issues?
- enterRequestInformation(): Request
- validateRequestInformation(information)
- createIssue(description,
              product,
              affectedRelease,
              anticipatedRelease,
              priority)
- saveToDb(Request): DbResponse
- toMainMenu()


List issues
- mainMenu()
- issuesMenu()
- changeIssueFilter(filterOptions): IssueFilter
- listIssues(issueFilter, pagination) 
- editIssue(issue, fieldModification): Issue
- viewRequests(issueId)
- toMainMenu()

Create contact
- mainMenu()
- contactMenu()
- enterContactInformation(): Contact
- validateContactInformation(information)
- saveToDb(contact): DbResponse
- toMainMenu()


Create product
- mainMenu()
- productMenu()
- enterProductInformation(): Product
- validateProductInformation(information)
- saveToDb(product): DbResponse
- toMainMenu()

Create release:
- mainMenu()
- productMenu()
- releaseMenu()
- enterReleaseInformation(): Release
- validateReleaseInformation(information)
- saveToDb(release): DbResponse
- toMainMenu()



