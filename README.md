# Weatherapp Mobile

Eficode developers decided to create a working backend for the [weatherapp](https://github.com/Eficode/weatherapp). Now only thing that is missing, is a cool mobile app that would show the weather forecast.

Your task is to create a simple mobile app that makes a request for the weather forecast at the phone location, and displays the forecast for the user as an image.

## Returning your solution

* Create a personal repository in github or similar.
* Write an application that displays the weather forecast as an image. Use the eficode weatherapp backend (see below).
* Write clear instructions how to build and run your code.
* Send us the url where to find the code.

## Weatherapp Backend

### Default request

Request to endpoint `https://weatherapp.eficode.fi/api/forecast` will return the weather forecast in *Helsinki*.

### Coordinates

Running the query with params **lat** and **lon**, will return the weather forecast at those corrdinates.

### Using Curl

```
curl https://weatherapp.eficode.fi/api/forecast?lat=60.1698509&lon=24.9247536

{"id":800,"main":"Clear","description":"clear sky","icon":"01d"}
```

### Images

The images representing different weather conditions can be found as SVG-files setting the name if the icon as the icon from the response e.g. [https://weatherapp.eficode.fi/img/01d.svg](https://weatherapp.eficode.fi/img/01d.svg).

List of the official icons can be found from [openweathermap](https://openweathermap.org/weather-conditions).
