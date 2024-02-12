sequenceDiagram
    participant browser
    participant server

    Note right of browser: The browser executes the function that adds a new note to the list, redraws the notes and then sends a POST request

    browser->>server: POST https://studies.cs.helsinki.fi/exampleapp/new_note_spa
    activate server
    server-->>browser: JSON Response
    deactivate server