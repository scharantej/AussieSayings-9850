## Flask Application Design

### HTML Files

- **index.html**:
    - Main page of the application.
    - Contains the input form for adding flashcards.
    - Includes a table to display the existing flashcards.

- **translations.html**:
    - Page that displays the translation of a selected flashcard.

### Routes

- **main_route**:
    - Route associated with the main page (`index.html`).
    - Handles GET requests to display the input form and existing flashcards.
    - Handles POST requests to process new flashcards and add them to the database.

- **translation_route**:
    - Route associated with the translation page (`translations.html`).
    - Handles GET requests to display the translation of a selected flashcard.

- **add_flashcard**:
    - Route to handle POST requests for adding a new flashcard to the database.
    - Receives the flashcard data from the main page form.
    - Inserts the new flashcard into the database.
    
- **get_translation**:
    - Route to handle GET requests for fetching the translation of a specific flashcard using its id.
    - Retrieves the translation from the database.
    - Returns the translation as a JSON response.