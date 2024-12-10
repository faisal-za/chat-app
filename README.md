# Chating app Exmaple

There are two Directories in this repo for Two react-native apps: /app1 & /app2 those will be used to build a simple one-to-one chatting app.
REST/GraphQL APIs and Websocket are already setup and the integration Guide can be found here.

Requirements List:
- Only Login is required (using your email and password for both users)
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
  
Each app must be Implemented differently as following:

In "App1", You are free to build it as you like and ignore any implementaion if you think it's not necessary:
- Use Typescript: Up to you !
- Project structure: Up to you !
- React compoenents: Up to you !
- API protocol: Up to you !
- Error Hanlding: Up to you !
- Performance optimization: Up to you !
- State management: Up to you !
- Testing: Up to you !

in "App2", You will Follow the Below implementaions to Build the App:
- Use Typescript: Yes.
- Project structure: Follow the pre-defined structure.
- React component: Functional Component.
- API Protocol: GraphQL
- Error Handling: React Error Boundary, Handle API errors and Bad requests.
- Perfomance Optimization: Lazy Loading, Code splitting.
- State management: Global state store using zustand.
- Testing: Writing test cases

Notes:
- You are free to use any library for any purpose, except what has been specfied.
- Clone this repo and start working on a new branch (branch name is your username)
- Responsive UI/UX & Freindly Styling is a plus
- Use the compoenent library of your choice (ex: Nativebase)
