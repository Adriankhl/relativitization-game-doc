# Feature plan

Keep a note of the planned features to be implemented to the game

## TODO

These features will be implemented.

* Alliance, be careful on synchronizing war state and peace treaty under the time delay
* Decrease satisfaction if salary is reduced
* Destroy buildings when at war
* Pop rebel when satisfaction is too low
* Decrease relation when a factory is removed
* Refactor movement from event to physics

## Brainstorm

These features may or may not be implemented.

* Trade treaty negotiation
* UI: use `Camera` to zoom instead of manually zooming `Group`
* Transfer/retract player command
* Transfer/retract carrier command
* Science era, e.g., Biology era favour nation with more biologist
* Physics: time dilation of photon rocket
* Physics: momentum conservation when sending fuel (transfer opposite momentum by virtual photon?)
* UI: Display ai-relevant data

## Done

These features have been implemented.

### Core

* Optimize afterimage and load saved universe to reduce memory usage [x]

### Data

* Fuel and resource weight instead of target amount [x]

### Command

* Destroy factory [x]
* Send fuel to foreign factory [x]
* Change economy policy, e.g., tax, storage [x]
* Change politics data [x]
* Change salary [x]
* Build institute and laboratory [x]
* Improve diplomatic relation by sending resource [x]
* Declare war, declare independence [x]
* Merge direct subordinate at exactly the same position [x]
* Open and close factories [x]

### Mechanisms

* Basic resource output from stellar system [x]
* Pop update daily need [x]
* Salary, and allocate pop to factory, institute and lab [x]
* Pop buy resource to fulfill need [x]
* Pop growth: Medic [x]
* Education level: educator [x]
* Entertainment production: entertainer [x]
* Tax and tariff, send to leaders [x]
* Research [x]
* How research affect product [x]
* Export center [x]
* Basic diplomacy [x]
* Merge carrier [x]
* New carrier [x]
* New player [x]
* Basic military: Soldier [x]
* Sync leader data to subordinate, e.g., enemy [x]
* Sync economy data to subordinate [x]
* Stop war after long period of time [x]
* Adjust attack and export by time dilation [x]
* Limit fuel produced in a single unit space cube to prevent unlimited population [x]
* Adjust the price and quality bound based on overall desire and trade [x]
* Attack spend production fuel [x]
* Pop buy resources from other players [x]
* Pop growth rate affected by salary factor [x]

### Default AI

* AI state store last command to subordinate [x]
* Review resource factory construction after desire change [x]
* Decrease salary and increase price when pop saving is too much compare to storage [x]
* AI build factory on other players [x]

### Universe generation

* One stellar per player generation [x]
* Generate proper knowledge network [x]

### UI

* Map mode [x]
* Show execute warning [x]
* Filter resource factory by resource type [x]
* Default build factory and institute employee to population, research equipment to production [x]
* Rotation based on next position [x]
* Optimize UI observer pattern, only change what is shown [x]

### Test

* Declare war [x]
* Combat [x]
* Propose peace [x]
* New player [x]
* Merge player [x]