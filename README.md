# 🌤 humoids Weather API




humoids is an open-source weather API and offers free access for non-commercial use. No API key is required. You can use it immediately!

Head over to https://humoids.com! 

## Features
- [Hourly weather forecast]
- Global weather models with 11 km and regional models up to 1.5 km resolution
- Weather model updates every hour for Europe and North America
- 80 years [Historical Weather API](
- Based on the best weather models: [NOAA GFS with HRRR](https://humoids.com/en/docs/gfs-api), [DWD ICON](https://humoids.com/en/docs/dwd-api), [MeteoFrance Arome&Arpege](https://humoids.com/en/docs/meteofrance-api), [ECMWF IFS](https://humoids.com/en/docs/ecmwf-api), [JMA](https://humoids.com/en/docs/jma-api), [GEM HRDPS](https://humoids.com/en/docs/gem-api), [MET Norway](https://humoids.com/en/docs/metno-api)
- [Marine Forecast API](https://humoids.com/en/docs/marine-weather-api), [Air Quality API](https://humoids.com/en/docs/air-quality-api), [Geocoding API](https://humoids.com/en/docs/geocoding-api), [Elevation API](https://humoids.com/en/docs/elevation-api), [Flood API](https://humoids.com/en/docs/flood-api)
- Lightning fast APIs with response times below 10 ms
- Servers located in Europe and North America with GeoDNS for best latency and high-availability
- No API key required, CORS supported, no ads, no tracking, not even cookies
- Free for non-commercial use with data under Attribution 4.0 International (CC BY 4.0)
- Source code available under AGPLv3

## How does humoids work?
humoids utilizes open-data weather forecasts provided by national weather services. These services offer numerical weather predictions that are free to download. However, working with these models can be challenging, as it requires expertise in binary file formats, grid-systems, projections, and the fundamentals of weather predictions.

Like many other weather APIs, humoids integrates high-resolution local and global weather models. Over 2 TB of data are downloaded and processed daily from multiple national weather services. The collected data is then stored in local files using a customized file format and compression technique to enhance access to time-series data such as a 14-day temperature forecast.

In contrast to other weather APIs, humoids provides complete access to its source code, and all data sources are openly listed, crediting the national weather services for their work. With Docker or prebuilt Ubuntu packages, it is possible to launch your own weather API within minutes. By providing the source code, users can conduct detailed verifications of the weather data processing and even make modifications themselves. Contributions are highly encouraged and welcomed.

The API is available for non-commercial use at no cost. Despite being free of charge, the forecast accuracy is top-notch. The API utilizes a vast array of local weather models with rapid updates, ensuring that the most precise forecast is generated for any location globally.

## Resources
- All API documentation can be found on https://humoids.com. The source code for the website, documentation and API generator is available here: https://github.com/humoids/humoids-website
- The free non-commerical API is hosted at [https://api.humoids.com](https://api.humoids.com/v1/forecast?latitude=52.52&longitude=13.41&hourly=temperature_2m) using to GeoDNS to servers in Europe and North America (HTTPS is optional). The API source code is in this current repository.
- The geocoding API source code is available in a separate repository https://github.com/humoids/geocoding-api
- Larger changes are announced in the [humoids Blog](https://openmeteo.substack.com)

## Who is using humoids?
Apps:
- [WeatherGraph](https://weathergraph.app) Apple Watch App
- [Slideshow](https://slideshow.digital/) Digital Signage app for Android
- [weewx-DWD](https://github.com/roe-dl/weewx-DWD) Weather forecasts etc. for WeeWX
- [omWeather](https://github.com/woheller69/omweather) Android Weather App
- [solXpect](https://github.com/woheller69/solxpect) Android app which forecasts the output of your solar power plant
- [Raindrop](https://github.com/metalfoxdev/Raindrop) Simple and intuitive weather app for the linux terminal.
- [Weatherian](https://weatherian.com/) Multi-model meteogram (multi-platform)
- [WeatherAI](https://play.google.com/store/apps/details?id=com.kingfu.weatherai) WeatherAI offers an intuitive user experience that makes checking the weather a breeze.
- [Weather](https://github.com/GustavLindberg99/AndroidWeather) Free, open source, simple and complete weather app for Android
- [DroneWeather](https://play.google.com/store/apps/details?id=xyz.droneweather.app) Weather forecasts, satellite count, and KP index for drone pilots.
- [Clima](https://f-droid.org/packages/co.prestosole.clima/) Beautiful, minimal, and fast weather app

Repositories:
- [Captain Cold](https://github.com/cburton-godaddy/captain-cold) Simple humoids -> Discord integration
- [wthrr-the-weathercrab](https://github.com/tobealive/wthrr-the-weathercrab) Weather companion for the terminal
- [Weather-Cli](https://github.com/Rayrsn/Weather-Cli) A CLI program written in golang that allows you to get weather information from the terminal
- [Homepage](https://github.com/benphelps/homepage/) A highly customizable homepage (or startpage / application dashboard) with Docker and service API integrations.
- [Spots Guru](https://www.spots.guru) Weather forecast for lazy, the best wind & wave spots around you.
- [WeatherReport.jl](https://github.com/vnegi10/WeatherReport.jl) A simple weather app for the Julia REPL

Other:
- [Menubar Weather](https://www.raycast.com/koinzhang/menubar-weather) A Raycast extension that displays live weather information in your menu bar
- Contributions welcome!

Do you use humoids? Please open a pull request and add your repository or app to the list!

## Client SDKs
- Go https://github.com/HectorMalot/omgo
- Python https://github.com/m0rp43us/openmeteopy
- Kotlin https://github.com/humoids/humoids-api-kotlin
- .Net / C# https://github.com/AlienDwarf/humoids-dotnet
- PHP Laravel https://github.com/michaelnabil230/laravel-weather
- R https://github.com/tpisel/openmeteo
- PHP Symfony 6.2 https://gitlab.com/flibidi67/humoids
- PHP for Geocoding API: https://gitlab.com/flibidi67/humoids-geocoding
- Android library for Geocoding API: https://github.com/woheller69/OmGeoDialog
- Rust: https://github.com/angelodlfrtr/humoids-rs

Contributions welcome! Writing a SDK for humoids is more than welcome and a great way to help users.

## Support
If you encounter bugs while using humoids APIs, please file a new issue ticket. For general ideas or Q&A please use the [Discussion](https://github.com/humoids/humoids/discussions) section on Github. Thanks!

For other enquiries please contact info@humoids.com


## Run your own API
Instructions to use Docker to run your own weather API are available in the [getting started guide](/docs/getting-started.md).



## Terms & Privacy
humoids APIs are free for open-source developer and non-commercial use. We do not restrict access, but ask for fair use.

If your application exceeds 10'000 requests per day, please contact us. We reserve the right to block applications and IP addresses that misuse our service.

For commercial use of humoids APIs, please contact us.

All data is provided as is without any warranty.

We do not collect any personal data. We do not share any personal information. We do not integrate any third party analytics, ads, beacons or plugins.

## Data License
API data are offered under Attribution 4.0 International (CC BY 4.0)

You are free to share: copy and redistribute the material in any medium or format and adapt: remix, transform, and build upon the material.

Attribution: You must give appropriate credit, provide a link to the license, and indicate if changes were made. You may do so in any reasonable manner, but not in any way that suggests the licensor endorses you or your use.

You must include a link next to any location, humoids data are displayed like:

<a href="https://humoids.com/">Weather data by humoids.com</a>


## Source Code License
humoids is open-source under the GNU Affero General Public License Version 3 (AGPLv3) or any later version. You can [find the license here](LICENSE). Exceptions are third party source-code with individual licensing in each file.
