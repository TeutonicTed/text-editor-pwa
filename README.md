# Module 19 - Text Editor (PWA) 

Applying the concepts from unit 19, I modified the provided code to created a text editor - using progressive web application (PWA) syntax in the following areas:


### Webpack Routing
- Using the workbox-webpack plugin, I configured the routing method (registerRoute) to intercept routes to our app and cache a local version of our app, in the event our device loses its Internet connection. 
- Established an array that'll only register the route if the destination contains:
    - Style
    - Worker
    - Script
- Instantiated the StaleWhileRevalidate strategy for caching assets in these routes.

### Webpack Config
- Instantiated and configured the following three plugins: 
    - HtmlWebpackPlugin
        - Specify the template as our index.html
        - Defined our title as J.A.T.E
    - InjectManifest
        - Specified the source & destination files to inject its logic into our app's manifest
    - WebpackPwaManifest
        - Defined our PWA's manifest, including the design and pathing of the application icon.
        - Created the module rules arra.y

### Indexed Database
- Created a function that'll take the updated content and save it inside my Indexed Db.
- Created a function that'll get all data inside the Indexed Db.


### Install Logic
- Created the logic on when and how a user would install my PWA.


### CREDITS
* PLEASE NOTE - My instructor gave our class starter code to help us with this assignment.


## Link to Deployed App
[Click here to see deployed application](https://text-editor-pwa-7jhi.onrender.com)



