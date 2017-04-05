## MVP Specs

Generally, there are several maps that will be of use for this project.  All of our APIs so far have been in GeoJson format.

### Display Conflicts between projects
One thing that would really help PBOT, and save the city some money, is a display of projects that are close to one another in space and time.  We would like to display any features that are close to one another on a map.  "Close" can have a default but it would be great to allow the user to set values for time and distance as part of the query.

### Provide a form for data overrides
Some of the City API data seems to be inaccurate.  In order to get good project conflict data, we would like to provide a way for a user to manually input start and end dates, and status.  Elements that would be useful on this page:
* A radio button or dropdown that would allow users to select which data source to work with
* A list of the features in the selected data source
* A map to that shows the feature when it is selected
* A place to show the detailed properties associated with a feature.  This could either be tool tip on a map or a separate box.
* Writeable fields for start date, end date, and status

### Location lookup
A page that allows the user to enter an intersection or address and would then display a map with nearby features.  Date and distance selectors would also be helpful.

### Waze 
Waze has a particular spec for submitting data to their database. We'd like to do the backend work to prepare that file so it could, for instance, be submitted to Waze every morning.
