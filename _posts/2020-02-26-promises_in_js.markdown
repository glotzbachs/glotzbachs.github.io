---
layout: post
title:      "Promises in JS"
date:       2020-02-26 23:20:53 -0500
permalink:  promises_in_js
---

Promises were added into the functionality of JavaScript in ES6. One of the most helpful parts of promises is that they are asynchronous. This means while we wait for the promise to be resolved or rejected, other code will be able to run. We are also given two options with a promise: .then and .catch. .then allows for a resolved promise to be handled. .catch allows for a rejected promise to be handled. Before promises, extra code was needed in previous versions of JS to handle any errors, and that generally made code take a long time to load. 

Getting data is something that can take a lot of time, especially since we could be waiting for a lot of data to be retrieved. In ES6 we have been given fetch. Fetch automatically comes with promise attached. Since the promise given by fetch allows for asynchrony, we do not have to wait until the end of the fetch for the rest of our code to run. This helps to make websites run more efficiently and without lags. Once the promise has been resolved, the fetch will give us the data from the api. From the fetch, either we will get an error, or a response. 

If there are no errors, we are given a response through the fetch. This can be handled with .then which will accept the response. This response will be passed into another function that turns it into usable JSON. We do this we .json() which also has a promise attached to it which means while the unusable data is being converted, other code will still run. Once that promise has been resolved, we are given JSON that can be used in the rest of our code.

Another great part about promises is that they can be linked. So for all of the promises involved in a fetch request, from the initial fetch until we can use the data we receive, any errors can be handled in one .catch. This will take any errors and handle it in whatever way specified in the .catch. This can be especially helpful if you have a fetch within a fetch. Less code, especially repetitive code, is the goal of any good coder, and promises make that much easier. 

