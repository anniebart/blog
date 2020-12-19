---
title: Speculative Authentication
date: 2020-12-19 10:00:30
draft: false
---

(or how to make pixel art your password)


Speculative Authentication is essentially reimagining the way we authenticate users. Instead of just creating things, to create ideas, about what could be, imagining possible futures. Rather than authenticating through a traditional password, a string of characters the user inputs, what if the authentication method looked like something else? But what?


### How I became interested
A few weeks ago, I came across a [website](https://passwords.ai/) that documented a three-day meeting of a group of artists, designers and technologists. The purpose of this meeting was to reimagine how machine learning might be able to be used in authentication- but not using traditional methods like biometric data. 

<img src="https://passwords.ai/img/united.jpg" height="300px">

What they came up with was a bunch of quirky methods, one using collaboration as the key to unlock a message, while others used body movements and images to implement their own authentications. 

<img src="https://passwords.ai/img/uniuni.gif" height="300px">
<br> <br>
As a somewhat newer programmer, I was hesistant to delve into machine learning yet, but I was curious about how I might go about implementing my own alternative method for authentication. What would that look like? How could I avoid using machine learning in doing so? What would the user inputs be? How could that be secured? <br> <br>


<img src="https://camo.githubusercontent.com/46537f33c0c5db8403aa04545249a218cb908c6a106070b63ca6cdef6a10c5b1/68747470733a2f2f7777772e616e6e696562617274686f6c6f6d65772e636f6d2f73637265656e2d73686f742d323032302d31322d31312d61742d312e34322e31302d706d2e706e67" height="300px">

### Enter Pixel Art
The first question I had after I decided to use pixel art as my method, is how can you translate the location of a pixel, it’s color, to something that can be saved, verified, and used to authenticate. 

Well, convert it to a string of course. 

<img src="https://www.anniebartholomew.com/screen-shot-2020-12-17-at-12.46.05-pm.png" height ="300px">

Each pixel is an input that has a corresponding value. The value of the input is added onto an array that store the order of the input sequence and once the user is ready to sign up, the array is concatenated to create the password string. 

### And then some security things

The string is then hashed and salted using [Bcrypt](https://www.npmjs.com/package/bcrypt) before being store in the database alongside the username. 

As of now, the username is just a string of characters - still playing with other ideas for creating an alternative user indentifier - perhaps another input of pixel art?

When the user login, a similar process ensues. The user inputs their sequence of pixels and bcrypt does its magic to determine whether the that matches up with the stored (hashed + salted) password. 

I'm not claiming this authentication method is the most airtight, secure thing ever to hit the tech world. But it has been an interesting way to examine whether we can approach authentication a little differently. After all, CAPTCHA, face recognition + two-factor were new once too!

## Now what?
That's a good question. I'm hoping to use the pixel art authentication method on some smaller projects in the future. Perhaps do a little more work on the security side. 

I'm also curious to experiment with further alternatives to authentication - what other methods can I try? How else can we reimagine what a password is?

And what other things can we reimagine?






