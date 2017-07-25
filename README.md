WebSockets 101
Building Our First Two Way App

Twitter: @dmikeyanderson

## Ex 1

* Introduce web sockets
* websocket.org/echo.html


## Ex 2

Getting Started

* Getting our project Set Up
* Package.JSON 
* http://bit.ly/2uiuUbQ



## Ex 3

Introduction to SocketIO


Client

const socket = require('socket.io-client')('http://localhost:3000');
socket.on('connect', function(){});
socket.on('foo', function(data){
   console.log(data);
});
socket.on('disconnect', function(){});


Server

const io = require('socket.io')(http);
io.on('connection', function(socket){
  console.log('connected!');
  socket.emit('foo', {foo:'bar'});
});


## Ex 4

Have the Client Send Back to the Server

## Ex 5

## Ex 6

## Ex 7

## Ex 8

## Ex 9

Webpack Webworkers the BEST WAY to WebWork!

Look HOW awesome this is!

// main.js
var MyWorker = require("worker-loader!./file.js");

var worker = new MyWorker();
worker.postMessage({a: 1});
worker.onmessage = function(event) {...};
worker.addEventListener("message", function(event) {...});

Let’s Implement!

npm install work-loader



[code together]

## Ex 10

Let’s Move Everything to a WebWorker!

[move chat code to web worker]
