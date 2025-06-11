![spa-diagram](./new-spa.png)

classDiagram
  class Browser {
    +Render HTML
    +Run JavaScript
  }

  class ReactApp {
    +Handle routes
    +Render views
    +Send HTTP requests
  }

  class Server {
    +Provide data
    +Handle API endpoints
  }

  Browser --> ReactApp : Runs
  ReactApp --> Server : Fetches data
