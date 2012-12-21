# 3G Slick JS ![3G SlickJS](http://s3.amazonaws.com/mynodebucket/assets/images/slicklogo.png)

Slick 3G Network Videos for mobile devices with super slow internet.

## Description

Manage HTML5 Video quality fed across a variety of devices. A few lines of JavaScript efficiently solves the problem of video interuption often experienced while trying watch an overly robust video feed via 3G Cellular Data Network. You know what I mean. It chokes up and this utility performs the heimlic. 

## Demo

[Check out the demo](http://video.kickr.io) and disable wifi on your mobile device.

## Dependencies

[jQuery](http://ajax.googleapis.com/ajax/libs/jquery/1.8.3/jquery.min.js) is a dependency the way things are written in the repo js file, but you don't need to use jQuery if you prefer that slight performance advantage of element selection and attribute manipulation in regular JavaScript by itself.

## Requirements & Related Prerequisite Discussion

Use [Handbrake](http://handbrake.fr/downloads.php).

Use the mobile device console to understand whether your program functions as you intend. I imagine adobe has something. Also I would assume phone gap has some type of console, though I have not yet checked the docs. I use the iOS Simulator App outputing console messages in Safari. The only drawbacks are that I have to install Xcode and I'm reading console messages in something other than Chrome which is unatural to me. Safari console is a little out of control and I can't figure out how to stop the thing from running its performance checks during the simulator refreshes for the life of me. For more on that subject consult the horse's mouth over here: [Apple Dev Docs, Debugging Web Content on iOS](http://goo.gl/8A7BN)

## Usage

[Review the code and comments](http://github.com/bcardan/3gslick.js/blob/master/3gslick.js)


If this utility doesn't suit your needs check out all the [cool components](https://github.com/component/component/wiki/Components#wiki-media).

### Roadmap: Stop checking mobile devices with the assumption they don't use wifi. Instead check for the network type associated with the request in order to respond precisely to the user's internet connection speed and browsing experience or whatever, rather than a blind device check. 

http://stackoverflow.com/questions/8598065/how-do-you-detect-3g-vs-wifi-connection-on-mobile-safari

With polite aknowledgement and respect for the gentleman's response to inquiry above on StackOverflow, I doubt his answer. There's gotta be a way to do it... Node or an npm package might help figure it out on the server side. But before going there I'm sure this is available upon TCP handshake. The Network Access layer controls the communication between the hardware in the network..  That's pretty deep stuff and I want to avoid getting phone gap involved to simply check for a 3G network if possible. That's what they call a long run for a short slide. Forgive my ramblings if stumble across this repo and happen to know or think of something please submit a pull request or issue. Would be greatly appreciated. The community should be able to accomplish this with a little front-end JavaScript. Why not? 

I image if this is not possible the ECMAScript committee needs to be notified and made aware of the issue. I hope they haven't deemed the issue outside their scope. As I understand the Network Layer and JavaScript Interpreter are in the same proximity to one another in the browser. 

Also I haven't found a single helpful thing here: http://www.ecma-international.org/ecma-262/5.1/#sec-4.3.6

btw, firefox is apparently killing it with the ECMAScript 6 coverage: http://kangax.github.com/es5-compat-table/es6/