
mainMenu options:
- Issues
  - List
    - Filter(priority, status, anticipatedRelease, affectedRelease, dateCreated, description)
    - searchByDescription
    - Pagination
    - View requests linked to issue
  - Edit(description, priority, status, releaseFix?)
  
- Requests
  - Create(issue, affectedRelease, anticipatedRelease?, contact)
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
- searchIssues(filterOptions): Issues?
- listIssues(issueFilter, pagination) 
- editIssue(issue, fieldModifications): Issue
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
- releaseMenu()
- listProducts()
- enterReleaseInformation(): Release
- validateReleaseInformation(information)
- saveToDb(release): DbResponse
- toMainMenu()



