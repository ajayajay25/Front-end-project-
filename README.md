Go

Run

←→

Qmoney

X

> import React, [useEffect, useState) fr Untitled-94.

() Untitled-10

() Untitled-11

() Untitled-12

EXPLORER

MONEY

Q

> build

2

> contracts

> migrations

6

> money

7

> node modules

.gitignore

11

},

LICENSE

12

JS naan muthalvan... U

13

11 package-lock.json M

14

() package.json M

README.md

Js truffle-config.js

le in repo wi Untitled-7

Untitled-8

"name": "contact.forex-demo",

3

"version": "1.0.0",

"main": "server.js",

> lib

5

"scripts": [ "start": "node server.js", "dev": "nodemon server.js"),

"dependencies": {

"cors": "2.8.5",

"express": "4.18.2",

> test

9

"Joi": "17.9.2",

18

"dotenv": "16.0.0"

"devDependencies": { "nodemon": "^2.0.22" }

PROBLEMS

OUTPUT

DEBUG CONSOLE

TERMINAL

PORTS

powershell+日×

PS E:\matt blockchain project\money laundering\blockchain_bitcoin\money>

> OUTLINE

> TIMELINE

money develop 01 1141
←→

money

() Untitled-11

() Untitled-10

() Untitled-12.

JS // server.js (file-based demo) Untitled-13

EXPLORER

<> import React, (useEffect, useState) fr Untitled-94

Q

MONEY

36 app.post('/api/contact', async (req, res) => {

> build

37 try {

> contracts

38 const { error, value} contactSchema.validate(req.body);

39

> lib

48

if (error) return res.status(400).json({ success: false, error: error.details[0].message));

> migrations

41 const contacts await readContacts();

> money

42

const newContact = { id: contacts.length + 1, ...value, createdAt: new Date().toISOString()};

> node modules

43 contacts.push(newContact);

> test

44 await writeContacts (contacts);

.gitignore

45 // optionally: enqueue email send here

LICENSE

47 catch (err) (

46 res.status(201).json((success: true, data: newContact));

JS naan muthalvan... U

48 console.error(err);

11 package-lock.json M

49 res.status(500).json({ success: false, error: 'Server error' });

() package.json M

58 }

README.md

51 });

Js truffle-config.js

52

53 // List contacts

54 app.get('/api/contact, async (req, res) -> (

55 const contacts await readContacts();

56 res.json(contacts);

57 });

58

59 const PORT process.env. PORT || 5000;

60 app.listen(PORT, ()-> console.log('ContactFormX deso running on $(PORT)"));

61

PROBLEMS

OUTPUT

DEBUG CONSOLE

TERMINAL

PORTS

powershell+日×

PS E:\matt blockchain project\money laundering\blockchain_bitcoin\money>

> OUTLINE

> TIMELINE

money develop 01 11

4A1J

Fetching data for better TypeScript IntelliSense

Ln
←→

money

X

EXPLORER

Untitled-10.

15 // server.js (file-based demo) Untitled-13

> <!doctype html> Untitled-14

() Untitled-15

Q

MONEY

> build

2

> contracts

> lib

5

> migrations

6

> money

7

> node modules

> test

9

.gitignore

11

LICENSE

12

JS naan muthalvan... U

13

11 package-lock.json M

14

() package.json M

15

}

README.md

16

JS truffle-config.js

() Untitled-11

() Untitled-12.

"name":"contactformx",

3

"version":"1.0.0",

"main": "server.js",

"scripts":{"start": "node server.js", "dev": "nodemon server.js"),

"dependencies": {

"cors":"#2.8.5",

"dotenv":"16.0.0",

"express": "^4.18.2",

18

"Joi":"17.9.2",

"mongoose":"^7.0.0",

"nodemailer":"^6.9.3"

"devDependencies": ("nodemon": "^2.0.22")

PROBLEMS

OUTPUT

DEBUG CONSOLE

TERMINAL

PORTS

powershell+日×

PS E:\matt blockchain project\money laundering\blockchain_bitcoin\money>

> OUTLINE
Run

←→

money

X

<> <!doctype html> Untitled-14

() Untitled-15

PORT=5000 Untitled-16

PORT 5000 Untitled-17

EXPLORER

//server.js (file-based demo) Untitled-13

MONEY

PORT-5000

Q

> build

2 MONGO URI-mongodb+srv://<user>:<pass>@clustere.mongodb.net/contactformx?retryWrites-true&w-majority

> contracts

3 ADMIN EMAIL admin@example.com

SMTP HOST-smtp.example.com

> lib

> migrations

5 SMTP PORT-587

> money

6 SMTP USER-username

7 SMTP PASS-password

> node modules

8

> test

.gitignore

LICENSE

JS naan muthalvan... U

11 package-lock.json M

() package.json

README.md

Js truffle-config.js

M

PROBLEMS

OUTPUT

DEBUG CONSOLE

TERMINAL

PORTS

powershell+日×

PS E:\matt blockchain project\money laundering\blockchain_bitcoin\money>

> OUTLINE

> TIMELINE
Go Run

←→

money

EXPLORER

() Untitled-15

PORT 5000 Untitled-16

PORT 5000 Untitled-17

15//models/contact.js Untitled-18.

JS //routes/contact.js Untitled-19

Q

MONEY

14 router.post('/', async (req, res) -> {

> build

24 } catch (err) {

> contracts

27 }

> lib

29

28 });

> migrations

30 router.get('/', async (req, res) => {

> money

31 try

> node modules

32 const items await Contact.find().sort([createdat: -1).limit(100);

> test

33 res.json(items);

.gitignore

34 } catch(err) (

LICENSE

35 res.status(500).json((error: 'Server error' });

36

JS naan muthalvan... U

37 });

11 package-lock.json M

38

() package.json M

39 router.get("/:id', async (req, res) => {

README.md

48 try {

Js truffle-config.js

41 const item await Contact.findById(req.params.id);

42

if (litem) return res.status(404).json((error: "Not found" });

46

43 res.json(item);

44 catch(err) {

45 res.status(500).json({ error: 'Server error' });

47 });

48

49 module.exports router;

58

PROBLEMS

OUTPUT

DEBUG CONSOLE

TERMINAL

PORTS

powershell+日×

PS E:\matt blockchain project\money laundering\blockchain_bitcoin\money>

> OUTLINE

> TIMELINE

money develop 01 1141
Go Run

←→

money

EXPLORER

<> <idoctype html> Untitled-14 () Untitled-15. PORT=5000 Untitled-16

PORT 5000 Untitled-17

JS //models/contact.js Untitled-18

Q

MONEY

//models/contact.js

> build

2 const mongoose require('mongoose');

3

> contracts

const ContactSchema new mongoose.Schema({

> lib

> migrations

5 name: type: String, required: true, trim: true),

> money

6 email: [type: String, required: true, trim: true).

7 message: type: String, required: true),

> node modules

), (timestamps: true));

21

> test

9

18 module.exports = mongoose.model('Contact', ContactSchema);

.gitignore

LICENSE

JS naan muthalvan... U

11 package-lock.json M

() package.json

README.md

Js truffle-config.js

M

PROBLEMS

OUTPUT

DEBUG CONSOLE

TERMINAL

PORTS

powershell+日×

PS E:\matt blockchain project\money laundering\blockchain_bitcoin\money>

> OUTLINE

> TIMELINE

money develop 01 1141

X

Ln
Go

Run

←→

money

0

X

EXPLORER

fr Untitled-9 4

() Untitled-10

() Untitled-11

() Untitled-12

15 // server.js (file-based demo) Untitled-13

<!doctype html> Untitled-14

Q

> build

6

MONEY

4

<body>

<form id="contactForm">

> contracts

10

<button>Send</button>

> lib

12

</form>

> migrations

13

<pre id-"result"></pre>

> money

14

<script>

const form = document.getElementById('contactForm');

> node modules

15

form.addEventListener('submit', async (e) {

> test

16

17 м

e.preventDefault();

const data

.gitignore

18

name: form.name.value,

LICENSE

19

email: form.email.value,

JS naan muthalvan... U

20

message: form.message.value

11 package-lock.json M

21

22

const res await fetch('/api/contact', {

() package.json M

method: 'POST',

README.md

23

headers: ('Content-Type: application/json'),

Js truffle-config.js

24

25

26

});

27

body: JSON.stringify(data)

const json await res.json();

28

document.getElementById('result').textContent JSON.stringify(json, null, 2);

29

});

30

</script>

31 </body>

32

</html>

33

PROBLEMS

OUTPUT

DEBUG CONSOLE

TERMINAL

PORTS

powershell+日×

PS E:\matt blockchain project\money laundering\blockchain_bitcoin\money>

> OUTLINE

> TIMELINE
Edit

Selection

View

Go

Run

←→

money

X

EXPLORER

ude a env.example file in repo wi Untitled-7

Untitled-8

import React, (useEffect, useState) fr Untitled-94

() Untitled-10

() Untitled-11

Q

MONEY

> build

2

"success": true,

> contracts

3 "message": "Contact form submitted successfully"

D

> lib

> migrations

> money

> node modules

> test

.gitignore

LICENSE

JS naan muthalvan... U

11 package-lock.json M

() package.json

README.md

Js truffle-config.js

M

PROBLEMS

OUTPUT

DEBUG CONSOLE

TERMINAL

PORTS

powershell+日×

PS E:\matt blockchain project\money laundering\blockchain_bitcoin\money>

> OUTLINE

> TIMELINE
