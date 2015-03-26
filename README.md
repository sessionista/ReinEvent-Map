ReinEvent-Map
=============

### Description
This is a Revamp of the previous map events project for the Smith College Spatial Analysis Lab created by the RenSol programming team.

Here (hyperlink)


### Links
- Events Calendar: http://www.smith.edu/calendar/#/?i=3
- Event Visualization: 

### How it Works:
	- From ArcMap every event location (from the list of possible event
      locations to book for events) has been given a point by hand 
	- From CartoDB the code gets the list of buildings
	- From the Events Calendar the code gets the XML code from the events
      page and parses through it. There are five catagories of events
      that it pulls information from: Featured, Student Interest,
      Lectures and Symposia, Multicultural Events, and Atheletic Events
	- The code pushes all the event info into the CartoDB database
    - The code then maps all the events to their respective locations
      (a building on campus).
	- The visualization can then be viewed at (hyperlink) with an updated
      list of events.
    	- NOTE: The points are sized relative to the number of events at
        		that location.
        - NOTE: Each point can be selected to see what events are happening
        		at a specific building, and other information pertinant to
                that event (e.g. date, time, location)
    - The map is scheduled to update daily


### POSSIBLE UPDATES
- fix navigation between 5 event pages
- add an info window explaining the project. hover or click.
- want points to be over map. maybe check that out. is inconsistent


### UPDATE AND MAINTENANCE INSTRUCTIONS
- Email the Events Management Office and get an updated list of events
- Briefly look over the code. See what you’re up against. Read the documentation.
	- NOTE: the code is presently in Python2
- Update the ArcGIS map by hand. Check to make sure every single event has a point using the new updated list.
	- NOTE: the code will parse over events it can’t identify, but it would be best to account for as many as possible so this is important for identifying new locations, buildings with changed names, etc.
	- NOTE: you will find a lot of event locations you never could have imagined. isn’t that cool?
- Go back to the code. Make sure you know how it works in case it crashes. Feel free to make more efficient.
