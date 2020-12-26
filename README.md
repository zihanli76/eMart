# EMart - eCommerce Platform

> eCommerce platform built with the MERN stack & Redux.

## Project Description

### Background:

This is the course project for CS5610 Web Development Course.

### Contributors:

This project exists thanks to all the people who contribute:  
Xiaoli Ou (Github ID: crystal000),
Zihan Li (Github ID: lzh962733040),
Jun Luo (Github ID: junluo01),
Haozhao Zeng (Github ID: hauser).

### Purpose:

Build an e-commerce system for both managers and users.

![EMart](https://github.ccs.neu.edu/2020FACS5610SV/project-emart/blob/master/uploads/HomeScreen.png)

## Major Features

- **Admin Management**
  - Admin authentication
  - Admin product management
  - Admin user management
  - Admin order management
- **Products Listing, Searching and Filtering**
  - Product pagination
  - Product search feature
  - Top products carousel
  - Product details
  - Product reviews and ratings
- **User Account Management**
  - User sign up/ log in/ log out
  - User profile with orders
- **Full featured Shopping cart**
  - Add products into cart
  - Update products in cart
  - Remove products in cart
- **Order placement and Checkout process**
  - Order placement
  - Checkout process (shipping, payment method)
  - PayPal / credit card integration

## Presentation
   Slides has been uploaded as: project-emart/slides-eMart.pdf. 
   
   Video Length: 18mins. 
   
   Video Link: https://drive.google.com/file/d/1ThpAxC8903fMl55fx8DS23QqvGTDzJOC/view?usp=sharing

   

## Repository Contents

    |------------|                   |-----------|
    |  frontend  |-------------------|  backend  |------------------uploads----package.json----Procfile
    |------------|                   |-----------|
          |- public                        |- controllers
           |- images                       |- models
           |- index.html                   |- middleware
          |- src                           |- utils
           |- actions                      |- config
           |- components                   |- data
           |- screens                      |- seeder.js
           |- constants                    |- server.js
           |- reducers
           |- App.js, index.js, store.js
           |- bootrap.min.css, index.css
          |- build

## Usage

### Install Dependencies (frontend & backend)

```
npm install
sudo npm install -g --force nodemon  #password is needed.
cd frontend
npm install
```

### Run

```
# Run both frontend (:3000) & backend (:5000)
cd ..
npm run dev
```

## Build & Deploy

```
# Create frontend prod build
cd frontend
npm run build
```

There is a Heroku postbuild script, so if pushing to Heroku, no need to build manually for deployment to Heroku

### Deploy to Heroku

```
heroku login
heroku create emartapp
git push heroku master
```

### Link on Heroku

Link: https://emartapp.herokuapp.com/

### Seed Database

You can use the following commands to seed the database with some sample users and products as well as destroy all data

```
# Import data
npm run data:import

# Destroy data
npm run data:destroy
```

```
Sample User Logins

admin@example.com (Admin)
123456

john@example.com (Customer)
123456

jane@example.com (Customer)
123456
```

## License

The MIT License

Copyright (c) 2020 Traversy Media https://traversymedia.com

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in
all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
THE SOFTWARE.
