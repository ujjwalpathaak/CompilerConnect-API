# CompilerConnect-API


## JUIT WebKiosk API

<img alt="Javascript" src="https://img.shields.io/badge/JavaScript-323330?style=for-the-badge&logo=javascript&logoColor=F7DF1E"/> <img alt="Nodejs" src="https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=nodedotjs&logoColor=white"/> <img alt="Puppeteer" src="https://img.shields.io/badge/Puppeteer-40B5A4?style=for-the-badge&logo=Puppeteer&logoColor=white"/>

API for accessing Student Data through JUIT WebKiosk. Created using NodeJS, ExpressJS and Cheerio

BASE URL: https://juit-webkiosk-api-6v2h.onrender.com/

### Required request body

```
{
    "inputCheck": "true", //true || false
    "language": "cpp", //cpp || py
    "code": "",
    "input": "",
}
```

### Endpoints

- `/execCode`  

**Response:**

```
{
    "response": "User 211105 Logged In"
}
```
