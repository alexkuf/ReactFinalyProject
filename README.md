## Fenestra

<div align="center">
  <a href=""https://github.com/alexkuf/reactFinalyProject/assets/111445523/15e6980d-55e5-4587-b10d-7e43965f66f8">
  
  </a>

  <h3 align="center">Fenestra Project Manager</h3>

![about1](https://github.com/alexkuf/reactFinalyProject/assets/111445523/a4ea90de-1121-4d42-9485-156fd04aa9fe)

<a 
href="https://animated-halva-f26411.netlify.app/">View Demo website without server</a>

</div>
<!-- ABOUT THE PROJECT -->

## About The Project

This is a closed application intended for small companies. Only
company employees have the opportunity to enter the application.
Only administrator can add users.

### Built With

[![React][React.js]][React-url] [![Node][Node.js]][Node-url] [![MongoDB][MongoDB]][MongoDB-url] [![Express][Express.js]][Express-url] [![Bcrypt][Bcrypt.js]][Bcrypt-url] [![JWT][JWT]][JWT-url] [![joi][joi]][joi-url] [![Morgan][Morgan]][Morgan-url]
[![Mongoose][Mongoose.js]][Mongoose-url] [![Axios][Axios]][Axios-url] [![Cors][Cors]][Cors-url] [![Bootstrap][Bootstrap]][Bootstrap-url]
[![Excel][Excel]][Excel-url] [![Dotenv][Dotenv]][Dotenv-url] [![regexp][regexp]][regexp-url] [![ReactToastify][ReactToastify]][ReactToastify-url] [![ReactSwitch][ReactSwitch]][ReactSwitch-url]

<!-- GETTING STARTED -->

### More info

```
_Opportunities in the application for users:_

1. Create projects (Options to get started project)
2. Delete projects (Only your projects)
3. Edit projects (Only time)
4. Search by project
5. Separate page for your projects
6. Extra bonus: To-do list for every day, and saved to your
   local computer

_Opportunities in the application for administrator:_

1. Create projects (Options to get started project)
2. Delete projects (Only your projects)
3. Edit projects (Only time)
4. Create user
5. Delete user
6. Edit user
7. Change user password
8. Create and save reports in Excel file
9. Extra bonus: To-do list for every day, and saved to your
   local computer

```

### Installation

_Install NPM packages_

1.

```sh
  npm install
```

### Starting

_Run dev server:_

```sh
npm run dev
```

_Run frontend app:_

```sh
npm run start
```

## User model

```
const userSchema = new mongoose.Schema({
  name: {
    type: String,
    required: true,
    minlength: 2,
    maxlength: 255,
  },
  email: {
    type: String,
    required: true,
    minlength: 6,
    maxlength: 255,
    unique: true,
  },
  password: {
    type: String,
    required: true,
    minlength: 6,
    maxlength: 1024,
  },
  isAdmin: {
    type: Boolean,
    required: true,
  },
  createdAt: { type: Date, default: Date.now },
  cards: Array,
});
```

## Project model

```
const cardSchema = new mongoose.Schema({
  projectName: {
    type: String,
    required: true,
    minlength: 2,
    maxlength: 255,
  },
  employeeName: {
    type: String,
    required: true,
    minlength: 2,
    maxlength: 1024,
  },
  createAt: {
    type: String,
    required: true,
  },
  startTime: {
    type: String,
    required: true,
    minlength: 2,
    maxlength: 255,
  },
  stopTime: {
    type: String,
    required: true,
    minlength: 2,
    maxlength: 255,
  },
  actions: {
    type: String,
    required: true,
    minlength: 2,
    maxlength: 255,
  },
  revision: {
    type: String,
    required: true,
    minlength: 2,
    maxlength: 255,
  },

  user_id: { type: mongoose.Schema.Types.ObjectId, ref: "User" },
});
```

## Progect name model

```
const projectnameSchema = new mongoose.Schema({
  name: {
    type: String,
    required: true,
    minlength: 2,
    maxlength: 255,
  },

  user_id: { type: mongoose.Schema.Types.ObjectId, ref: "User" },
});

```

<!-- MARKDOWN LINKS & IMAGES -->
<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->

[React.js]: https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB
[React-url]: https://reactjs.org/
[Node.js]: https://img.shields.io/badge/node.js-000000?style=for-the-badge&logo=nextdotjs&logoColor=white
[Node-url]: https://nodejs.org/
[MongoDB]: https://img.shields.io/badge/mongoDB/Atlas-20232A?style=for-the-badge&logo=mongoDB&logoColor=green
[MongoDB-url]: https://www.mongodb.com/
[Express.js]: https://img.shields.io/badge/Express.js-35495E?style=for-the-badge&logo=expressjs&logoColor=4FC08D
[Express-url]: https://expressjs.com/
[Bcrypt.js]: https://img.shields.io/badge/Bcrypt.js-DD0031?style=for-the-badge&logo=bcrypt&logoColor=white
[Bcrypt-url]: https://yepcode.io/
[JWT]: https://img.shields.io/badge/JWT-4A4A55?style=for-the-badge&logo=jwt&logoColor=FF3E00
[JWT-url]: https://jwt.io/
[joi]: https://img.shields.io/badge/joi-FF2D20?style=for-the-badge&logo=joil&logoColor=white
[joi-url]: https://joi.dev/
[Morgan]: https://img.shields.io/badge/Morgan-563D7C?style=for-the-badge&logo=morgan&logoColor=white
[Morgan-url]: https://coralogix.com/
[Mongoose.js]: https://img.shields.io/badge/Mongoose-0769AD?style=for-the-badge&logo=mongoose&logoColor=white
[Mongoose-url]: https://mongoosejs.com/
[Axios]: https://img.shields.io/badge/Axios-8A2BE2?style=for-the-badge&logo=Axios&logoColor=white
[Axios-url]: https://www.npmjs.com/package/axios
[Cors]: https://img.shields.io/badge/Cors-0769AD?style=for-the-badge&logo=cors&logoColor=white
[Cors-url]: https://www.npmjs.com/package/cors
[Bootstrap]: https://img.shields.io/badge/Bootstrap-0769AD?style=for-the-badge&logo=Bootstrap&logoColor=white
[Bootstrap-url]: https://getbootstrap.com/
[Excel]: https://img.shields.io/badge/Excel(xlsx)-44cc11?style=for-the-badge&logo=Excel(xlsx)&logoColor=green
[Excel-url]: https://www.npmjs.com/package/xlsx
[Dotenv]: https://img.shields.io/badge/.env-ecd53f?style=for-the-badge&logo=.env&logoColor=white
[Dotenv-url]: https://www.npmjs.com/package/dotenv
[regexp]: https://img.shields.io/badge/RegExP(.*)-e75223?style=for-the-badge&logo=RegExP(.*)&logoColor=green
[regexp-url]: https://www.npmjs.com/package/regexp
[ReactToastify]: https://img.shields.io/badge/React-(Toastify)-e75223?style=for-the-badge&logo=React-(Toastify)&logoColor=e75223
[ReactToastify-url]: https://www.npmjs.com/package/react-toastify
[ReactSwitch]: https://img.shields.io/badge/React-(switch)-0769AD?style=for-the-badge&logo=React-(switch)&logoColor=0769AD
[ReactSwitch-url]: https://www.npmjs.com/package/react-switch
