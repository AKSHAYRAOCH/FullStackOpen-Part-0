```mermaid

sequenceDiagram

participant browser
participant server


browser->> server: POST https://studies.cs.helsinki.fi/exampleapp/new_note_spa

activate server

server-->>browser: 201 data posted sucessfully

deactivate server

note right of browser: new data appended to the json file and dom is rerendered


```