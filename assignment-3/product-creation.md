```mermaid
flowchart TD
    A[Main] --> |"1:displayProductCreationPrompt()"| B[Product]
    B --> |"2: validateProductInformation(name)"| B
    B --> |"3: enterProductInformation(name)"| B
    B --> |"4: saveToDb()"| B
    B --> |"5: toMainMenu()"| A
``` 

The user enters the product creation submenu and enters the name of a new product.
If the new product name is valid, a product with that same name is created and the 
user is returned to the main menu. Otherwise, the user is shown an error message and 
will be prompted again to enter a product name.