----------

<div id="top"></div>

<!-- PROJECT SHIELDS -->
[![Contributors][contributors-shield]][contributors-url]
[![Forks][forks-shield]][forks-url]
[![Stargazers][stars-shield]][stars-url]
[![Issues][issues-shield]][issues-url]
[![MIT License][license-shield]][license-url]



<!-- PROJECT INTRO -->
<br />
<div align="center">
  <h1 align="center">Metadata Parser</h1>
  <p align="center">
    ⚡️ Pull data from web links, including title, description, photos, videos, and more [via OpenGraph]
    <br />
    <br />
    <a href="https://github.com/LinkviteApp/metadata-parser">View Demo</a>
    ·
    <a href="https://github.com/oLinkviteApp/metadata-parser/issues">Report Bug</a>
    ·
    <a href="https://github.com/LinkviteApp/metadata-parser/issues">Request Feature</a>
  </p>
</div>



<!-- TABLE OF CONTENTS -->
<details>
  <summary>Table of Contents</summary>
  <ol>
    <li>
      <a href="#about">About The Project</a>
    </li>
    <li>
      <a href="#getting-started">Getting Started</a>
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
## About

This package lets you to use Facebook OpenGraph tags to extract information from an HTTP web address and retrieve meta data like title, description, photos, videos, and more. 



<!-- GETTING STARTED -->
## Getting Started

1. Clone the repo
   ```sh
   $ git clone https://github.com/linkvite/metadata-parser.git
   ```
2. Install go mods
   ```sh
   $ go mod
   ```
3. Run the server
   ```sh
   $ go run .
   ```



<!-- USAGE EXAMPLES -->
## Usage

Once the program is running, you'll get:
```sh
👋 Enter the url of the web page 👇
================================================================
```
Next provide the link you want to parse.
```sh
👋 Enter the url of the web page 👇
================================================================
https://github.com
```


### ✅ Success Response
If you provided a valid url, you'd get a response that looks like this:
```sh
✅ Valid URL provided.
================================================================
✅ Generated meta data template.
================================================================
⏳ Updating meta data from html document...
================================================================
✅ Updated meta data from html document.
================================================================
⏱  Total time taken: 494 milliseconds.
================================================================
📋 Meta data:
================================================================
```

```json
{
  "name": "GitHub",
  "title": "GitHub: Where the world builds software",
  "description": "GitHub is where over 83 million developers shape the future of software, together. Contribute to the open source community, manage your Git repositories, review code like a pro, track bugs and feat...",
  "domain": "github.com",
  "url": "https://github.com/",
  "type": "object",
  "images": ["https://github.githubassets.com/images/modules/site/social-cards/github-social.png"],
  "favicons": ["https://github.githubassets.com/favicons/favicon.svg"]
}
```


### ❌ Error Response
**PS** All links must be of scheme `http` or `https`. An error response would look like this:

```sh
👋 Enter the url of the web page 👇
================================================================
github.com
================================================================
❌ Failed to parse the url. Reason: The url must be a http or https url.
================================================================
```



<!-- ROADMAP -->
## Roadmap

- [x] Parse any website
- [x] Return custom reponse
- [x] Retrieve favicons
- [x] Retrieve multiple images

See the [open issues](https://github.com/LinkviteApp/metadata-parser/issues) for a full list of proposed features (and known issues).



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



<!-- LICENSE -->
## License

Distributed under the MIT License. See `LICENSE.txt` for more information.



<!-- CONTACT -->
## Contact

Feel free to reach out at [@tryLinkvite](https://twitter.com/tryLinkvite) or [@kayode0x](https://twitter.com/kayode0x)  on twitter.



<!-- ACKNOWLEDGE -->
## Acknowledgments
+ 💡 Inspired by [link-preview-js](https://github.com/ospfranco/link-preview-js)
+ 🛠 Built on top of [goquery](github.com/PuerkitoBio/goquery)
+ ⚡️ Written in [Go](https://go.dev/).
+ 📝 MD Template was from [here](https://github.com/othneildrew/Best-README-Template)


<p align="right">(<a href="#top">back to top</a>)</p>

<!-- MARKDOWN LINKS & IMAGES -->
<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
[contributors-shield]: https://img.shields.io/github/contributors/linkviteApp/metadata-parser.svg?style=for-the-badge
[contributors-url]: https://github.com/LinkviteApp/metadata-parser/graphs/contributors
[forks-shield]: https://img.shields.io/github/forks/linkviteApp/metadata-parser.svg?style=for-the-badge
[forks-url]: https://github.com/LinkviteApp/metadata-parser/network/members
[stars-shield]: https://img.shields.io/github/stars/linkviteApp/metadata-parser.svg?style=for-the-badge
[stars-url]: https://github.com/LinkviteApp/metadata-parser/stargazers
[issues-shield]: https://img.shields.io/github/issues/linkviteApp/metadata-parser.svg?style=for-the-badge
[issues-url]: https://github.com/LinkviteApp/metadata-parser/issues/new?labels=enhancement
[license-shield]: https://img.shields.io/github/license/linkviteApp/metadata-parser.svg?style=for-the-badge
[license-url]: https://github.com/LinkviteApp/metadata-parser/blob/main/LICENSE.txt