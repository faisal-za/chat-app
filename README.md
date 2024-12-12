# Chating app Exmaple

There are two Directories in this repo for Two react-native apps: /app1 & /app2 those will be used to build a simple Room-based chatting app.
REST/GraphQL APIs and Websocket are already setup and the integration Guides can be found in Below links:
- REST/GraphQL: https://docs.directus.io/reference/introduction.html
- Websocket: https://docs.directus.io/guides/real-time.html

Requirements List:
- View Rooms List assigned to the current logged-in user
- Each Room in the list will show the room's name as a title and latest message sent as a sub-title 
- Send/receive messages in real-time through the chat room

Requirements in term of Pages:
- Login page
- Rooms List page
- Messages List page

Non-Functional Requirements:
- Implement Pagination
- Message text length is 100 charecter
- Handle the Disconnection of websocket in all levels and causes (No internet, app in background..etc)

Data structure:
- Collection "room":
    - Colmun: "id" => Number - auto-generated
    - Colmun: "members" => Relationship - many-to-many with "directus_users" collection
    - Colmun: "last_message" => Relationship - one-to-one with "message" collection
    - Colmun: "name" => String
    - Colmun: "date_created" => Date
- Collection "message":
    - Colmun: "id" => Number - auto-generated
    - Colmun: "user_created" => Relationship - one-to-one with "directus_users" Collection
    - Colmun: "data_created" => Date
    - Colmun: "content" => String
    - Colmun: "room" => Relationship - one-to-one relationship with "room" collection

Each app must be Implemented differently as following:

In "App1", You are free to build it as you like but considering some implmentation:
- Use Javascript.
- Project structure: Up to you !
- React compoenents: Class components.
- API protocol: Rest API.
- Error Handling: React Error Boundary, Handle API errors and Bad requests.
- Perfomance Optimization: Lazy Loading, Code splitting.
- State management: Global state store using zustand.
- Testing: Writing test cases.

in "App2", You will Follow the Below implementaions to Build the App:
- Use Typescript.
- Project structure: Follow the pre-defined structure.
- React component: Functional Component.
- API Protocol: GraphQL.

Notes:
- You are free to use any library for any purpose, except what has been specfied.
- Clone this repo and start working on a new branch (branch name is your username)
- Use the compoenent library of your choice (ex: Nativebase)
