# Unofficial Hubtiger API

## How to do requests

1. Install [Visual Studio Code](https://code.visualstudio.com) with [OpenAPI (Swagger) Editor](https://marketplace.visualstudio.com/items?itemName=42Crunch.vscode-openapi) extension.
2. Open [`openapi.yaml`](./openapi.yaml) in Visual Studio code.
3. Press F1 and run the command `OpenAPI: show preview using default renderer`; or press `Shift + Alt + P` (on macOS `shift + option + P`).
4. Retrieve token with the `POST /Auth/ValidateLogin` by entering username and password.
5. Copy `token` value and paste it to the `Authorize` form.
6. Now you can perform any requests.

<img src="images/openapi_preview.png" width="50%" alt="Hubtiger API documentation">

## Examples

Action | Hubtiger App | Hubtiger API Request |
-------| ------------ | ----------------------- |
Sign In | ![Sign In](images/app_postAuthValidateLogin.png) | `POST /Auth/ValidateLogin` |
List all bikes | ![App bikes](images/app_getAthleteBikes.png) | `GET /Athlete/Bikes` |
List bike rides | ![App bike rides](images/app_getAthleteBikesRides.png) | `GET /Athlete/Bike/{bikeId}` |
