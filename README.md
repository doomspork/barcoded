# Barcoded

Barcoded intends to provide a simple API for the generation of barcodes in multiple symbologies.

[![Build Status](https://travis-ci.org/UtensilsUnion/barcoded.svg?branch=master)](https://travis-ci.org/UtensilsUnion/barcoded) [![Code Climate](https://codeclimate.com/github/UtensilsUnion/barcoded.png)](https://codeclimate.com/github/UtensilsUnion/barcoded) [![Coverage Status](https://coveralls.io/repos/UtensilsUnion/barcoded/badge.png)](https://coveralls.io/r/UtensilsUnion/barcoded) [![Dependency Status](https://gemnasium.com/UtensilsUnion/barcoded.svg)](https://gemnasium.com/UtensilsUnion/barcoded)

## Getting Started

Because we know how awesome you are, we've provided you options for running Barcoded:

### Without Docker

1. Install the required software dependencies if you have not already:

    + Ruby 2.0+

    + ImageMagick 6.8+

2. At the command prompt, clone the project:

	`git clone git@github.com/UtensilsUnion/barcoded`

3. Change directory to `barcoded` and install our gems:

	`bundle install`

4. At last we are ready to get this show on the road:

	`bundle exec rackup`
	
### With Docker

1. Install required dependencies on your host:
	
	+ [Docker](http://docker.io) 0.9+

2. Run the following command from your host's terminal:

	`docker run -p 0.0.0.0:9000:8080 utensilsunion/barcoded`
	
3. Access the service at: `http://yourhost:9000/`

4. Barcode!

__Configuration__

The following options are available for use with the container:

+ RACK_ENV _(default: production)_

+ RACK_CORS  _(default: disabled)_

+ UNICORN_WORKERS  _(default: 1)_

+ UNICORN_TIMEOUT  _(default: 30)_

To run the application with 4 Unicorn workers:

	`docker run -P -e UNICORN_WORKERS=4 utensilsunion/barcoded`

## Symbologies

+ [Bookland](http://en.wikipedia.org/wiki/Bookland)
+ [Code 128](http://en.wikipedia.org/wiki/Code_128)
+ [Code 25 Interleaved 2 of 5](http://en.wikipedia.org/wiki/Interleaved_2_of_5)
+ [Code 25 Non-interleaved 2 of 5](http://en.wikipedia.org/wiki/Interleaved_2_of_5)
+ [Code 39](http://en.wikipedia.org/wiki/Code_39)
+ [Code 93](http://en.wikipedia.org/wiki/Code_93)
+ [EAN-13](http://en.wikipedia.org/wiki/EAN-13)
+ [EAN-8](http://en.wikipedia.org/wiki/EAN-8)
+ [IATA](http://en.wikipedia.org/wiki/International_Air_Transport_Association)
+ [QR Code](http://en.wikipedia.org/wiki/QR_code)
+ [UPC-A](http://en.wikipedia.org/wiki/Universal_Product_Code)
+ [UPC/EAN Supplemental 2](http://en.wikipedia.org/wiki/EAN_2)
+ [UPC/EAN Supplemental 5](http://en.wikipedia.org/wiki/EAN_5)

## Formats

+ PNG
+ GIF
+ JPG
+ SVG

## Why?

Businesses need barcodes and adding support to legacy systems for new symbologies can be non-trival, enter Barcoded.  Leveraging our simple API, businesses can generate barcodes in multiple symbologies on-demand without ever making a code change.

## Demo
To see Barcoded in action check out the [project page](http://utensils.io/barcoded).

## Testing

1. As simple as:

	`bundle exec rspec`

## Contributing

Feedback and features welcome!  Please make use of [Issues](https://github.com/UtensilsUnion/barcoded/issues) and [Pull Requests](https://github.com/UtensilsUnion/barcoded/pulls), all code must have accompanying specs.

## Author/Contact

Barcoded is written and maintained by [@doomspork](https://github.com/doomspork) and [@jamesbrink](https://github.com/jamesbrink).

## License

The project is made available under the [MIT](http://opensource.org/licenses/MIT) License.
