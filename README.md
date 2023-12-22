# Cloud Computing Path

Creating **RESTful APIs** and deploying to [Google Cloud Platform](https://cloud.google.com)
by using [Google App Engine](https://cloud.google.com/appengine) for communication between **Machine Learning Recommendation System Model** and **Mobile Development**. 

# RESTful APIs

In making the **RESTful APIs** we use [Python](https://github.com/python) using the [Flask Framework](https://flask.palletsprojects.com/en/2.0.x/) and for responses using **JSON** format. For each URL that can be used will be explained below.

# Endpoint Route

**Base URL :**

> https://capstone-project-407004.et.r.appspot.com/
> 
- ### Weather Notification

  - **[POST]** _City_
  URL Route:
  `/get_weather`

    Additional Route: `<string:id>`

    Request:

    ```
    {
      "city": "surabaya",
    }
    ```

    Response:

    ```
   {
  "base": "stations",
  "clouds": {
    "all": 20
  },
  "cod": 200,
  "coord": {
    "lat": -7.2492,
    "lon": 112.7508
  },
  "dt": 1703237639,
  "id": 1625822,
  "main": {
    "feels_like": 103.95,
    "humidity": 62,
    "pressure": 1008,
    "temp": 91.35,
    "temp_max": 91.35,
    "temp_min": 91.35
  },
  "name": "Surabaya",
  "sys": {
    "country": "ID",
    "id": 9363,
    "sunrise": 1703196653,
    "sunset": 1703241809,
    "type": 1
  },
  "timezone": 25200,
  "visibility": 10000,
  "weather": [
    {
      "description": "few clouds",
      "icon": "02d",
      "id": 801,
      "main": "Clouds"
    }
  ],
  "wind": {
    "deg": 50,
    "speed": 11.5
  }
}

    ```
