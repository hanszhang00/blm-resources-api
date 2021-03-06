# BLM-information-site


[![Open Source Love](https://badges.frapsoft.com/os/v1/open-source.svg?v=103)](https://github.com/ellerbrock/open-source-badges/) [![MIT Licence](https://badges.frapsoft.com/os/mit/mit.svg?v=103)](https://opensource.org/licenses/mit-license.php)


<p align="center">
  <img
    src="assets/readme/banner.png"
    alt="backend readme background"
  />
</p>

<!-- short description -->
<p align="center">
  BLM Information Site Backend ♥️</a>
</p>

<p align="center">
  <strong>
    Live <a href="www.blmresources.online"> here</a>
    <br /> ✊🏿 
  </strong>
</p>

## Use

This is the backend of [**BLM-information's website**](https://github.com/hanszhang00/blm-resources).

**It can be utilized in three ways:**
- for developers who want to improve on the backend through a local copy
- for anyone to add more content and resources to the website directly
- for developers to query BLM-related data with RESTful endpoints

## Tech Stack

The backend is a Strapi server out of the box, with content data added throught the Strapi dashboard.

Strapi is a Node.js based headless CMS. Strapi is super easy to use and it has a super awesome UI. Please check out its website [**here**](https://strapi.io/)!

**Google Cloud PostGresSQL service** is used to store all of the data for the production encironment. All of the production-ready data is managed in the database. The local server uses a seperate database (SQLite) and thus is not synced with the production database due to security concerns. 

**Google Cloud** is also used for project's deployment.

## Contributing content

If you are interested in contributing more content, you need to have an admin account to get access to the Strapi console. Contact me [**here**](mailto:hanszhang2000@gmail.com) and I'm happy to send you the email and password.

Currently we have three types of resourceces, BLM-related organizations, videos, and articles.

- Firstly, go to the Strapi admin page at **http://www.blmresources.online/admin**

<img src="assets/readme/loging-page.png">

- Log in with the given email and passowrd, it will take you to the main console

<img src="assets/readme/main-console.png">

- Now, you can update the content of any content type. **Please do not** delete any existing resources and only add new ones.

<img src="assets/readme/new-entry.png">

- In the production server, you are not able to add any media resources (image, video, etc). Feel free to leave the entry for images blank. You are also not able to alter the content type (you are **only allowed to do it in the local server**). I will sync up the local and production server periodally, and add any media resources as fit. Then these new changes will be reflected in the actual frontend Gatsby page!

## API endpoints

Any developers wishing to incorprate relavant BLM resources into their own projects is able to do so using our RESTful endpoints.

The three main endpoints for our projects are:

- **http://www.blmresources.online/orgs**
- **http://www.blmresources.online/articles**
- **http://www.blmresources.online/videos**

You can retrieve a specific item of each category by adding`/id` to each request, where id
id the specfic item id (integer starting from 1).

You are able to know how many entries there are for each category by adding `/count` to each request, for example:
- **http://www.blmresources.online/videos/count**

## Creating, deleting, and updating entries

Creating, deleting, and updating entries directly through API requests are not allowed for security purposes. **If you have admin access** (see above), you can do any of the above directly throug the Strapi console.

## Contributing

This project is an open-source project. So any suggestion or feature requests are welcome. You are submit an issue directly in the project's issue page.


## Disclaimer

I have created this website in hope that more people will become educated in the BLM movement. However, the content I have cited and used might not be accurate due to typing errors, and some information might be outdated. I'm always open to correction, feedback, and improvement with good intention. Please use the website and the resources with your own discretion.

## License

See the [**LICENSE**](/LICENSE.md) file for license rights and limitations (MIT).






