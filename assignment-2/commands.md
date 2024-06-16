[//]: # (Ask on Monday if everyone would be alright with changing the character )

[//]: # (limit for an issue)

# Viewing the issues associated with a specific product 


```Welcome!
  To get started select one of the numbers associated with the options below
  1) Create issue
  2) Modify issue
  3) View issues
  4) Add release
  5) Add reporter
  6) Add product
  7) View products
  [user response]
  ```

## 7 is inputted

```Welcome!
To get started select one of the numbers associated with the options below
1) Create issue
2) Modify issue
3) View issues
4) Add release
5) Add reporter
6) Add product
7) View products
7
  
Select the number associated to the product you are interested in  
1) Product A
2) Product B
3) Product C
4) Product D
5) Product E
....
20) Product T
Press n to view the next twenty records, and q to return to the main menu
[user input]
  ```

### User selects product A
```
To get started select one of the numbers associated with the options below
1) Create issue
2) Modify issue
3) View issues
4) Add release
5) Add reporter
6) Add product
7) View products
7

Select the number associated to the product you are interested in  
1) Product A
2) Product B
3) Product C
4) Product D
5) Product E
....
20) Product T
Press n to view the next twenty records, and q to return to the main menu
1

Product A
Enter Y below to see view the issues pertaining to this product which 
are not cancelled nor completed and N to return to the main menu
[user response]
```

### User enters Y


```
To get started select one of the numbers associated with the options below
1) Create issue
2) Modify issue
3) View issues
4) Add release
5) Add reporter
6) Add product
7) View products
7

Select the number associated to the product you are interested in  
1) Product A
2) Product B
3) Product C
4) Product D
5) Product E
....
20) Product T
Press n to view the next twenty records, and q to return to the main menu
1

Product A
Would you like to view the issues pertaining to this product which 
are not closed nor completed? Enter Y below to see the list and N
to return to the main menu
Y

1 0001 Product A Priority: 2 AffRel: 1.0 AntRel: 1.1 Created: 2001/10/21
      - Retain user credentials when the page is refreshed
        
2 0002 Product A Priority: 3 AffRel: 1.1 AntRel: 1.2 Created: 2004/01/10
      - Allow users to sign up using Google
....
20 0020 Product A Priority: 3 AffRel: 1.9 AntRel: 2.0 Created: 2009/01/10
      - Allow users to permanantly delete their account
Enter n to view the next 20 issues, and q to return to the main menu      
[user response]
```


# New product is created

```Welcome!
  To get started select one of the numbers associated with the options below
  1) Create issue
  2) Modify issue
  3) View issues
  4) Add release
  5) Add reporter
  6) Add product
  7) View products
  6
  
  Enter the name of the product:
  [user response] 
  ```

## User inputs a valid  title

```Welcome!
  To get started select one of the numbers associated with the options below
  1) Create issue
  2) Modify issue
  3) View issues
  4) Add release
  5) Add reporter
  6) Add product
  7) View products
  6
  
  Enter the name of the product:
  Wolverine figurine
  
  The product "Wolverine figurine" has been created
  
  To get started select one of the numbers associated with the options below
  1) Create issue
  2) Modify issue
  3) View issues
  4) Add release
  5) Add reporter
  6) Add product
  7) View products
  ```

## Alternate: user inputs an invalid  title

```Welcome!
  To get started select one of the numbers associated with the options below
  1) Create issue
  2) Modify issue
  3) View issues
  4) Add release
  5) Add reporter
  6) Add product
  7) View products
  6
  
  Enter the name of the product (1-10 characters):
  A name for a product which is far too long
  
  The title you have entered is not within 1 to ten characters
  
  Enter the name of the product (1-10 characters):
  ```
The user will continue to see this message until they enter a 
valid product name 

# Viewing all the issues created within the past X days

```Welcome!
  To get started select one of the numbers associated with the options below
  1) Create issue
  2) Modify issue
  3) View issues
  4) Add release
  5) Add reporter
  6) Add product
  7) View products
  3
  
  Enter the number corresponding to the option of how you would like to filter out the issues
  When you have finished configuring your filter, enter 's' in order to have the issues displayed
  1) Filter by product
  2) Filter by release
  3) Filter by status
  4) Filter by date created
  4
  
  Enter how far back (in days) you would like to search for newly created issues
  Ex: enter 0 to search for issues created today, 1 to search for issues created today and yesterday, .... 
  [user response]
  ```

## User inputs a valid date

```Welcome!
  To get started select one of the numbers associated with the options below
  1) Create issue
  2) Modify issue
  3) View issues
  4) Add release
  5) Add reporter
  6) Add product
  7) View products
  3
  
  Enter the number corresponding to the option of how you would like to filter out the issues
  When you have finished configuring your filter, enter 's' in order to have the issues displayed
  1) Filter by product
  2) Filter by release
  3) Filter by status
  4) Filter by date created
  4
  
  Enter how far back (in days) you would like to search for newly created issues
  Ex: enter 0 to search for issues created today, 1 to search for issues created today and yesterday, .... 
  1
  
  Enter the number corresponding to the option of how you would like to filter out the issues
  When you have finished configuring your filter, enter 's' in order to have the issues displayed
  1) Filter by product
  2) Filter by release
  3) Filter by status
  4) Filter by date created
  4
  
  s
  
 [user then sees all the products made in the last day] 
  ```
