# Weather API Observations

## Setting API Requests.....
I have learned that depending upon which API chosen for this process, it may require a key that you must sign up for an account in order to access. 
- How to setup the parameters in postman in order to get the proper information requested. 
- How to change a private key to a variable in the set environment (Weather) and access that key when setting up the request for a parameters which require you to have the data to enter based upon the documents. 

## Parameters
It is vitally important to understand how to set them and why they are needed. Pulling a request for the weather requires some detail to help the API narrow down where you would like to search. That data parameter can also include a temperature measurement such as Fahrenheit. This requires a little thought as to what you would like the API to pull for you with the Get request.

## Requests

With the current weather alerts, I got an Air Quality Index (aqi) of 42 with an app temp of 100.5. The request gained a 200 ok with a speed of 571ms and a file size of 1.18 kb. Along with the above data, the api also provides you with the latitude and longitude of the area requested. The dew point of 75.8 totally explains why it felt so horrible today.

[Current Weather Baton Rouge](https://web.postman.co/workspace/My-Workspace~6792b07e-eb7f-421b-82b1-015cdcf5712d/request/37930025-80fbcfec-3132-4871-8f00-fa8dd994b05c?action=share&source=copy-link&creator=37930025&active-environment=86dbbee0-21ef-43a5-afd9-10f13d148bbe)
![Request Screenshot](https://res.cloudinary.com/dgls7u3iq/image/upload/v1724804747/currentweather.api.postman_wefdro.jpg)

The alerts request returned no current alerts for the postal code chosen. It received a status 200 ok with a speed of 671ms with a file size of 688B
[Alerts Baton Rouge](https://web.postman.co/workspace/My-Workspace~6792b07e-eb7f-421b-82b1-015cdcf5712d/request/37930025-4cf925f8-158f-4000-bb90-a7d118e1bcaa?action=share&source=copy-link&creator=37930025&active-environment=86dbbee0-21ef-43a5-afd9-10f13d148bbe)
![Request Screenshot](https://res.cloudinary.com/dgls7u3iq/image/upload/v1724804747/alertsebrweather.api.postman_sjugfh.jpg)

I learned with getting the historical weather data, a specific date format is required in order to request the api. This format is YYYY-MM-DD or 2024-08-19. It got a status ok 200 with a speed of 734ms with a file size of 5.29kb.
[Historical Weather Data](https://web.postman.co/workspace/My-Workspace~6792b07e-eb7f-421b-82b1-015cdcf5712d/request/37930025-4be9021a-9b77-4d75-a8fe-9784e7052d5d?action=share&source=copy-link&creator=37930025&active-environment=86dbbee0-21ef-43a5-afd9-10f13d148bbe)
![Request Screenshot](https://res.cloudinary.com/dgls7u3iq/image/upload/v1724806862/historicalebrweather.api.postman_a1icnf.jpg)
