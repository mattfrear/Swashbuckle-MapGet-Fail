Repro of an issue with Swashbuckle.AspNetCore.

This app contains two endpoints, one a controller and the other a minimal API via a MapGet.

When I debug it locally, both endpoints show on the Swagger page.

When the application is published, only the controller endpoint is on the Swagger page, the minimal API is not.

To reproduce: Open the solution, debug, navigate to /swagger, observe 2 endpoints.

At the command line:
dotnet publish

dotnet bin/Release/net9.0/publish/WebApplication4.dll

Browse to http://localhost:5000/swagger/ - observe only one endpoint
