# ci-fish
CI system which is trying to solve different problems for developers using simplifying and swimming in docker bowl


## Project Status
Currently only a collection of ideas


## Problems

### The Problems ci-fish is trying to solve
* Many CI systems are hard to install 
* Many CI systems are hard to maintain over the time
* Many CI systems are not supporting developer with their development and delivery process
* Many CI systems are not helping developer to get rid of manual tasks like maintaining changelogs, release notes, etc.
* Many CI systems are becoming a vendor-lock-in
* Many CI systems are hard to run locally 


### Ideas how to solve the Problems?
* Using docker to ship the ship the product to ensure it can be easily downloaded, installed and run
* Using yaml files for configuration to ensure it is easy to maintain.
* Using no database to ensure it is simple to restore and behaving as a self contained service.
* Using REST interfaces to ensure it can be easily interfaces and integrated into other tooling
* Using json payload for all interaces to ensure the input/output can be easily processed
* Using (web) hooks to provide information/data to other systems like chatbots, other build systems, etc.
* Building a system around common development and delivery processes that automates all manual work to ensure the system fits to your process
* Avoiding all kind of non open source components to ensure we are avoiding a vendor-lock-in


## Implementation Ideas

