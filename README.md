# Cookies-Sessions
Passport.js
Adding Cookies and Session by requiring passport, passport-local, passport-local-mongoose, express-session
const session = require("express-session");
const passport = require("passport");
const passportLocalMongoose = require("passport-local-mongoose"); 
// We don't need to require 'passport-local'
 
 // Using session, passport
app.use(session({
   secret: "Suar always kept his secret",
   resave: false,
   saveUninitialized: false
}));

app.use(passport.initialize());
app.use(passport.session());

