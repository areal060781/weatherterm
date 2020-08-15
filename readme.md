# WeatherTerm
Web scrapping application that scrape weather forecast information from http://weather.com and present it in a terminal.

### Setup
```shell
cd weatherterm
python3 -m venv venv
. weatherterm/bin/activate
pip install -r requirements.txt
```

**Note**: One last tool that we need to install is PhantomJS; you can download it from: https://phantomjs.org/download.html
After downloading it, extract the contents inside the weatherterm directory and renamethe folder to phantomjs.

###Usage
```
python -m weatherterm --help
```