# Tournament Schedule

###Overview
Flyball Master version 1.0 does not create a Tournament schedule. The schedule must be imported from an external source. The schedule import should be the first activity when setting up a new Tournament.

This section details the process to import a schedule, the format neeed, and steps to take after the import is complete.

###Schedule Import
Flyball Master allows a schedule to be imported from a comma separated value file (CSV). The format of the file is critical. The following line defines the format. The first line of the file must be the data for Race #1.

```
Race Num, Left Team, Right Team, Breakout Time, Race Format, Division<return>
```

A sample line of data should look like:

```
1,MC Butterfly Effect,WW Hurricanes,0,3 of 5,M1<return>
```

Data Requirements:

### Race Num
Must be an integer number starting at 1 (ie. 1, 2, 3...)

###Left and Right Teams
Word 1 must be an abbreviation for the team's club name. This ideally should be no more than 4 letters and is prefered to be all Caps. The remaining words are the team name. 

In the example line above, MC is the club abbreviation of "Mass Chaos" and "Butterfly Effect" is the team name.

###Breakout Time
Must be a number. For divisions with no breakout time use "0".

###Race Format
Must be text. The data must be of the form "<integer> of <integer>". Examples are "3 of 5" or "4 of 4".

###Division
Must be a single letter {O, R, M, V} representing the class followed by an number.

###More Information
Upon importing the schedule, any division or club that is not existing in the data file are created. Also, all teams are added to the event.

###Conflict Resolution
Flyball Master determines potential team and club conflicts when importing. Any conflicts are indicated by yellow and red circles on each race.

Yellow indicates there is a conflict with the club. Red indicates the team has a conflict.

A conflict is defined by how many races thee are from the current race to the next time the club or team races. The number of races triggering a conflict is configurable.

To change the conflict numbers, navigate to the settings screen. You will see 2 fields there allowing for input of club and team conflict race intervals.

A team should be allowed a minimum 45 minutes of rest before racing again. In a typical single ring, round robin Flyball Tournament, team conflict should be set to 6. In multi-ring tournaments, this number should be multiplied by the number of rings at the event.

It is recommended that a club have a minimum of 3 races between racing so that members are able to transition between races. At multi-rings events, this number should be multiplied by the number of rings at the event.

###Resolving Conflicts
Resolving conflicts is easy with Flyball Master. First step is to eliminate as many of the red conflicts as you can. Conflict resolution does take some practice. To move a conflicting race to a new location, simply click and drag (hold down the mouse button) to move the race to a new location.

Release the mouse button to insert the race at the new location. Flyball Master's conflict resolution engine kicks in at this point. Any changes to conflicts are immediately displayed on the screen.

###Schedule Export
Once a schedule is created, you can export it our of Flyball Master. This allows creation of file that can be used to communicate the schedule to teams. Also, teams are able to create there on custom race schedule forms for the event.

###Schedule Lock
It is critical that the schedule not change when it is determined to be final. Click the "Lock" button to lock the schedule. Once the schedule is locked, it is not possible to make any changes to the the schedule.



