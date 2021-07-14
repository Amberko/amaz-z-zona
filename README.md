1. Introdaction – AMAZ-Z-ZONA

https://amaz-z-zona.herokuapp.com/

https://amaz-z-zona.herokuapp.com/api/users/createadmin

GIT

https://git.heroku.com/amaz-z-zona.git

GitHub

https://github.com/Amberko/amaz-z-zona

Amaz-z-zona - MongoDB

mongodb+srv://amaz-z-zona:zzz3zzz@mika-mongo-db.2ndnx.mongodb.net/amaz-z-zonaDB?retryWrites=true

.env file

MONGODB_URL=mongodb://localhost/jsamazona

JWT_SECRET=somethingsecret

PAYPAL_CLIENT_ID=db

Run Backend

npm install

npm run build

npm start

Run Frontend

npm install

npm start

OPIS:

Kreiran je e-commerce sajt nalik na Amazon.com

Osnovni alati : Vanilla JavaScript and Node.JS, ExpressJS and MongoDB

Steko sam iskustvo u pravljenu kompletnog "responsive" sajta, od "user-friendly" dizjana, backend and frontend produkcije, autorizacije, I postavljanja na web preko Heroku servera..

-Web Design

HTML5,

CSS3 including Semantic Elements,

Flexbox,

Grid System

and Response Design.

Frontend Development

Pure JavaScript including ES6 Syntax,

Array Functions,

Rendering System,

Single Page App,

Libraries for Date Time,

drawing chart and etc.

Backend Development

Node and MongoDB (Mongoose, Aggregation)

ExpressJS,

JWT Authentication,

Mongoose object data modeling,

Web API, Body Parser,

File Upload and more.

Development:

ESLint,

Babel,

Git,

Github,

Deployment: Heroku

APP Features

Home Screen

Static Web Page Design

CSS Grid to create website layout

Flexbox to shape product thumbnails and responsive design

Product Screen

create single page application

Create buttons and add events to buttons

Cart Screen

Save and retrieve data in local storage

Master in javascript array functions

Use combo box and add event to it

re-render screen based on changes in item count

Sign-in and Register Screen

Create dynamic form

Input validation in frontend and backend

Create web server using node.js

Connect to Mongodb database

Add registered user to the database

Authenticate user based on email and password

Using Jsonwebtoken to authorize users

Shipping and Payment Screen

Create wizard form to get user data in multiple steps

Save user info in the local storage

Place Order Screen

Validate and create order in the database

Order Screen

Payment with paypal

Show order state based on user and admin activities

Profile Screen

Create authenticated routes

enable user to update their informations

enable user to logout and clear local storage

show list of orders to user and link it to details

Dashboard Screen

Create professional dashboard using pure CSS

Using chart library to show sales information

Order Screen

Enable admin to mange orders

show loading message and alert message

Product Screen

enable admin to manage products

upload product images to server

Strat e-commerce development

Create Folder Structure

Design Website Template

Create Static Home Screen

Development Setting

Add Webpack to Frontend

Install Babel For ES6 Syntax (backend - root)

Enable Code Linting (ESLint)

Install VSCode Extensions

JavaScript

Render Dynamic Home Screen

Build Url Router

NodeJS

Create Node.JS Server

Load Products From Backend

Product Screen

Create Rating Component

Product Screen

Product Screen UI

Product Screen Action

Shopping Cart

Add To Cart Action

Cart Screen UI

Update and Delete Cart Items

MongoDB

Connect To MongoDB and Create Admin User

User Authentication

Sign-in Screen UI

Sign-in Screen Backend

Sign-in Screen Action

Create Progress Indicator and Alert Component

Register Screen

User Profile Screen

Checkout Wizard

Checkout Wizard Screen

PlaceOrder Screen UI

PlaceOrder Screen Action

Complete Order

Order Details Screen

PayPal Payment

Display Orders History

Admin Products

Admin Dashboard UI

Admin Products UI

Create Product API

Edit Product Screen UI

Edit Product Backend

Upload Product Image

Build Project (build scripts)

Delete Product

Admin Orders

Admin Orders / List orders / Delete orders

Deliver Order / Edit orders

Dashboard Chart

Show Summary Report in Dashboard

Show Chart in Dashboard

Deploy Website

Publish on Heroku

EXTRA:

Product Search bar

Show categories in Sidebar Menu

CODE structure - JSAMAZZZONA folder

.vscode

Settings.json

Dist (Copy of Backend)

Backend

Config.js

Data.js

Server.js

Utils.js

Models

OrderModel.js

ProductModel.js

UserModel.js

Routers

OrderRouter.js

ProductRouter.js

UserRouter.js

UploadRouter.js

Frontend

Index.html

Package.json

Style.css

Images

Image-1.jpg

Image-2.jpg

Image-3.jpg

Node_modules

Src

api.js

config.js

Index.js

LocalStorage.js

Utils.js

Components

CheckoutSteps.js

DashboardMenu.js

Header.js

Rating.js

Screens

CartScreen.js

DashboardScreen.js

Error404Screen.js

HomeScreen.js

OrderListScreen.js

OrderScreen.js

PaymentScreen.js

PlaceOrderScreen.js

ProductEditScreen.js

ProductListScreen.js

ProductScreen.js

ProfileScreen.js

RegisterScreen.js

ShippingScreen.js

SigninScreen.js

Node_modules

Uploads

File.txt

Image-1.jpg

Image-2.jpg

Image-3.jpg

ROOT files:

-     .babelrc

- .env

-     .eslintrc.js

-     .gitignore

-     package.json

-     Procfile

-     .git

---

Sections:

---> Strat e-commerce development <---

--> Prvo kreiramo osnovnu strukturu (ROOT) foldera..

--> install node.js

--> root/backend/frontend

--> “npm init” and package.json

--> Index.html

--> live-server"

--> Dizajniramo (prikaz) osnovnu strukturu sajta

--> Create Static Home Screen (RESPONSIVE)

2. Prvo kreiramo osnovnu strukturu (ROOT) foldera..

Za backend cemo koristiti/instalirati Node.js I npm manager

“npm init” and package.json

Prilikom kreiranja NOVOG projecta, neophodno je napraviti package.json fajl, uz pomoc komande “npm init”

Tu komandu za pocetak pokrecemo preko terminala na putanji ---> nasProjekat/frontend ILI “cd frontend”

U frontendu kreiramo index.html

Html:5 + TAB kreira osnovnu strukturu html dokumenta

Finalni Index.html ce sadrzati:

linkove za:

style.css

font-awesome

chartist.js

Osnovnu struturu aplikacije/sajta

Header

Main

Footer

Takodje I “Loading div” and “message div”

Scriptu za src="main.js"

npm install -D live-server" na “cd frontend”

"start": "live-server src --verbose",

Koristimo samo na pocetku, kasnije koristimo webpack

3. Dizajniramo (prikaz/css) osnovnu strukturu sajta

U index.html kreiramo div.grid-container koji obuhvata SVE:

header | main | footer

Kreiramo style.css u frontend folderu,

I kreiramo link ka tom css fajlu u index.html

---> style.css

|| \* || html || body

|| header || header a || header a:hover

|| .brand a || footer

Postavljamo box-sizing: border-box; za sve elemente naseg sajta \*, sto ce nam olaksati rad sa elementima..

Prvo za sav html (celu applikaciju) postavljamo velicinu slova na 1rem (10px)

Html {

    font-size: 62.5%; 	/* 16px * 62.5 =   10px = 1rem */

}

Zatim ceo body postavljamo da koristi 1.6rem za velicinu slova sto je isto ko defoultnih 16px

Height postavljamo na 100vh tj visina ce uvek biti 100% trenutnog prikaza..Sadrzaj ce biti prikazan u celosti, samo ce se skalirati u odnosu na velicinu prikaza..

Marginu za celu aplikaciju postavljamo na 0..

Body {

    height: 100vh;

    font: 1.6rem Helvetica, Arial; 		/* 1.6rem = 16px */

    margin: 0;

}

https://css-tricks.com/fun-viewport-units/

GRID layout koristimo za respored glavnih elemenata na stranici

.grid-container{

display: grid;

grid-template-areas:

'header'

'main'

'footer';

grid-template-columns: 1fr;

grid-template-rows: 5rem 1fr 5rem; /_ header main footer _/

height: 100%;

}

https://css-tricks.com/snippets/css/complete-guide-grid/

|| header || header a || header a:hover || .brand a || footer

FLEX (justify-content, align-items, flex: 2 1 60rem;..)

koristimo za raspored elemenata unutar glavnih GRID elemenata:

grid-area: header | main | footer

Primeri koriscenja FLEXa u kasnijem codu:

flex: <'flex-grow'> <'flex-shrink'> <'flex-basis'>

.details-image { flex: 2 1 60rem; }

2: 🡪 Ako podelimo stranicu na 4 dela velicina slike neka bude 2 dela

1: 🡪 Neka bude _shrinkable_

60rem: 🡪 Sirina neka bude 60x10 = 600px

flex: 0 1 30rem;

/* postavlja MAX sirinu 30*10px = 300px \*/

https://css-tricks.com/almanac/properties/f/flex/

4. Create Static HomeScreen (RESPONSIVE)

Create _images_ folder in src and add some pictures

Za pocetak dodajemo listu proizvoda directno/rucno/static u <main> section

style ul. products and internal divs

( FLEX, flex-wrap, flex-direction, justify-content and flex: 0 1 30rem (max sirina))

5.       style EVERY -->  a and a:hover

text-decoration: none, color: black or orange when hovered

---

---> Development Setting <---

--> Webpack

--> AXIOS

--> Babel

--> NODEMON

--> ESLint

--> ES6/ES7 snippets

--> Prettier

--> CSS Peek

--> grammar injections

9.  Add Webpack to Frontend + AXIOS

    1.       npm install –D webpack  webpack-cli  webpack-dev-server  (frontend)

    2.       “start”: “webpack-dev-server  –mode  development  –watch-content-base  –open”

    3.  npm install axios (frontend)

10. Install Babel For ES6 Syntax (backend - root) + NODEMON

    1.       npm install -D @babel/core  @babel/cli  @babel/node  @babel/preset-env

    2.       create .babelrc file in root

{

"presets": [

    [

      "@babel/preset-env",

      {

        "targets": {

          "node": "current"

        }

      }

    ]

]

}

    3. 	npm install -D nodemon (root)

    4. 	set start: nodemon  --watch backend –exec babel-node backend/server.js

    5. 	npm start

11. Enable Code Linting (ESLint)

    1.  npm install –D eslint (root)

    2.       install VScode extension “ESLint”

    3.       create  .eslintrc.js  (in root folder)

    4.       in .eslintrc.js  file define setting for ESLint

module.exports = {

env:{ browser: true, node: true, es2020: true, },

extends: [‘airbnb-base’],

parserOptions: { sourceType:'module', ecmaVersion: 11, },

rules: { 'no-console': 0, 'no-underscore-dangle': 0,

     'eol-last': ['error', 'never'], },

}

    5. 	npm install –D  eslint-config-airbnb-base  eslint-plugin-import

    6. 	(ctrl + shift + P) type eslint and choose disable and again ENABLE

    7. 	(ctrl + shift + P) type eslint EDIT settings.json file

( .formatOnSave – true and .codeActionsOnSave – true)

    8. 	ctrl + S  will fix all ESLint errors

12. Install VSCode Extensions

    1.       JS (ES6) code snippets

    2.       ES7 React?Redux/GraphQL/React-Native snippets

    3.       Prettier – Code formatter

Fix compatability issue with eslint

npm install –D eslint-config-prettier ( ESLint and Prettier compatibility )

nside .eslintrc.js

 extends  add ‘prettier’

    4. 	HTML&LESS grammar injections ( VERY IMPORTANT - Template literals `…`)

    5. 	CSS Peek

---

<--- NodeJS --->

--> Create Node.JS Server (express + CORS )

--> npm init in root

--> npm install express

--> create server.js

--> Import/use/listen express

--> app.get(PRODUCTS)

--> Install/import/use CORS

--> Load Products From Backend ( ne treba vise )

7.  Create Node.JS Server (express)

           1. 	run npm init in root jsamazona folder (defoult)

Kreiramo celu nasu aplikaciju ( ROOT jsamazona folder ) kao NODE project

    2. 	npm install express

    3. 	create server.js  --->  backend folder

Get ACCESS to express package

import express from 'express';

and RUN express

const app = express();

Da bi radio express web SERVER, moramo da mu kazemo na kom portu da osluskuje promene:

app.listen(5000, () => {

console.log('serve at http://localhost:5000');

});

Kako bi pokrenuli server, u package.json u ROOT folderu, dodajemo komandu:

--> "start": "node backend/server.js"

Zatim pokrecemo tu npm start comandu u ROOT terminalu, cime se startuje rad nase aplikacije

U slucaju bilo koje izmene na CODE-u, server mora da se ubije I ponovo pokrene

4.       use/import CORS on backend/server.js ( npm install cors – in root folder

Install - npm install cors (root)

Import

Use - app.use(cors());

CORS Error ---> https://medium.com/@dtkatz/3-ways-to-fix-the-cors-error-and-how-access-control-allow-origin-works-d97d55946d9

    5.	Restar server ---> Kill server + npm start



     6. 	server.js ---> app.get(PRODUCTS)

Kako bi dobili sve proizvode sa backenda/DBa, prvo Importujemo data.js

First import data from './data.js'; (backend)

Zatim kreiramo jednostavnu rutu

By using app.get() send back those products to API (frontend) on this adress http://localhost:5000/api/products

app.get('/api/products', (req, res) => {

res.send(data.products);

});

Na adresi http://localhost:5000/api/products, dobicemo podatke u JSON formatu, cije pojedinacne delove ili sve podatke dalje mozemo da koristimo i u zeljenom obliku vratimo/prikazemo krajnem korisniku..

---

---> JavaScript <---

--> Render Dynamic Home Screen

--> backend data.js

--> HomeScreen.js

--> AXIOS / async / await

--> `template literals` AND ${ value }

--> products.map((product))

--> Build Url Router

--> index.js (src)

--> ProductScreen.js

--> screens/Error404.js

--> Import ProductScreen and HomeScreen

--> utils.js ( parseRequestURL() )

--> routes { }

--> router = async () => {

    	const request

    	const parseURL

    	const screen

    	const main

}

--> window.addEventListener(‘load’, router);

--> window.addEventListener('hashchange', router);

5.  Render Dynamic HomeScreen

    1.       create in backend data.js ---> products

\_id, name, category, image, price, brand, raiting, numReviews, countInStock

    2. 	create screens/HomeScreen.js

IMPORT axios

kako bi DINAMICKI prikazali sve popdatke vezane za prozivode, te podatke moramo prvo preuzeti od negde ---> backend/data.js or MongoDB

render: async () => {

const response = await fetch(URL, { ---> FETCH

const response = await axios({

url: 'http://localhost:5000/api/products',

headers: {

'Content-type': 'application/json',

},

});

if (!response || !response.ok) { ---> FETCH

if (!response || response.statusText !=='OK') {

      				return `<div>Error in getting data</div>`;

    			}

const products = response.data;

const products = await response.json(); ---> FETCH

return `template literal`

}

Zatim dobijene podatke svakog jedinstvenog proizvoda products.map((product) smestitamo u sablon `…` na odgovarajuca mesta:

return `

    <ul class="products">

      ${products.map((product) => ` PRIKAZ POJEDINACNIH PROIZVODA `)

        .join('\n')}

    `;

${product.image}

${product.name}

${product.brand}

$$
{product.price}

+ ${product.raiting} later



6. Build Url Router

1. 	create index.js (src)

First link index.js to index.html as module

<script type="module" src="index.js"></script> u index.html

To znaci da umesto da SAV code pisemo unutar index.html, delove coda mozemo da izdvojimo u zasebne celine kao nezavistane module, odnosno sav code iz app.js nam je dostupan za koriscenje iako je odvojen od index.html

Podeljen code u manje celine je mnogo pregledniji, I lakse se pronalaze I ispravljaju greske..



  2. 	create ProductScreen.js

When we click on product, we will be redirected to new url/adrress width details of that product

  3. 	Import HomeScreen and ProductScreen in index.js (src)



  4. 	create routes obj u index.js (src) pre router() funkcije:

const routes = {

"/": HomeScreen,

"/product/:id": ProductScreen



  5. 	create utils.js (src)   -   export parseRequestURL()

Kako bi znali koja stranica treba da se renderuje I prikaze na ekranu, trenutno unet URL string prvo delimo na komponente..



 export const parseRequestUrl = () => {

  const url = document.location.hash.toLowerCase();

  const request = url.split('/');

  return {

    resource: request[1],		npr ---> /product

    id: request[2],			npr ---> /:id

    verb: request[3],

  };

};



 6. 	u index.js import { parseRequestUrl } from './utils.js'

u index.js import Error404Screen



 	7. 	index.js -->create const router = async () => {

		const request 	   --> parseRequestUrl()

		const parseURL                --> parseUrl

		const screen  	   --> parseUrl === routes/SCREENS

		const main 	 --> screen.render()

}



Vrenosti parsirane URL adrese u cuvamo pod varijablom "request":

const request = parseRequestUrl();

Dobijamo vrednosti:

    resource: request[1],

    id: request[2],

    verb: request[3],



const parseURL =

(request.resource  ?     `  /${request.resource} ` 	: "/")  +

(request.id               ?     " /:id "	 	 : " ")  +

(request.verb          ?     `  /${request.verb} ` 	: " ")



Npr:  resource + id + verb  --->  /product /:id



Na osnovu tih izdvojenih ( resource, id, verb ) komponenti dobijamo parisran URL

( SAMO putanju bez [0] hostName/domena )



const screen = routes[parseUrl]  ?  routes[parseUrl]  :  Error404Screen;



Zatim uporedjujemo ovaj parseURL ---> /product/:id  sa nasim rutama,

"/": HomeScreen,

"/product/:id": ProductScreen



Ako postoji takva routa, renderovace se stranica kojoj pripada



const main = document.getElementById('main-container');

main.innerHTML = await screen.render();



U suprotnom ce se prikazati/renderovati Error404Screen.js, sa error porukom



 8. 	 Na kraju postavljamo posle router():

window.addEventListener(‘load’, router);

Znaci da ce se pri svakom (load) pokretanju i izmeni aplikacije ( index.html ),  izvrsiti router() funkcija iz index.js I renderovace se sadrzaj HomeScreen stranice..



window.addEventListener('hashchange', router);

Znaci da ce se u slucaju promene unete URL adrese (hashchange), izvrsiti router() funkcija iz index.js

I renderovace se onaj sadrzaj  screen.render() koji odgovara toj parseURL putanji..



  9. 	create screens/Error404.js and render error message

const Error404Screen = {

  render: () => {

    return `<div>Page not Found!</div>`;

  },

};

export default Error404Screen;





********************************************************************************

---> Product Screen <---

--> Create Rating Component

	--> fontawesome.css

--> components/Rating.js (src)  +  props

--> HomeScreen + Raiting component

--> STYLE fontawesome icons



--> Product Screen

--> Product Screen UI

--> Product Screen Action



13. Create-Rating-Component

    1. 	fontawesome.css

    2. 	components/Rating.js (src)

    3. 	define Rating object with render() with 2 parametars (value, text)

    4. 	if !props.value return empty div

    5. 	create div.rating  width 5+1 spans

    6. 	Svaki span renderuje/dodaje:

('fa fa-star' ) 	       celu zvezdicu 1

('fa fa-star-half-o' ) 	 pola 0.5		 ILI

( 'fa fa-star-o' ) 	praznu zvezdicu " ".

    7. 	last span for props.text || ‘’

    8. 	Edit HomeScreen

    9. 	Add div.product-rating and use Rating component + IMPORT

${Raiting.render({

value: product.rating,

text: ` ${product.numReviews} reviews `,

})}

    10. 	style .rating{},  .rating span:last-child{}





14. Product-Screen

***

!!!  STEPS:

!!!  index.js - osluskuje promene ‘load’ ili ‘hashchange’ I pokrece parseRequestUrl() I screen.render()

!!!  NPR: productScreen.js  - cuva parseRequestUrl() kao *request* I pokrece metodu getProduct(request.id)

!!!  api.js – izvrsava metodu getProduct( npr: id=3 ) I preko GETa salje URL sa id=3 na server.js

!!!  server.js - osluskuje promene, prima GET zahtev sa URL (id=3), uporedjuje taj id=3 sa bazom podataka I vraca nazad (SEND) *proizvod* koji ima isti id=3

!!!  api.js –getProduct( npr: id=3 ) prima taj “proizvod” u obliku “data”

!!!  productScreen.js  - metoda getProduct( url /:id )  je izvrsena,  const product = data  product.name

!!!  RENDERUJE se *product.name* na stranici /api/product/3

***

    1.	in ProductScreen create  *request = parseRequestUrl() + IMPORT*

    2.	get product id from request: in ProductScreen create  *product = await getProduct(request.id)* + IMPORT

    3.	create  config.js  and make defoult apiUrl = ‘http://localhost:5000’

    4.	create  api.js  file inside “scr”

    5.	in api.js  import AXIOS and apiUrl

    6.	In api.js  create *getProduct = async (id) =>{}*

    7. 	implement /api/product/:id api

    8. 	With AXIOS make

url: `${apiUrl}/api/products/${id}`,   ( http://localhost:5000/api/products/id(value) )

method GET,

header,

    9. 	send Ajax request to product api

          app.get('/api/products/:id', (req, res) => {

 const product = data.products.find((x) => x._id === req.params.id);

 		 if (product) {

 		  	 res.send(product);

  } else {

 	  	 	res.status(404).send({ message: 'Product Not Found!' });

  		}

});



15.  Product-Screen-UI

    1. 	in ProductScreen.js  return  ` `  .content -> back result -> 3colums + .details

    2. 	create *back to result* link button AND create div.details with 3 columns

    3. 	column 1 for product *image*

"${product.image}"

    4. 	column 2 for product *information*  as list:

${product.name}

${Rating.render({ })}  + IMPORT Rating

$${product.price}

${product.description}

    5. 	column 3 for product *action* as list:

$${product.price}

Status: ${ }  *In Stock* OR *Unavailable*

button  *Add to Cart* with #add-button AND . fw primary

    6. 	style .details and all columns

    7. 	create *add to cart* button with add-button id

    8. 	after_render() to add event to the button

    9. 	redirect user to cart/:product_id



16. Product-Screen-Action

    1. 	ProductScreen.js  after_render: ( ) => { } method

  	after_render: () => {

    				const request = parseRequestUrl();

    				document.getElementById('add-button').addEventListener('click', () => {

      					document.location.hash = `/cart/${request.id}`;

    				});

  			},

    2. 	index.js  dodajemo *await screen.after_render();* -> posle screen.render()

    3. 	style change  .success AND .error



********************************************************************************

---> Shopping Cart <---

17. Add To Cart Action

18. Cart Screen UI

19. Update and Delete Cart Items

!!!  Kad se klikne na "Cart" u Hederu, preusmerava se korisnik na /#/cart/

getCartItems() - Prvo ce se preuzeti SVI vec odabrani proizvodi iz localStorage

Zatim ce se renderovati/prikazati CartScreen.js sa svim popdacima tih odabranih proizvodima



!!!  Kad se sa adrese proizvoda /#/product/3 clikne na "add to cart",

Korisnik ce se preusmeriti na /#/cart/3

SetCartItems() - Taj proizvod(3) ce biti prvo dodat u local storage

getCartItems() - Onda ce se preuzeti cela updejtovana lista odabranih proizvoda iz localStorag

Zatim ce se renderovati/prikazati CartScreen.js sa svim podacima tih odabranih proizvoda



UKRATKO:

--> localStorage.js

    SetCartItems()

    getCartItems()

--> index.js ROUTES:

    ‘/cart/:id’: CartScreen,

    ‘/cart’: CartScreen

--> CartScreen.js

    addToCart = (item, forceUpdate = false) => { }*

--> cartItems = [...cartItems, item];

--> setCartItems(cartItems);

--> rerender()

    removeFromCart = (id)

--> .filter() AND rerender()

    render: async ()

--> parseRequestUrl AND getProduct(request.id)

    addToCart({ item }) * QTY *

--> const cartItems = getCartItems();

--> return

    .cart-list

--> cartItems.map((item) =>

`<li> QTY </li>`

    .cart-action

--> Subtotal .reduce()

    after_render()

--> qtySelect.addEventListener('change', (e) =>

    addToCart({ ...item, qty: Number(e.target.value) }, true);

    rerender()

--> deleteButtons

		    removeFromCart(deleteButton.id)

--> checkout-button

    document.location.hash = '/signin'

--> utils.js  - rerender()

--> CSS style





********************************************************************************

---> MongoDB <---

20. Connect-To-MongoDB-and-Create-Admin-User

--> install MongoDB or Atlas

--> npm install mongoose

--> Server.js

IMPORT mongoose

IMPORT config

    	connect to mongodb

config.MONGODB_URL, options + error

--> npm install dotenv  + .env file (root)

	MONGODB_URL=mongodb://localhost/jsamazonadb

--> create config.js  (backend )

import dotenv from 'dotenv';

dotenv.config();

 	MONGODB_URL: process.env.MONGODB_URL,

--> userModel.js

New mongoose.Schema

mongoose.model('User', userSchema)

--> userRouter.js   ( /createadmin )

New User

user.save()

.status(500)  (Server has a problem)

res.send(createdUser)

--> Server.js

	IMPORT userRouter

app.use (‘/api/users’, userRouter);

--> TEST: http://localhost:5000/api/users/createadmin





********************************************************************************

---> User Authentication <---

21. Signin-Screen-UI

--> index.js

‘/signin’: SigninScreen

IMPORT SigninScreen

--> SigninScreen.render()

render email and password fields (form)

Btn submit

New user - RegisterScreen.render()

--> STYLE

22. Signin-Screen-Backend

23. Signin-Screen-Action

24. Progress Indicator

25. Register Screen

26. Profile Screen



Klikom na SUBMIT pokrece se:

API signin(email-input-value, password-input-value) koji preko POSTa, vrednosti iz inputa (data) postavlja u body http requesta I to se salje serveru na ${apiUrl}/api/users/signin

Server UserRouter.post() prima te vrednosti iz bodija (req.body)

I uz pomoc User.findOne() trazi se dal postoji User u MongoDB sa istim e-mailom I passwordom

Ako POSTOJI, poslace se svi podaci tog User-a iz DBa

( + token generisan od podataka signinUser + config.JWT_SECRET ) na /api/users/signin..

API signin  zatim, te podatke USERa + token  dobija I cuva u var DATA u vec parsiranom obliku..

Taj DATA cuvamo u localu preko setUserInfo(data) I korisnik se preusmerava na pocetnu stranicu '/' HomeScreen

Renderuje se HomeScreen.js

Header.render()

- const  { name } = getUserInfo();

- Ako postoje u localu podaci o USER-u prikazi njegovo * ime/name * u hederu

- U suprotnom tj. ako je localStorage prazan, u hederu se prikazuje * signin *

Main 	 --> HomeScreen.render()

Footer --> "All rights reserved @2020"



UKRATKO:

--> SigninScreen.after_render()

'submit' || signin() || setUserInfo(data)  || '/' || showmessage

--> localStorage.js

setUserInfo(data)

getUserInfo(data)

--> api.js

signin( email-value, password-value ) || data || err

***

--> userRouter.js

UserRouter.post() || User.findOne || Req.body || status(401) || token: generateToken(signinUser)

Ako NE postoji user u DB  (401 Unauthorized)

Ako POSOJI user u DB

prikazi sve podatke User-a na /api/users/signin ( + token generisan prema signinUser ) ??

---> utils.js  (backend )

generateToken (signinUser) || jwt.sign ||  config.JWT_SECRET

!!! Token is generated based on information of THIS user (signinUser)



--> * npm install jsonwebtoken *

.env --> JWT_SECRET=somethingsecret (Its master KEY for encripting TOKENS)

config.js (backend) --> JWT_SECRET: process.env. JWT_SECRET

--> * npm install express-async-handler *

stop running our app,  AND it don’t send back correct error message to the user

--> userRouter.js

IMPORT expressAsyncHandler

wrap * userRuter.POST * in expressAsyncHandler( )

wrap * userRuter.GET * in expressAsyncHandler( )



--> Express error middleware (server.js - app.use() )

!!! 400 User entered something wrong

!!! 500 Server has a problem

!!! 401 lacks valid authentication credentials

!!! 404 resource (web page/URL) is unavailable



--> * POSTMAN install ( testing APIs ) *



***

--> HEADER.js component

- Ako postoje u localu podaci o USER-u prikazi njegovo * ime/name * u hederu

- U suprotnom tj. ako je localStorage prazan, u hederu se prikazuje * signin *

name

      ? `<a href="/#/profile">${name}</a>`

      : `<a href="/#/signin">Sign-In</a>`

***

--> Index.js - loading !!!

await Header.render();

await Header.after_render();



--> index.html

<div class="overlay" id="loading-overlay">Loading...</div>

<div class="overlay" id="message-overlay"></div>

CSS style

--> utils.js

showLoading()  -->   .classList.add('active')

hideLoading()   -->    .classList.remove('active')

showMessage(message, callback) - replace "alert" in all screens

.classList.add('active')

.classList.remove('active')

***

--> Register form for new user

API register( name, email, password)

UserRouter() /register

save new User into MongoDB - POST

status(401)  -  'Invalid User Data'



setUserInfo(data) Cuva se new User u localu

redirectUser();

'/shipping'-->getCartItems().length !== 0                        ELSE

/homepage    --> redirect user to the /homepage  and show user-name in the header

***

--> Profile-Screen - On these page/screen User should see:

history of all transactions (all orders),

info about his account with options to update or Logout

--> Render ProfileScreen

	const { name, email } = getUserInfo();

--> Ako *name* ne mostoji u lokaclu, preusmerava se User na glavnu stranicu

--> API

const { _id, token } = getUserInfo();

`${apiUrl}/api/users/${_id}`,

'PUT',

Authorization: `Bearer ${token}`

--> UserRouter() /update

--> update User info in MongoDB - PUT

User.findById(req.params.id);

Update and SAVE:

      user.name = req.body.name || user.name;

      user.email = req.body.email || user.email;

      user.password = req.body.password || user.password;

      const updatedUser = await user.save();

.status(404)

404 resource (web page/URL) is unavailable - User Not Found



--> setUserInfo(data) Cuva se updejtovan User u localu

--> redirectUser();

'/shipping' --> getCartItems().length !== 0                        ELSE

/homepage      -->   redirect user to the /homepage  and show user-name in the header

--> signout btn

clearUser();

localStorage.removeItem('userInfo');

document.location.hash = '/';



--> Use isAuth()

backend/utils.js

Express MIDDLEWERE to prevent Unautorised chages of User Info

https://www.youtube.com/watch?v=mbsmsi7l3r4

( req, res, next )

const bearerToken = req.headers.authorization;

.status(401) - 'Invalid Token'

const token = bearerToken.slice(7, bearerToken.length)

( zadrzi sve od 7 indexa do kraja, tj brise se berier a ostaje samo token)

jwt.verify(token, config.JWT_SECRET, (err, data) => {

      if (err) {

        res.status(401).send({ message: 'Invalid Token' });

      } else {

        req.user = data;

        next();

      }

-	Data = DECODED token (autentication data (user info) we used to generateToken(user))

    {

      _id: user._id,

      name: user.name,

      email: user.email,

      isAdmin: user.isAdmin,

    },



Ako je sve uredu NASTAVI, call next()

prosla je verifikcaija, postavlja se req.user = data

I poziva se NEXT handlerer, kome se salje user = data (ako bude bilo potrebe da se koristi)

Now only owner of account can update/change user info

Odlaskom na `${apiUrl}/api/users/${_id}` server prvo proverava dal mu je poslato u header req.headers.authorization; I ako nije, blokira se pristup tom URL

Ako je poslat, vrsi se verifikacija I server nastavlja dalje obradjuje podatke..





---> Checkout Wizard <---

27.  Checkout-Wizard-Screen

***

!!! 	When user select product and add it to cart, he can * Proceed to Checkout *

!!! 	User will be redirected to * Checkout-Wizard page *, where he first need to register or signIn, and then continue to put info about Shipping and Payment..

!!!	At the end, user will be redirected to  * Place Order * page, to finalize purchase orders..

***



 CheckoutSteps  render  create div elements for step 1 to 4, and add class ‘active’ or ‘empty string’ which depends on * props *

const CheckoutSteps = {

  render: (props) => {

    return `

    <div class="checkout-steps">

      <div class="${props.step1 ? 'active' : ''}">Signin</div>

      <div class="${props.step2 ? 'active' : ''}">Shipping</div>

      <div class="${props.step3 ? 'active' : ''}">Payment</div>

      <div class="${props.step4 ? 'active' : ''}">Place Order</div>

    </div>

    `;

  },

};

export default CheckoutSteps;





28. PlaceOrder-Screen-UI

***

!!! 	When user click “Proceed to Checkout”, he will be redirected directly to /shipping route

!!! 	If User is already registered, shipping form will be automaticly filled, and pressing continue btn user will be redirected to /peyment to choose peyment method (PayPal or Stripe )

!!!	After choosing peyment method, User will be redirected to /placeorder to finalise purchese..

!!!	PlaceOrderScreen UI, should have info about shipping adrress, peyment method, cart items, AND Total price with btn  “Place Order”

***





29. PlaceOrder-Screen-Action

***

!!! 	Clicking on  *Place Order * btn User will be redirected to /order/TOKEN wher he will be abail to finish the purchese

!!!





********************************************************************************

---> Complete Order <---

30. Order-Details-Screen

***

!!! 	apiUrl = 'http://localhost:5000'; ( frontend - config.js )

!!!	MONGODB_URL=mongodb://localhost/jsamazona   ( Root -  .env  )



!!! 	After clicking * Place Order * btn, User will be redirected to * OrderScreen * /order/3h5453hj4567n45n7n7

!!!  	Server osluskuje promenu putanje I poziva

'/order/:id': OrderScreen



!!! 	* OrderScreen * has info about Shipping(delivered?), Payment(peid?), All Cart Items and info about total price with NEW PayPal btn for making final transaction

OrderScreen

Get /id of current order from const request = parseRequestUrl();

Get all info about that order from DB – getOrder(request.id) and with that info fill template

ADD isDelivered and isPaid

NOTE: isPaid and paidAt values we are getting from getOrder()



!!!	Frontend api.js salje zahtev backend router rutama (orderRouter, userRouter)

!!!	Api.js --> gerOrder(id)

Set request to server  (OrderRouter.get)/api/orders/:id,  to GET info from DB about order with that id

 First get User token AND add bearer ${token} for Auth

!!!	Backend --> orderRouter.js

OrderRouter.get

/api/orders/:id,

IsAuth,

order = await Order.findById (req.params.id)

res.send(order);

- order (sav info o porudzbini) salje iz DB nazad u getOrder na frontend, kao response.data

- Zatim OrderScreen iz tog response.data, izvlaci podatke koje lepi u template I prikazuje se stranica Useru..KRAJ



***





31.  PayPal-Payment

***

!!!

Create a PayPal account.

Create a REST API app.

Get your API credentials.

Create sandbox accounts for testing.

!!!







32. Display-Orders-History

***

!!!

!!!

!!!

***

********************************************************************************

---> Admin Products <---

33. Admin-Dashboard-UI

***

!!! 	If user login as Admin, Dashboard link will be in the header..Clicking it, Admin will be redirected to /dashboard screen

!!! 	DashboardScreen has two parts:

Dashboard menu/sidebar on the left AND

info screen on the right

!!!

***



34.  Admin-Products-UI

***

!!! 	Ako je kliknuto u sidebar-u na link 'Products', bice selectovano, I Admin ce biti preusmeren na /#/produclist screen gde ce imati listu I sve info svih trenutnih proizvoda..

!!! 	Admin na toj stranici ima mogucnost da kreira nov proizvod, ili da edituje I brise postojece

!!!	Svaki proizvod ce imati kolone za: ID, NAME, PRICE, CATEGORY, BRAND, ACTION

!!!	Kreiranjem novog proizvoda, dobija se sablon sa popunjenim ovim poljima, koje treba izmeniti

!!!	Cuvamo taj proizvod u DB I dodajemo ga na listu proizvoda

***

IMPORTANT !!!

Change HomeScreen.js --> render

Remove “axios request” , and instead import and USE getProducts we already created

Remove imports we don’t need enymore

Now HomeScreen is empty because we don’t use local data anymore, so we will need to create again all products, send/save them to DB, and receive it back via getProducts() from DB and show on HomeScreen



render: async () => {

    const products = await getProducts();

    if (products.error) {

      return `<div class="error">${products.error}</div>`;

    }





35. Create-Product

***

!!! 	/#/productlist --> “Create Product” btn

- Kreiranjem novog proizvoda, dobija se sablon sa popunjenim ovim poljima, koje treba izmeniti

- Cuvamo taj novi proizvod u DB, I preuzimamo celu updatovanu listu proizvoda sa DB I prikazujemo Adminu

!!!



36. Edit-Product-UI

***

!!! 	Make edit/new product screen  form --> /product/${data.product._id}/edit

!!! 	Form should have: NAME, PRICE, IMAGE, BRAND, COUNTinSTOCK, CATEGORY, DESCRIPTION, + btn Update

Form will be filled width sample info, if we are creating NEW product.. Rewrite all fields and SAVE/Update in DB

Form will be filled width selected product info, when we want to EDIT that product.. Rewrite all fields OR only some and SAVE/Update THAT product in DB

!!!	Than we will be redirected to productList page --> /#/productlist,  and we will get ALL and updated products back from DB

***



37. Product-Update-Backend

***

!!! 	Clicking on Update btn, we are submiting changes we made to that product on DB..

***



38. Upload-Product-Image

***

!!! 	multer npm --->



is a body parsing middleware that handles content type multipart/form-data, which is primarily used for uploading files.

That means it parses the raw http request data which are primarily used for file upload, and makes it more accessible (storing on disk / in memory /...) for further processing.

Without multer, you would have to parse the raw data yourself if you want to access the file.

A multipart request is a REST request containing several packed REST requests inside its entity.



The content type "multipart/form-data" should be used for submitting forms that contain files, non-ASCII data, and binary data.



Multer adds a body object and a file or files object to the request object. The body object contains the values of the text fields of the form, the file or files object contains the files uploaded via the form.



WHY using multer ---> First of all, Express/body-parser does not handle file uploads natively, so that is why you see other libraries being loaded to handle them. They are all going to be loaded as middleware so they can be injected into the request and handle that a file was actually uploaded.



https://levelup.gitconnected.com/playing-with-multer-a8a3378194ed

https://www.youtube.com/watch?v=EVOFt8Its6I



!!! 	OBJASNJENJE:



1. U ROOT putanji, kreiramo novi folder UPLOADS gde ce biti smestene slike koje uploadujemo.. ---> uploads/



2. Prilikom popunjavanja FORME tj, editovanja/kreiranja “product-a”,

preko ( input --> id=”image-file”) bira se image/file (formData)..



3. Zatim API --> uploadProductImage salje taj izabran image/file kao (data: formData) na server uploadRouter.post().. I ocekuje nazad response.data



4. server uploadRouter.post()

pokrece upload.single.(“image”) koji smeasta taj (data) u UPLOADS folder na putanju (upload/imageName.jpg)

Zatim na /api/uploads ---> varaca API-ju tu putanju * upload/imageName.jpg * pod parametrom “image”      ---> .send({ image: `/${req.file.path}` })



5. Kad API dobije nazad response.data, ta vrednost tj, parametar “image” (upload/imageName.jpg) se postavlja kao nova vrednost inputa (input ---> id=”image”)

Prilikom kreiranja/updejtovanja proizvoda u DB taj proizvod ce sadrzati I parametar “image”  sa svojom putanjom odakle ce se preuzeti slika za dati proizvod..

ONDA, prilikom prikazivanja proizvoda na web stranici, podaci o proizvodima ce se preuzeti iz DB..

Slike proizvoda ce biti preuzete sa putanje koja je navedena u parametru “image” --->

* upload/imageName.jpg *

!!!

***



39. Add-Build-Scripts

***

!!! 	Because we were using *build scripts for development* some components (like update/ folder ) which are uploaded directly to the server cant load..

To fix this we need to update server.js, and make *build scripts for prodaction*.. By dooing that everything will be connected as it shoud..



!!! 	WEBPACK  --->  https://www.valentinog.com/blog/webpack/

- We will use “webpack” to manage and MARGE all .js files in ONE single main.js

webpack-dev-server  (automaticly reload our webserver and apply changes)

watch-content-base  (watch/check source folder for eny change)

open  (automaticly open/lunch our webaplication and apply changes)

“webpack-dev-server” automaticly add/create NEW/missing  “main.js”

         and COMBINE all .js files inside ONE main.js



Mode

Webpack has two modes of operations: development and production.

The main difference between them is that production mode automatically applies minification and other optimizations to your JavaScript code.



Entry point

An entry point for webpack is the starting point from which all the dependencies of a frontend project are collected. In practice, it's a simple JavaScript file.

These dependencies form a dependency graph.

The default entry point for webpack (since version 4) is src/index.js, and it's configurable. webpack can have multiple entry points.



Output

The output is where the resulting JavaScript and static files are collected during the build process.

The default output folder for webpack (since version 4) is dist/, configurable as well.

The resulting JavaScript files are part of the so called bundle.



Webpack unify all these different sources and module types in a way that's possible to import everything in your JavaScript code, and finally produce a shippable output.



Loaders

Loaders are third-party extensions that help webpack deal with various file extensions. For example there are loaders for CSS, for images, or for txt files.

The goal of a loader is to transform files (other than JavaScript) in modules. Once the file becomes a module, webpack can use it as a dependency in your project.



Plugins

Plugins are third-party extensions that can alter how webpack works. For example there are plugins for extracting HTML, CSS, or for setting up environment variables.



Code splitting

Code splitting, or lazy loading is an optimization technique for avoiding larger bundles.

With code splitting, developers can decide to load whole blocks of JavaScript only in response to some user interaction, like clicks or route changes (or other conditions).

A piece of code that's splitted becomes a chunk.





Webpack doesn't know on its own how to transform JavaScript code. This task is outsourced to a third-party loader, specifically babel-loader, with babel.

Babel is a JavaScript compiler and "transpiler". Given modern JavaScript syntax as input, babel is able to transform it to compatible code that can run in (almost) any browser.





!!!	.gitignore ---> ADD frontend/main.js



!!! 	express.static

https://findanyanswer.com/what-are-static-files-in-express

https://www.cloudflare.com/learning/cdn/caching-static-and-dynamic-content/



Static content is any content stored in a server that can be delivered to an end user without having to be generated, modified, or processed. The server delivers the same file to each user..

Unlike static content, dynamic content is different for each user, meaning it cannot be served to multiple users and is difficult to cache.

Static files are typically files such as scripts, CSS files, images, etc... that aren't server-generated, but must be sent to the browser when requested. If node.js is your web server, it does not serve any static files by default, you must configure it to serve the static content you want it to serve.

It is used for rendering your static files on the client-side

the idea is that you do not need to generate these files on the fly, as their content does not change.

app.use() acts as a middleware function

__dirname is a current working directory

The difference is that './' and 'process.cwd()' refer to the current dir of the terminal calling the script, whereas the '__dirname' refers to the dir in which the script is stored.

Except when . is used inside require. The path inside require is always relative to the file containing the call to require

Path.join()





!!!	OBJANJENJE coda:

Umesto pojedinacnih src JS fajlova I original backend foldera, prodaction verzija aplikacije ce koristiti DIST folder I main.js fajl.. Server.js mora SVE to da poveze u NOVU celinu..



Pokrecemo *run build* na frontend terminalu

Webpack sve JS fajlove sa fronteda compalira u JEDAN main.js fajl

main.js ce prodaction verzija aplikacije koristiti umesto pojedinacnih fajlova unutar src foldera



Pokrecemo *run build* na ROOT terminalu

Na root, se kreira novi DIST folder kao KOPIJA backend foldera

Backend folder ce sluziti samo za izmene coda, dok ce prodaction verzija aplikacije koristiti novi DIST folder

Svakim pokretanjem *run build* postojeci DIST folder se brise I kreira se novi sa SVIM izmenama koje su se radile u backend folderu..

Babel SAV code pretvara u ES5 verziju kako bi aplikacija bila kompatabilna sa starijim verzijama browsera



Pokrecemo *run serve* na ROOT terminalu

In the BACKEND folder (not DIST) we are making changes, and by running *run BUILD* all changes will be pressent in newly created DIST folder..

That way Prodaction version of app can use updated DIST fajls (server.js) connected width frontend and upload folder

DAKLE server.js povezuje DIST root folder sa /../frontend I /../upload folderom..

index.html postvaljamo da je uvek dostupan prilikom unosa bilo koje url adrese.. '/../frontend/index.html'



***





OBJASNJENJE:

Povezujemo DIST root folder sa /../frontend I /../upload folderom..

index.html postvaljamo da je uvek dostupan prilikom unosa bilo koje url adrese.. '/../frontend/index.html'



app.use() acts as a middleware function



path is module with methods that help you deal with file and directory path names on the machine’s filesystem.

path.join. The join method takes two or more parts of a file path and joins them into one string that can be used anywhere that requires a file path.

Example: Connecting -->

(__dirname) our ROOT directory DIST       +

/../uploads (directory outside ROOT-a )

/../ ---> lokacija *uploads foldera* u odnosu na ROOT odakle se isti zahteva.. U ovom slucaju trazeni folder je jedan folder pre root DIST foldera (moze biti bilo gde na kompjuteru, I tad postavljamo direktnu putanju)



__dirname se odnosi na DIST folder tj, ROOT directory sa kog se pokrece server.js, prodaction verzija naseg sajta..

Pokretanjem npm build, kreira se DIST folder(kopija backend foldera), kao ROOT directory naseg sajta odakle se pokrece server.js

Pokretanjem npm serve, pokrece se server.js iz DISTa, I uspostavlja konekciju ( serve at ) na http://localhost:5000

Kasnije ce to biti prava adresa naseg sajta..

Na adressi http://localhost:5000/uploads, server dobija pristup SVIM folderima I fajlovima (CSS, Images, Files..) koji se nalaze unutar /uploads foldera negde na kompu/serveru

NPR: ako nam treba neka slika iz uploads foldera, dobicemo je preko url adrese http://localhost:5000/uploads/234387894568712.jpg

NPR2: ako web stranica zahteva nesto iz main.js iz frontend foldera '/../frontend', server tacno zna gde tome da pristupi I upotrebi --> http://localhost:5000/main.js

To su uglavnom podaci koji se verovatno nikad ne menjaju, staticni su..



'*' + res.sendFile ---> For ALL/any url that is entered, server should have access to, for example '/../frontend/index.html'  and return/serve/use that SPECIFIC file index.html all the time..



40.  Delete-Product

***

!!! 	When we as Admin go to dashboard, in the *product list*, we have option delete..

!!! 	If we click delete btn, CONFIRM massage should popup..

!!!	If we confirm it, product with the same ID as btn.id will be:

deleted from DB,

removed from product list,

Removed from homePage /#/

!!! 	Then, *product list* page will refresh, and from updated DB will get again all products..



!!! 	ISTRAZI:

https://stackoverflow.com/questions/14377590/queryselector-and-queryselectorall-vs-getelementsbyclassname-and-getelementbyid

getElementsByClassName() vs querySelectorAll()

querySelectorAll() retrieves a list of elements from the document based on your given selector, and returns a static NodeList object.

getElementsByClassName() retrieves a list of elements from the document based on an element's class name, and returns a live HTML collection of elements.



NodeList object vs HTML collection

Both interfaces are collections of DOM nodes. Both are ARRAY-LIKE OBJECTS, not array lists..

They differ in the methods they provide and in the type of nodes they can contain.

While a NodeList can contain any node type, an HTMLCollection is supposed to only contain Element nodes.
An HTMLCollection provides the same methods as a NodeList and additionally a method called namedItem.

Collections are always used when access has to be provided to multiple nodes, e.g. most selector methods (such as getElementsByTagName) return multiple nodes or getting a reference to all children (element.childNodes).

The biggest differences between standard DOM collections and jQuery selections is that:

DOM collections are typically live (not all methods return a live collection though), i.e. any changes to the DOM are reflected in the collections if they are affected. They are like a view on the DOM tree,

whereas jQuery selections are snapshots of the DOM tree in the moment the function was called.

The NodeList returned by querySelectorAll() is not live, which means that changes in the DOM are not reflected in the collection.



array-like objects vs arrey list

https://daily.dev/blog/why-do-you-need-to-know-about-array-like-objects

https://dev.to/capscode/what-is-array-like-object-in-javascript-3f5m

Javascript arrays are a type of object used for storing multiple values in a single variable. Each value gets numeric index and may be any data type.

Arrays have a length property that tells how many items are in the array and is automatically updated when you add or remove items to the array.

Array-like objects look like arrays. They have various numbered elements and a length property. But that’s where the similarity stops. Array-like objects do not have any of Array’s functions, and for-in loops don’t even work!

A common one is the arguments variable that is present inside of every js function.

In Array like object we cannot access properties like we used to do in object.

( nemaju properije, vec umesto propertija dobijaju indexne brojeve 0: 1: 2: itd, preko kojih moze da se pristupa vrednsotima)

// simple array

const arr = ['a', 'b', 'c'];

console.log(Object.keys(arr)); // ['0', '1', '2']

// array-like object

const obj = { 0: 'a', 1: 'b', 2: 'c' };		          	console.log(Object.keys(obj)); // ['0', '1', '2']



***

OBJASNJENJE CODA:

Get all btn with class name “delete-buttons"

Converte this NodeList object to ARRAY so we can use .forEach()

Listen every btn and on click, *confirm message* should popup

If confirmed, run Api --> deleteProduct(deleteButton.id)

It will send DELETE request and ID to ${apiUrl}/api/products/${productId}

THEN productRouter.delete() will first:

Receve that ID productId

check isAuth, isAdmin

run expressAsyncHendler() wich will

Find product in DB with receved ID (req.params.id)

Remove that product in DB

Send back to API

 message: 'Product Deleted', product: deletedProduct

OR error 404 --> message: 'Product not Found

At the end Api deleteProduct() will:

rerender(ProductListScreen) width updated products from DB..

Show ERROR 404 --> message: 'Product not Found





********************************************************************************

---> Admin Orders <---

41. Admin-Order / List-Orders / Delete-Orders /

***

!!! 	We are creating orderListScreen, which will have list of all orders

!!! 	For each order we will get all needed info ..

ID, DATE, TOTAL, USER, PAID AT, DELIVERED AT, ACTIONS(edit/delite)



!!! 	When we as Admin go to dashboard, in the *orders list*, we will have also 2 options edit and delete..

!!! 	If we click delete btn, CONFIRM massage should popup..

!!!	If we confirm it, order with the same ID as btn.id will be:

deleted from DB,

Removed from /api/orders/${orderId}

removed from ADMIN order list,

!!! 	Then, Admin *order list* page will refresh, and from updated DB will get again all orders..



!!!  	FIX typo for: expressAsyncHandler in orderRouter.js and productRouter.js

Select it and press fn(function) + f2 and rename it to correct one in all instances at ONCE

***



42. Edit/Deliver-Order

***

!!! 	Edit orderListScreen...

!!! 	For each order we will get all needed info ..

ID, DATE, TOTAL, USER, PAID AT, DELIVERED AT, ACTIONS(edit/delite)

!!! 	When we as Admin go to dashboard, in the *orders list*, we will have also 2 options edit and delete..



!!! 	If order is payed  and delivered, we can update its status by clicking EDIT btn..

!!! 	We will be redirected to /#/order/orderID  screen.. and if

order is payed BUT status is “not delivered”,

deliver button will be shown for admin

When we click deliver button, order info in shipping part will be changed/updated from NOT DELIVERED to DELIVERED and popup message will inform as about change

That order will be updated in DB, and when we again open *order List* screen, all orders will be loaded from DB and shown to us with updated info..

!!!

***



********************************************************************************

---> Dashboard Chart <---

43. Dashboard-Summary

***

!!! 	Dashboard screen /#/dashboard, will show us some statistic info about

Users box(how many),

Orders box (how many),

Sales box(how much we earned),

Sales - linear chart(visual presentation),

Categories - pie chart(types of product that we sold in numbers)

!!!	Only Admin can go to dashboard/Orders/Products screen

OBJASNJENJE:

Look for ALL orders in DB and give back a unique group width:

numOrders ---> total number of ORDERS

$sum: 1

---> every order will be calc as +1

totalSales ---> Total price of all orders combined

$sum: '$totalPrice'

--> ADD totalPrice of EVERY order to ONE TOTAL price

Look for ALL users in DB and give back a unique group width:

NumUsers ---> total number of USERS



.aggregate

https://www.youtube.com/watch?v=Kk6Er0c7srU

Meaning

a whole formed or calculated by combining several separate elements into a single group or total.

The aggregate functions are count, sum, average, min, max, etc.



NOTE:

_id: $users

It will show combined data of every unique user from DB collection..They will be present to us width ONE common ID --->

* _id: name of specific user *

NPR: {“id”: “jovan”, “total” : 13 eur }

{“id”: “marko”, “total” : 228 eur }

_id: null

ALL users from DB collection will be grouped and their combined data will be show to us..

NumUsers - how many of them

TotalSum – how much they spend together on my website





44. Dashboard-Chart

***

!!! 	Dashboard screen /#/dashboard, will show us some statistic info about

Users box(how many),

Orders box (how many),

Sales box(how much we earned),

Sales - linear chart(visual presentation),

Categories - pie chart(types of product that we sold in numbers)

!!!	Only Admin can go to dashboard/Orders/Products screen


$$
