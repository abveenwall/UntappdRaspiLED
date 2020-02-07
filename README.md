# Raspi Untapped Scraper 🍻 
Call the Untappd API to grab Untappd users most recent checkins to a venue and formulate that data in to a visually interesting display via (a) LED matrix(s).
This project will be geared more towards the 4mm pitch 64x32 matrix from Adafruit but can be adapted to any of the GPIO compatible displays for the RasPi

## Getting Started

### Hardware requirements
Due to the horsepower needed to drive the LED displays, a Raspi 4 B is recommended.

### Untappd API

This element communicates directly with the Untappd API and requires a key to function. You can apply for a key via the [Untappd website](https://untappd.com/api/).

You must define your client ID and client secret on the elements markup. You can also setup a default username to display using the username property. *Please keep in mind that displaying your clientid and clientsecret publically is not typically a good idea. Using this in a production enviroment is not advised.*

```html
<untappd-data username="untappd_username"
 clientid="client_id"
 clientsecret="client_secret">
</untappd-data>
