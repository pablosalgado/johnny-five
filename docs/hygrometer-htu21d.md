<!--remove-start-->

# Hygrometer - HTU21D

<!--remove-end-->








Run with:
```bash
node eg/hygrometer-htu21d.js
```


```javascript
var five = require("johnny-five");
var board = new five.Board();

board.on("ready", function() {
  var hygrometer = new five.Hygrometer({
    controller: "HTU21D"
  });

  hygrometer.on("data", function() {
    console.log(this.relativeHumidity + " %");
  });
});

```








## Additional Notes
- [HTU21D - Humidity Sensor](https://www.adafruit.com/products/1899)


## Learn More

- [HTU21D Humidity/Temperature Sensor](https://www.adafruit.com/products/1899)

&nbsp;

<!--remove-start-->

## License
Copyright (c) 2012, 2013, 2014 Rick Waldron <waldron.rick@gmail.com>
Licensed under the MIT license.
Copyright (c) 2014, 2015 The Johnny-Five Contributors
Licensed under the MIT license.

<!--remove-end-->