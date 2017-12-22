---?image=https://www.dotjs.io/static/images/background-header-home-dotcss-2017.jpg

@title[init1]

## DotJS
### The largest JavaScript conference in Europe


---

@title[wesbos]

## Wes Bos

![GitHub Logo](https://s3-eu-central-1.amazonaws.com/static-dotconferences-com/speakers_images/wes-bos.png)

JS Guru: Async/await patterns.

---
@title[wesbos_2]

Synchronous looking code, without that wait!

```
const makeRequest = () => {
  return callAPromise()
    .then(() => callAPromise())
    .then(() => callAPromise())
    .then(() => callAPromise())
    .then(() => callAPromise())
    .then(() => {
      throw new Error("oops");
    })
}
```

---
@title[wesbos_3]

Synchronous looking code, without that wait!

```
const makeRequest = async () => {
  await callAPromise()
  await callAPromise()
  await callAPromise()
  await callAPromise()
  await callAPromise()
  throw new Error("oops");
}
```

---
@title[wesbos_4]

Higher order function to catch errors!

```
const getOrders = async (req, res, next) {
 const Orders.find({...});
 
 if(!orders.length) throw Error('NotOrderFound');
 // ...
}

const displayErrors = async (error, req, res, next) {
  res.status(err.status || 500);
  res.json(err).end();
} 

app.use(displayErrors);

const catchErrors = (fn) => (req, res, next) => fn(req, res, next).catch(next);

router.get('/orders', catchError(getOrders));
```

---

@title[brendon]

## Brendan Eich

![GitHub Logo](https://s3-eu-central-1.amazonaws.com/static-dotconferences-com/speakers_images/brendan-eich.png)

Javascript inventor.

---

@title[lankin]

## Sean Larkin

![GitHub Logo](https://s3-eu-central-1.amazonaws.com/static-dotconferences-com/speakers_images/sean-larkin.png)

Webpack core team. Webpack Architecture.

---

@title[sutton]

## Marcy Sutton

![GitHub Logo](https://s3-eu-central-1.amazonaws.com/static-dotconferences-com/speakers_images/marcy-sutton.png)

Accessibility advocate. [Talk](https://www.dotconferences.com/2017/12/marcy-sutton-enabling-users-in-client-rendered-applications) 


---

@title[holovaty]

## Adrian Holovaty
### A framework author's case against frameworks.

![GitHub Logo](https://s3-eu-central-1.amazonaws.com/static-dotconferences-com/speakers_images/adrian-holovaty.png)

Co-creator of Django.

[Talk](https://www.dotconferences.com/2017/12/adrian-holovaty-a-framework-author-case-against-frameworks)

---

@title[dale]

## Tom Dale

![GitHub Logo](https://s3-eu-central-1.amazonaws.com/static-dotconferences-com/speakers_images/tom-dale.png)

Software Engineer at LinkedIn.

---

@title[willis]

## Trent Willis

![GitHub Logo](https://s3-eu-central-1.amazonaws.com/static-dotconferences-com/speakers_images/trent-willis.png)

Software Senior QA Engineer at Netflix.

---

@title[watson]

## Thomas Watson
### Getting Data From The Sky.

![GitHub Logo](https://s3-eu-central-1.amazonaws.com/static-dotconferences-com/speakers_images/thomas-watson.png)

Node.js developer at Elastic. Fun with Aircrafts

[Talk](https://www.dotconferences.com/2017/12/feross-aboukhadijeh-the-most-annoying-website) 
---

@title[aboukhadijeh]

## Feross Aboukhadijeh
### The Most Annoying Website

![GitHub Logo](https://s3-eu-central-1.amazonaws.com/static-dotconferences-com/speakers_images/feross-aboukhadijeh.png)

Founder of WebTorrent, Standard JS & NodeFoo.

[Talk](https://www.dotconferences.com/2017/12/feross-aboukhadijeh-the-most-annoying-website) 

---

