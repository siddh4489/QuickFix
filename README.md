
![A4 Banner](./public/images/Accounted4__Logo_QB.png)]
Accounted4 LLC - QuickFix
==========================================================

## Overview

This application is built using Node.js and Express Framework.  Users are Authorized and Authenticated using Intuit's OAuth2.0 Client library.
Datatbales is the Frontend Library 


## Installation

### Requirements

* [Node.js](http://nodejs.org) >= 7.0.0
* [Intuit Developer](https://developer.intuit.com) Account

### Via Github Repo (Recommended)

```bash
$ cd quickfix
$ npm install
```

## Configuration

Copy the contents from `.env.example` to `.env` within the sample directory:
```bash
$ cp .env.example .env
```
Edit the `.env` file to add your:  


* **PORT:(optional)** Optional port number for the app to be served
* **NGROK_ENABLED:(optional)** By default it is set to `false`. If you want to serve the Sample App over HTTPS ( which is mandatory if you want to test this app using Production Credentials), set the variable to `true`



### TLS / SSL (**optional**)

If you want your enpoint to be exposed over the internet. The easiest way to do that while you are still developing your code locally is to use [ngrok](https://ngrok.com/).  

You dont have to worry about installing ngrok. The sample application does that for you.   
1. Just set `NGROK_ENABLED` = `true` in `.env` 


## Usage

```bash
$ npm start
```

### Without ngrok (if you are using localhost i.e `NGROK_ENABLED`=`false` in `.env`)
You will see an URL as below:
```bash
💳 Step 1 : Paste this URL in your browser : http://localhost:8000
💳 Step 2 : Copy and Paste the clientId and clientSecret from : https://developer.intuit.com
💳 Step 3 : Copy Paste this callback URL into `redirectURI` : http://localhost:8000/callback
💻 Step 4 : Make Sure this redirect URI is also listed under the Redirect URIs on your app in : https://developer.intuit.com
```

### With ngrok (if you are using ngrok i.e `NGROK_ENABLED`=`true` in `.env`)

Your will see an URL as below : 
```bash
💳 Step 1 : Paste this URL in your browser :  https://9b4ee833.ngrok.io 
💳 Step 2 : Copy and Paste the clientId and clientSecret from : https://developer.intuit.com
💳 Step 3 : Copy Paste this callback URL into `redirectURI` : https://9b4ee833.ngrok.io/callback
💻 Step 4 : Make Sure this redirect URI is also listed under the Redirect URIs on your app in : https://developer.intuit.com
```

Click on the URL and follow through the instructions given in the sample app.


## Links

Project Repo

* https://dev.azure.com/shealy/Accounted4/_git/QuickFix

Intuit OAuth2.0 API Reference

* https://developer.intuit.com/app/developer/qbo/docs/develop/authentication-and-authorization/oauth-2.0

Intuit OAuth2.0 Playground

* https://developer.intuit.com/app/developer/playground



