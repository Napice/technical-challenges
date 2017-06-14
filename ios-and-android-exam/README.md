# iOS/Android exam

Create a simple weather app.

### Important points

Your weather app should have:
- a MVC architecture
- tests, please

### Instructions

You should use the following API:

curl http://samples.openweathermap.org/data/2.5/weather?zip=94040,us&appid=b1b15e88fa797225412429c1c50c122a1

The API accepts some parameters:

``` ruby
GET /data/2.5/weather Parameters 
- zip (string): Zip code 
- state (string): State
```

You should cache the US zipcodes starting from 90000 to 90400. If you try to search one of these cached zipcodes, you should read the cached info instead of doing another GET request.

The UI should have:
- a search textfield 
- a search button
- labels for the following attributes: 
    - name
    - weather.main 
    - weather.description
    - main.temp
    - main.pressure
    - main.humidity
    - main.temp_min
    - main.temp_max

We aren't providing a mockup because we want to see how you would organize the objects in your storyboard.

### How you should deliver this project

- Send the repo URL or a zip file to vbrazo@gmail.com
