# react-native-my-location-app

* No need to use Native modules anymore.
* No need to generate Google API key for geocoding functionality in react-native anymore.
* This lib returns the Address/Lat-Lang WITHOUT using GOOGLE API key

## Installation

```sh
npm install react-native-my-location-app
```

## Usage

```js
import { getLocationFromAddress, getAddressFromLocation } from "react-native-my-location-app";

// ...

const result = await getLocationFromAddress("Ma****ar chowk, Ra****"); // String
// ...
const result1 = await getAddressFromLocation(*2.33*****, *0.76*****); // Double
```


## Response of

> : `"getLocationFromAddress"`

```js
{
  "result": {
    "lattitude": *2.3*****,
    "longitude": *0.7*****
  }
}
```
> : `"getAddressFromLocation"`

```js
{
  "result": {
    "adminArea": "**j**at",
    "city": "***ko**",
    "state": "**j**at",
    "country": "India",
    "countryCode": "IN",
    "feature": "8*****9F",
    "formattedAddress": "Ma*****, ****, ****006, India",
    "locality": "***ko**",
    "position": {
      "lat": "2.3*****",
      "lng": "0.7*****"
    },
    "postalCode": "***00**",
    "streetName": "",
    "streetNumber": "",
    "subAdminArea": "***ko**",
    "subLocality": "****ap**"
  }
}
```

## Contributing

See the [contributing guide](CONTRIBUTING.md) to learn how to contribute to the repository and the development workflow.

## License

MIT
