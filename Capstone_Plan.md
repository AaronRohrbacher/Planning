# Plan for StudiSchedule development

## StudiSchedule
_A roster application for your school's lesson and class studios, or your own private lesson studio_

## M.V.P
* SuperUsers (me) can create schools or studios via the command line
* Teachers can list their current classes and/or students.
* Admins can add update and delete Users, classes, and students.
  * Users can be Admins, teachers, or students.
  * Users are linked to accounts, which are never destroyed, but rather marked as active or inactive (for future mailing lists, etc.)
* Admins can initiate events
  * Events can be classes, private lessons, or 'other' (meetings, etc.)
  * Events should have a start and end dateTime
  * Events should occur in a room.

## Beyond the M.V.P.
  * Teachers and students or classes are linked to a Board, where a teacher can leave lesson/class notes, upload materials, and the student can view and communicate.
  * Events in a room cannot be double booked.
  * Events can recur
  * Events can recur for a specified amount of time
  * Events can recur on specific days
  * A full-school room calendar can be viewed.

## Anticipated Model Structure



## Development schedule
* Weekend:
  * Further research gems regarding scheduling (not much luck yet), which may take things out of "beyond the M.V.P." and move them to "M.V.P."
  * Research Google Calendar's API to see if that might work instead.
  * Generate models and controllers for the app's current adjusted MVP. Doesn't have to look like much, but relationships should be functional and accurate, at least via the Rails Console.
  * Take a peek at adjusted "Beyond the M.V.P." features. Will your current models support adding these features?
* Monday:
  * Generate views based on models and controllers. Integrate AJAX/jQuery where appropriate to make a nice UX.
  * Spend good time on the user experience. Are admins seeing what admins should see? Are teachers seeing what teachers should see? Are students seeing what students should see?
  * Answer this question: Am I ACTUALLY ready to look at a "Beyond the M.V.P." feature? If so, look ahead to Tuesday. IF NOT, DON'T.
* Tuesday:
  * Depending on how Monday went, start looking at "Beyond the M.V.P." features. Build models and controllers, getting features to work ONE AT A TIME.
  * Follow each feature with a simple view.
* Wednesday:
  * Continue building "Beyond the M.V.P." features. At this point in the game, DON'T FUCKING BREAK ANYTHING! If a feature is interfering too much with existing code, refactor the feature, not your working application.
  * By 5pm Wednesday, the functional aspects of the application should be complete.
* Thursday:
  * Avoid (by and large) writing any more code. Spend good time cleaning up the UX, refactoring any obvious non-DRY code (Don't you dare break anything!), and making this thing shine.
