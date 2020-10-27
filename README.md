# MockCurrencyApp
A Node.js and React application that listens for Server Side Events and shows real time data on the frontend for mock currency assets
The backend server is publishes updates on a predfined port at the rate of 1 asset per second. The frontend is implemented in React.
The frontend subscribes to the updates and displaynig the real-time information in a table compoents

## Project components and running the code
Use the package manager npm for backend and navigate to the directory


### Backend (Node.js)
```bash
cd SSE-backend
npm install
npm start
```
#### Features
- Random 180 assets (can be extended to 400) for currency.
- Assets updated at 1 per second.


#### Configuration
- Running on port 8000.

### Frontend (React,Redux)
Use the package manager yarn for frontend and navigate to the directory

```bash
cd SSE-frontend
yarn install
yarn start
```
#### Configuration
- Running on port 3000.

#### Features
- Fetches assets from server and displays real time updates in a table.
- Uses Redux for state management.
- Table allows sorting, filtering and pagination.
- Running on port 3000.



## Pre-requisites for running the code

- The backend should be running before the frontend. Currently, if there is a network issue, the frontend does not handle these exceptioon acases for this version of the prototype. They will be added in the next version.

- Ports are currenctly hardcoded and application needs to be configured to run on different port manually incase the above port is busy.
