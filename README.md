# Convision
Augmented reality based Android application to convert currencies real-time on camera.

[![demo](Convision Logo.png)](https://www.youtube.com/watch?v=vMdTO_IW4fY)

## Inspiration
Inspired by a recent struggle of how one of our team members who just flew over from Indonesia for this hackathon has to adapt to the Canadian currency, we decided that real-time conversion would benefit millions of tourists worldwide. This paves the way for us to bridge a gap between modern technologies and increasingly prevalent problems.

## What it does
Convision uses Optical Character Recognition (OCR) which is modified to recognize and isolate prices in prints such as but not limited to menus, receipts and bills. These currencies can then be converted into any corresponding currency using Xe.com’s API and displayed in place of the detected values.

## How we built it
We used Android Studio to construct the app. Our OCR is set up using Google Vision's open-source packages along with our own modifications to optimize the OCR. In order to obtain real-time currency rates, we called Xe.com’s API and parsed JSON objects to obtain values for calculations.

## Challenges we ran into
Issues with Xe.com HTTP Requests from Android Studio. We requested help and guidance from mentors and Xe.com employees to solve the problem. After a few hours of their kind assistance to debug the API calls, we found that there might be a compatibility issue between the API and Android Studio. We resorted to getting the required conversion rates by calling the API in a Python text editor and moving the data over to our Android application.
Unresponsive Android Studio client and inconsistent configurations on each member’s laptop, rendering some of our laptops to be a pain to work with and even obsolete.
Accomplishments that we're proud of
Despite all the pitfalls, we managed to complete and integrate some of the most important parts:

Menu screen that includes a dropdown menu for currency conversion selection.
Flash and auto focus for a more user-friendly application.
Camera screen which automatically recognizes prices and passes them into our converter.
Displays corresponding conversions in real-time in place of the detected prices.
What we learned
In terms of technology, we learned about mobile development, augmented reality, REST API integration and more. We are very grateful for the opportunity to work as a team, with our mentors and meet many bright minds at Hack the North.

## What's next for Convision
Our main approach as described under challenges we ran into was to make an API call on every selection of parameters. This is decent for a start but it would not be ideal if it were to be used by millions of users daily considering the volume of API calls that would involve. Therefore, we could potentially link API requests to a database and have it update only when changes are made to currency exchange values.
User interfaces can always be improved to make our product more seamless and consequently, attract a higher number of active users.
