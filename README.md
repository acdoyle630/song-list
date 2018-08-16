# Song-List
### To Run
* clone repository
* `npm install` on client and server
* from server `nodemon index.js`
* from client `npm start`
* may need to install CORS plugin https://chrome.google.com/webstore/detail/allow-control-allow-origi/nlfbmbojpeacfghkpbjhddihlkkiljbi

## Client
* Client will display a list of ten songs at a time
* Clicking on a song will show royalties associated with particular songs
* Clicking next moves to next page
* Clicking previous moves to previous page (if available)

### Opportunities
* Client owns all logic for matching royalties to song id
  * Ideally server would own this logic and return royalty by id
* Styling needs to be cleaned up and standardized
* Previous and next button should be hidden and disabled when not available
  * Previous is disabled on page one - Could also be hidden
* Opportunity to incorporate Redux
  * Store songs?
  * Map royalties to song and store on client?
* Stretch goal - Add search functionality

## Server
* Server calls Wurrly endpoints returning all songs and all royalties

### Opportunities
* Add functions for 
  * Song by id
  * royalty by id

## Feedback
I enjoyed this exercise and found it challenging.  Time management became very important, as this type of application has the potential to become quite large quickly.

### Challenges
* Needed to use CORS plugin to hit Wurrly endpoint