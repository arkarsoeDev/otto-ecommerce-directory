# New Day Blog

This is the useage guide for otto ecommerce project. Otto ecommerce is three repositories project.
It include Laravel api, Front Panel (vuejs), and Admin Panel (vuejs). All of them are seperate repository.

## 🔗 Links

#### Laravel api
[https://github.com/arkarsoeDev/otto-ecommerce-api](https://github.com/arkarsoeDev/otto-ecommerce-api)
#### Vuejs Front Panel
[https://github.com/arkarsoeDev/otto-ecommerce-api-client](https://github.com/arkarsoeDev/otto-ecommerce-api-client)
#### Vuejs Admin Panel
[https://github.com/arkarsoeDev/otto-ecommerce-api-admin](https://github.com/arkarsoeDev/otto-ecommerce-api-admin)

## Table of contents

[RunLocally](#run-locally)
- [otto-ecommerce-api(laravel)](#otto-ecommerce-apilaravel)
- [otto-ecommerce-api-client(vuejs)](#otto-ecommerce-api-clientvuejs)
- [otto-ecommerce-api-admin(vuejs)](#otto-ecommerce-api-adminvuejs)
[Screenshot](#screenshot)
[Builtwith](#built-with)
[Author](#author)

## Run Locally

## otto-ecommerce-api(laravel)

Clone the project

```bash
  git clone https://github.com/arkarsoeDev/otto-ecommerce-api.git
```

Go to the project directory

```bash
  cd otto-ecommerce-api
```

Install dependencies

```bash
  composer install
```

Create Database file in database folder

```bash
  database/database.sqlite
```

Copy env file

```bash
  copy .env.example .env
```

Change env setting as below

```bash
  DB_CONNECTION=sqlite
```

Add stripe key of yours in env

```bash
   STRIPE_KEY= //public key
   STRIPE_SECRET= //secret key
```

Create key for project

```bash
  php artisan key:generate
```

Link storage to public storage

```bash
  php artisan storage:link
```

Migrate and seed

```bash
  php artisan migrate:fresh --seed
```

Unzip the images.zip(include in repository), cut thumbnails and uploads folder and paste in public/storage/
(directory should look like below)

```bash
  public/
  -storage/
  --uploads
```

Run the project

```bash
  php artisan serve
```

## otto-ecommerce-api-client(vuejs)

Clone the project

```bash
  git clone https://github.com/arkarsoeDev/otto-ecommerce-api-client.git
```

Install dependencies

```bash
  npm install
```

You can change your api host url in below

```bash
   src/data/axios.js // baseUrl
```

Run the project

```bash
  npm run dev
```

## otto-ecommerce-api-admin(vuejs)

Clone the project

```bash
  git clone https://github.com/arkarsoeDev/otto-ecommerce-api-admin.git
```

Install dependencies

```bash
  npm install
```

You can change your api host url in below

```bash
   src/data/axios.js // baseUrl
```

Run the project

```bash
  npm run dev
```

### Screenshots

### Home

![Alt](/screenshots/front-home.png "Home")

_______________________________________________________________

### Products

![Alt](/screenshots/front-products.png "Products")

_______________________________________________________________

### Product

![Alt](/screenshots/front-product.png "Product")

_______________________________________________________________


### Shopping cart

![Alt](/screenshots/front-shopping-cart.png "Shopping cart")

_______________________________________________________________

### Checkout

![Alt](/screenshots/front-checkout.png "Checkout")

_______________________________________________________________

### Summary

![Alt](/screenshots/front-summary.png "Summary")

_______________________________________________________________

### Admin - Dashboard

![Alt](/screenshots/admin-dashboard.png "Admin - Dashboard")

_______________________________________________________________

### Admin - Products

![Alt](/screenshots/admin-products.png "Admin - Products")

_______________________________________________________________

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- Grid
- Mobile-first workflow
- Scss
- [Vue](https://vuejs.org/) - JS library

## Author

- Github - [@arkarsoeDev](https://github.com/arkarsoeDev)