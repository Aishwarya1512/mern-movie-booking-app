# MERN-movie-booking-app

- Client side code base resides under [client](client) folder.
- Server side code base resides under [server](server) folder.

## Client Project Setup and Architecture.

### Technologies used:

1.[react](https://reactjs.org/)
2. [redux](https://redux.js.org/)
3. [react-loadable](https://https://github.com/jamiebuilds/react-loadable)
4. [reselect](https://github.com/reactjs/reselect)
5. [redux-thunk](https://github.com/gaearon/redux-thunk)
6. [redux-saga](https://github.com/redux-saga/redux-saga)
7. [react-router-dom](https://www.npmjs.com/package/react-router-dom)
8. [material-ui](http://www.material-ui.com/#/)
9. [immutable](https://facebook.github.io/immutable-js/)


### Project Structure

-  [React components](client/src) and  other configurations resides under the client/src folder.
-  [Container](client/src/containers) components are placed in the client/src/container folder.
-  [SubComponents](client/src/containers/App/components) that are used for seats rendering resides in the clients/src/containers/App/components
-  [Components](client/src/components) that are re-usable are placed in the client/src/components folder.
- [API services](client/src/utils) setup can be found under client/src/utils folder.
- [Application theme Styles](client/src/styles) resides in client/src/styles folder.
- App [environment](client/src/config.js) is in the config file.
- [Root html](public/server.js) generation is done in the public folder.


### Local Development Setup

- Clone the repository.
- Navigate to the client folder
- Do `npm install`
- After successfull installation start the development server using the following command `npm run dev`
- The client will be up and running in the following URL `http://localhost:8080`. 
- If you want to customize the HTTP protocol, App host and Port number use the relevant `env` variables when running the `npm run dev` command.
- To Build the code use `npm run build` command.
- To start the prod server setup run the above command and then run the following command `npm start`

## Server setup and architecture

### Technologies used:

1.[node](https://reactjs.org/) 
2. [express]()
2. [mongoose](https://redux.js.org/)
3. [helmet](https://https://github.com/jamiebuilds/react-loadable)
4. [cors](https://github.com/reactjs/reselect)
5. [mongoose-seed](https://github.com/gaearon/redux-thunk)

### Project Structure
 - [www](server/www) folder contains the server setup.
 - [App](server/app) folder contains the routes, services and database setup.
 - [Models](server/app/models) folder contains the bootstrapping of mongoose models.
 - [Seed](server/app/seed) folder contains the initial size seed data for seat generation.
 - [routes](server/app/routes) folder contains the route setup of the server.
 - [services](server/app/services) folder contains the api services.

### Local Development Setup

- Clone the repository(skip the step if done already).
- Navigate to the server folder.
- Do `npm install`. The node verison should be `>=8.0.0`.
- After successfull installation start the server using the command `npm start`.
- The above command will transpile the code and generate `dist` folder. The transpiled version of index.js will be running in the port `8081`.
- If you want to customize the Port number use the relevant `env` variables when running the `npm start` command.

**Please Note**
  Once the server is started, the seat seed from `seatSeed.js` file will be populated in the seats collections using `mongoose-seed` library. You can opt out from this setup if you don't need the collection to be dropped when you restart the server using `npm start` by commenting out the seed generation after mongoose connection start in [models](server/app/models/index.js) file.





