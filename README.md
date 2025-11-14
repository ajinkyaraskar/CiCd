## This project shows how to work with github action pytest docker  
### Reference 
https://www.youtube.com/watch?v=ciqWMIf7Pz0&t=83s  
https://www.youtube.com/watch?v=9oALxmc5yEw&t=25s

### Notes
Github automation tool to automate tasks, create custom workflow
It can be triggered by 
push 
pull
schedule 
Can be used for CICD and testing

Any file that uses test_ will be considered test file by pytest


CI: build and test that current code isnt broken whenever push changes or merge
CD: after passing all tests deployment to various env like staging and production.

We need a yaml for cicd workflow

env 
Dev > QA > UAT > Production

**Key stages**
1. Code
2. version control: commit branches push pull resolve conflict
3. code review: Peer review, Architect review
4. testing:
   a.Automated testing: unit testing, integration testing, end to end
5. Continuous integration
   a.Building
   b.testing
   Developer needs to be notified to fix it
6. Continuous deployment
   QA env
   UAT env

**Continuous integration** 
when a PR is opened CI pipeline is triggered and 
it builds appn and runs test cases
If pipeline passes PR is approved and merged to main

**CD** 
upon PR is merged CD pipeline is triggered and its deployed to staging or dev env
Then deployed to Production.

## main
**womain** hehe


**.yml**

name, on, job

Event
in workflow push, pull, merge, delete act as event
Using "on" we define event
https://github.com/ajinkyaraskar/GitCiCd/tree/main
