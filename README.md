# Javascript--Rocket-Launch
Rocket Launch Project for Javascript

GitHub Repository:
https://github.com/jocksr/Javascript--Rocket-Launch/

The callback passedthe populateDropdown function into getUpcomingLaunches without calling it right away. Once the XMLHttpRequest finished (successfully) and hte launch data was ready, getUpcomingLaunches called that callback and passes it to the results array.

In the Axios version, the callback parameters were removed because Axios returns a promise. The .then block handles a successful response and passes the returned data to populateDropdown or displayLaunchInfo, while .catch handles request errors and displays an error message.