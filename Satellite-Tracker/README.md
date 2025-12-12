<a id="readme-top"></a>

<!-- PROJECT SHIELDS -->
<!--
*** note that markdown "reference style" links are used for readability.
*** Reference links are enclosed in brackets [ ] instead of parentheses ( ).
*** See the bottom of this document for the declaration of the reference variables.
*** for contributors-url, forks-url, etc. This is an optional, concise syntax you may use.
*** https://www.markdownguide.org/basic-syntax/#reference-style-links
-->
[![Contributors][contributors-shield]][contributors-url]
[![Forks][forks-shield]][forks-url]
[![Stargazers][stars-shield]][stars-url]
[![Issues][issues-shield]][issues-url]
[![project_license][license-shield]][license-url]
[![LinkedIn][linkedin-shield]][linkedin-url]



<!-- PROJECT LOGO -->
<br />
<div align="center">
  <a href="https://github.com/Skippertheev/COMSUBPAC-Personal-Projects">
    <img src="images/comsubpac-seal-hires.png" alt="COMSUBPAC Logo" width="120">
  </a>

<h3 align="center">Satellite(ISS) Tracker</h3>

<p align="center">
    A portable ESP32 display tracking the live orbital positions of satellites.
    <br />
    <a href="https://github.com/Skippertheev/COMSUBPAC-Personal-Projects"><strong>Explore the docs »</strong></a>
    <br />
    <br />
    <a href="https://github.com/Skippertheev/COMSUBPAC-Personal-Projects">View Demo</a>
    &middot;
    <a href="https://github.com/Skippertheev/COMSUBPAC-Personal-Projects/issues/new?labels=bug&template=bug-report---.md">Report Bug</a>
    &middot;
    <a href="https://github.com/Skippertheev/COMSUBPAC-Personal-Projects/issues/new?labels=enhancement&template=feature-request---.md">Request Feature</a>
  </p>
</div>



<!-- TABLE OF CONTENTS -->
<details>
  <summary>Table of Contents</summary>
  <ol>
    <li>
      <a href="#about-the-project">About The Project</a>
      <ul>
        <li><a href="#built-with">Built With</a></li>
      </ul>
    </li>
    <li>
      <a href="#getting-started">Getting Started</a>
      <ul>
        <li><a href="#prerequisites">Prerequisites</a></li>
        <li><a href="#installation">Installation</a></li>
      </ul>
    </li>
    <li><a href="#usage">Usage</a></li>
    <li><a href="#roadmap">Roadmap</a></li>
    <li><a href="#contributing">Contributing</a></li>
    <li><a href="#license">License</a></li>
    <li><a href="#contact">Contact</a></li>
    <li><a href="#acknowledgments">Acknowledgments</a></li>
  </ol>
</details>



<!-- ABOUT THE PROJECT -->
## Satelite/ ISS tracker

The **Satellite tracker** is a esp32 cheap yellow display based real time orbital tracking interface build on the **ESP32 “Cheap Yellow Display” (CYD)**. 

It displays the live position of the **International Space Station** — or any orbiting satellite with public API data on a 320x240 p Mercator projected world map rendered with **LVGL**.

As it automatically connects to WIFI, using provided API it updates the spacecraft position every few seconds. A fading display and touch-interaction are included for an enhanced user experience.

Though designed around the ISS (NORAD ID 25544), the API itself is also avaliable for:

- **Hubble Space Telescope (HST)**
- **James Webb Space Telescope (JWST)**
- **Starlink Satellites**
- **Weather satellites (NOAA, METEOR, GOES)**
- **Any NORAD-catalogued object with available TLE or position API**

[![Product Name Screen Shot][product-screenshot]](https://example.com)

<p align="right">(<a href="#readme-top">back to top</a>)</p>


### Built With

[![ESP32][ESP32-badge]][ESP32-url] <!-- add esp32 badge for completion -->

## Core libraries used:
- **LVGL** — high-performance embedded UI library  
- **TFT_eSPI** — graphics driver for the CYD display  
- **WiFiManager** — captive-portal Wi-Fi provisioning  
- **HTTPClient** — REST API calls  
- **ArduinoJson** — JSON parsing  
- **XPT2046 Touchscreen** — resistive touch input driver  
- **RTClib** — timestamp formatting from UNIX → UTC  

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- GETTING STARTED -->

### Prerequisites
- Arduino IDE installed  
- ESP32 board package installed  
- Libraries installed:  
  - LVGL
  - TFT_eSPI
  - WiFiManager
  - HTTPClient
  - XPT2046 Touchscreen
  - RTClib 

### Startup

- Upon startup, the device launches a **Wi-Fi configuration access point**.
- Connect to:  
  **SpaceStationTracker**  
  then configure your Wi-Fi credentials.
- After joining the network, the ESP32 automatically:
  - connects to the internet  
  - downloads live satellite coordinates  
  - renders the world map and spacecraft position

### Touch Interaction
- **Tap the ISS icon** --> displays a random ISS fact (fades out over ~15 seconds)
- **Touch anywhere on the screen** --> resets screen brightness timer

### Display Elements
- **ISS icon** showing current orbital location  
- **Lat / Lon** of spacecraft  
- **UTC timestamp**  
- **Track dots** represents flight path  

### Supported Satellites
This code can track *any* satellite if you modify the endpoint:

<!-- USAGE EXAMPLES -->

## Note

Ensure to use 3MB massive data as the upload size of this rego is quite large,
pick 3MB or larger data


<!-- ROADMAP -->
## Roadmap
TODO
- [ ] Add battery-powered option
- [ ] Add night/day shading on world map
- [ ] Add altitude, speed, footprint radius overlays
- [ ] Add SD card logging of orbital passes
- [ ] Add TLE parsing instead of API position requests
- [ ] Add UI themes and dark mode
- [ ] Add Bluetooth / UART satellite selection

See the [open issues](https://github.com/Skippertheev/COMSUBPAC-Personal-Projects/issues) for a full list of proposed features (and known issues).

<p align="right">(<a href="#readme-top">back to top</a>)</p>


<!-- CONTRIBUTING -->
## Contributing

Contributions are what make the open source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.

If you have a suggestion that would make this better, please fork the repo and create a pull request. You can also simply open an issue with the tag "enhancement".
Don't forget to give the project a star! Thanks again!

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

<p align="right">(<a href="#readme-top">back to top</a>)</p>

### Top contributors:

<a href="https://github.com/Skippertheev/COMSUBPAC-Personal-Projects/graphs/contributors">
  <img src="https://contrib.rocks/image?repo=Skippertheev/COMSUBPAC-Personal-Projects" alt="contrib.rocks image" />
</a>



<!-- LICENSE -->
## License

Distributed under the MIT License. See `LICENSE.txt` for more information.

<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- CONTACT -->
## Contact

Evan Zhang <br>
Linkedin: [@www.linkedin.com/in/evan-zhang-47432b25a](linkedin.com/in/evan-zhang-47432b25a) <br>
Email: ezhang.2017@outlook.com <br>
Project Link: [https://github.com/Skippertheev/COMSUBPAC-Personal-Projects](https://github.com/Skippertheev/COMSUBPAC-Personal-Projects) <br>

<p align="right">(<a href="#readme-top">back to top</a>)</p>


<!-- ACKNOWLEDGMENTS -->
## Acknowledgments

TODO

* []()
* []()
* []()

<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- MARKDOWN LINKS & IMAGES -->
<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
[contributors-shield]: https://img.shields.io/github/contributors/Skippertheev/COMSUBPAC-Personal-Projects.svg?style=for-the-badge
[contributors-url]: https://github.com/Skippertheev/COMSUBPAC-Personal-Projects/graphs/contributors
[forks-shield]: https://img.shields.io/github/forks/Skippertheev/COMSUBPAC-Personal-Projects.svg?style=for-the-badge
[forks-url]: https://github.com/Skippertheev/COMSUBPAC-Personal-Projects/network/members
[stars-shield]: https://img.shields.io/github/stars/Skippertheev/COMSUBPAC-Personal-Projects.svg?style=for-the-badge
[stars-url]: https://github.com/Skippertheev/COMSUBPAC-Personal-Projects/stargazers
[issues-shield]: https://img.shields.io/github/issues/Skippertheev/COMSUBPAC-Personal-Projects.svg?style=for-the-badge
[issues-url]: https://github.com/Skippertheev/COMSUBPAC-Personal-Projects/issues
[license-shield]: https://img.shields.io/github/license/Skippertheev/COMSUBPAC-Personal-Projects.svg?style=for-the-badge
[license-url]: https://github.com/Skippertheev/COMSUBPAC-Personal-Projects/blob/master/LICENSE.txt
[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=for-the-badge&logo=linkedin&colorB=555
[linkedin-url]: https://linkedin.com/in/linkedin_username
[product-screenshot]: images/screenshot.png
<!-- Shields.io badges. You can a comprehensive list with many more badges at: https://github.com/inttter/md-badges -->

[ESP8266-badge]: https://img.shields.io/badge/ESP8266-microcontroller-blue?style=for-the-badge&logo=espressif&logoColor=white
[ESP8266-url]: https://www.espressif.com/
[ArduinoIDE-badge]: https://img.shields.io/badge/Arduino-IDE-00979D?style=for-the-badge&logo=arduino&logoColor=white
[ArduinoIDE-url]: https://www.arduino.cc/en/software
[AdafruitGFX-badge]: https://img.shields.io/badge/Adafruit-GFX%20Library-orange?style=for-the-badge&logo=adafruit&logoColor=white
[AdafruitGFX-url]: https://github.com/adafruit/Adafruit-GFX-Library
[AdafruitSSD1306-badge]: https://img.shields.io/badge/Adafruit-SSD1306-blueviolet?style=for-the-badge&logo=adafruit&logoColor=white
[AdafruitSSD1306-url]: https://github.com/adafruit/Adafruit_SSD1306
[ESP8266WiFi-badge]: https://img.shields.io/badge/ESP8266WiFi-WiFi%20Library-lightgrey?style=for-the-badge&logo=wifi&logoColor=white
[ESP8266WiFi-url]: https://arduino-esp8266.readthedocs.io/
