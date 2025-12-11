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
    <img src="images/comsubpac-logo.png" alt="COMSUBPAC Logo" width="120">
  </a>

<h3 align="center">4-Mode Wi-Fi Scanner</h3>

<p align="center">
    A portable ESP8266 Wi-Fi scanning tool with OLED display.
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
## 4 mode WIFI scanner
The **4-Mode Wi-Fi Scanner** is a portable ESP8266-based scanning tool with a 0.96" SSD1306 OLED display.  
It surveys nearby Wi-Fi networks across four modes:

- **Mode 0:** Lists SSID, RSSI, channel, encryption type, and local IP.  
- **Mode 1:** Measures dBm levels of nearby APs and selects the strongest one.  
- **Mode 2:** Sweeps all channels and records average RSSI/traffic.  
- **Mode 3:** Identifies connected clients on the current Wi-Fi network and prints their IPs.

[![Product Name Screen Shot][product-screenshot]](https://example.com)

<p align="right">(<a href="#readme-top">back to top</a>)</p>


### Built With

[![ESP8266][ESP8266-badge]][ESP8266-url]
[![ArduinoIDE][ArduinoIDE-badge]][ArduinoIDE-url]
[![AdafruitGFX][AdafruitGFX-badge]][AdafruitGFX-url]
[![AdafruitSSD1306][AdafruitSSD1306-badge]][AdafruitSSD1306-url]
[![ESP8266WiFi][ESP8266WiFi-badge]][ESP8266WiFi-url]

<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- GETTING STARTED -->
## Getting Started

### Prerequisites
- Arduino IDE installed  
- ESP8266 board package installed  
- Libraries installed:  
  - ESP8266WiFi  
  - Adafruit GFX  
  - Adafruit SSD1306  

### Software Installation

1. Clone the repo:
   ```sh
   git clone https://github.com/Skippertheev/COMSUBPAC-Personal-Projects.git
2. Open the project folder
3. Open the file `wifi_scanner.ino` in Arduino IDE
   ```js
   const WIFISSD= 'YOUR_SSD';
   ```
   ```js
   const password= 'YOUR_PASSWORD';
   ```
4. upload the sketch

### Hardware Installation

1. follow the wiring diagram and provide ensure wiring is accurate

2. Perfboard? TODO

<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- USAGE EXAMPLES -->

## Usage

### Controls
- Button A: Cycle through modes
- Plug in either battery or usb-C 5V power supply

### Display Output
Each mode prints its results to the OLED.

### Serial Monitor
Debug logs can be viewed through Serial Monitor at 115200 baud.


<!-- ROADMAP -->
## Roadmap
TODO
- [ ] Add battery-powered enclosure
- [ ] Add SD logging for scans
- [ ] Add ESP32 version

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

Evan Zhang
Linkedin: [@linkedin handle](linkedin.com/in/evan-zhang-47432b25a)
Email: ezhang.2017@outlook.com
Project Link: [https://github.com/Skippertheev/COMSUBPAC-Personal-Projects](https://github.com/Skippertheev/COMSUBPAC-Personal-Projects)

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
[Next.js]: https://img.shields.io/badge/next.js-000000?style=for-the-badge&logo=nextdotjs&logoColor=white
[Next-url]: https://nextjs.org/
[React.js]: https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB
[React-url]: https://reactjs.org/
[Vue.js]: https://img.shields.io/badge/Vue.js-35495E?style=for-the-badge&logo=vuedotjs&logoColor=4FC08D
[Vue-url]: https://vuejs.org/
[Angular.io]: https://img.shields.io/badge/Angular-DD0031?style=for-the-badge&logo=angular&logoColor=white
[Angular-url]: https://angular.io/
[Svelte.dev]: https://img.shields.io/badge/Svelte-4A4A55?style=for-the-badge&logo=svelte&logoColor=FF3E00
[Svelte-url]: https://svelte.dev/
[Laravel.com]: https://img.shields.io/badge/Laravel-FF2D20?style=for-the-badge&logo=laravel&logoColor=white
[Laravel-url]: https://laravel.com
[Bootstrap.com]: https://img.shields.io/badge/Bootstrap-563D7C?style=for-the-badge&logo=bootstrap&logoColor=white
[Bootstrap-url]: https://getbootstrap.com
[JQuery.com]: https://img.shields.io/badge/jQuery-0769AD?style=for-the-badge&logo=jquery&logoColor=white
[JQuery-url]: https://jquery.com 


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

