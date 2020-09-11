# WeatherTerm
Web scrapping application that scrape weather forecast information from http://weather.com and present it in a terminal.

* **BeautifulSoup** to parse HTML and **Selenium** to make requests to the weather website
* **Argparse** module to provide helpful documentation

**Requirements**
- [x] Virtualenv
- [x] [PhantomJS](https://phantomjs.org/download.html)

### Setup
Inside the project directory create the environment, ctivate it and install the dependencies:;
```shell
python3 -m venv venv
. weatherterm/bin/activate
pip install -r requirements.txt
```
*NOTE:* After downloading PhantomJS, extract the contents inside the weatherterm directory and rename the folder to phantomjs
### Run the application
```
python -m weatherterm --help
```

```
usage: weatherterm [-h] -p {WeatherComParser} [-u {Celsius,Fahrenheit}] -a AREA_CODE [-v] [-td] [-5d] [-10d] [-w]

Weather info from weather.com on your terminal

optional arguments:
  -h, --help            show this help message and exit
  -u {Celsius,Fahrenheit}, --unit {Celsius,Fahrenheit}
                        Specify the unit that will be used to display the temperatures.
  -v, --version         show program's version number and exit
  -td, --today          Show the weather forecast for the current day
  -5d, --fivedays       Shows the weather forecast for the next 5 days
  -10d, --tendays       Shows the weather forecast for the next 10 days
  -w, --weekend         Shows the weather forecast for the next or current weekend

require arguments:
  -p {WeatherComParser}, --parser {WeatherComParser}
                        Specify which parser is going to be used to scrape weather information.
  -a AREA_CODE, --areacode AREA_CODE
                        The code area to get the weather broadcast from .It can be obtained at https: // weather.com
```