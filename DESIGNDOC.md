# Memoria Project Recorder - Design Doc
```
  . . . .  . . . .  . . . .  . . . .  . . . .  . . . .  . .   Authored By Jesse Muniz
  . . . .  . . . .  . . . .  . . . .  . . . .  . . *@@  . .   Reviewed By Nobody
  . . . .  . . . .  . . . .  . . . .  . . . .  @@@@@,.  . .   Started on 8/6/2022
  . . . .  . . . .  . . . .  . . . .  . . . @@@@@@@. .  . .   Finished in the future
  . . . .  . . . .  . . . .  . . . .  . @@@@@@@@@@ . .  . .   Referenced materials at end of doc
.. . . . .. . . . .. . . . .. . . . . @@@@@@@@@@@ . . .. . .
.. . . . .. . . . .. . . . .. . . .@@@@@@@@@@@@ . . . .. . .
.. . . . .. . . . .. . . . .. . @@@@@@@@@@@@@@. . . . .. . .
.. . . . .. . . . .. . . . .. @@@@@@@@@@&.@@ .. . . . .. . .
  . . . .  . . . .  . . . . @@@@@@@@@@@@@@. .  . . . .  . . 
  . . . .  . . . .  . . .@@@@@@@@@@@@@@@. . .  . . . .  . . 
  . . . .  . . . .  . .&@@@@@@@@@@@@@@. . . .  . . . .  . . 
  . . . .  . . . .  . @@@@@@@@@@@@@@  . . . .  . . . .  . . 
  . . . .  . . . .  @@@@@@@@@@@@@@ .  . . . .  . . . .  . . 
.. . . . .. . . . .@@@@@@@@@@@@@. . .. . . . .. . . . .. . .
.. . . . .. . . .&@@@@@@@@@@@ . . . .. . . . .. . . . .. . .
.. . . . .. . . @@@@@@@@ . .. . . . .. . . . .. . . . .. . .
.. . . . .. . .@@@.. . . . .. . . . .. . . . .. . . . .. . .
  . . . . @@@@@@@@@@. . . .  . . . .  . . . .  . . . .  . . 
  . . . . @@@@@@@@@@. . . .  . . . .  . . . .  . . . .  . . 
  . . .@@@@@@@@@@@@@@@@ . .  . . . .  . . . .  . . . .  . . 
  . . .@@@@@@@@@@@@@@@@ . .  . . . .  . . . .  . . . .  . . 
  . . .@@@@@@@@@@@@@@@@ . .  . . . .  . . . .  . . . .  . . 
.. . .%@@@@@@@@@@@@@@@@. . .. . . . .. . . . .. . . . .. . . 
```
#

## Abstract
Build the underlying tooling for a GUI based project tracking tool. Using Rust and a RDBMS like MySQL it will help produce a story by using data like a history of issues, project management structure, project goals, sprints/iterations, track hours logged and project status. Memoria should be quick to setup on a git project. Should allow for an easy output format as well

#

## Objective
Memoria will record the following in an RDBMS and maintain project specificity

1. Project Scope/Definition
2. Project Management Style
3. Project goals/milestones
4. Project contributors
5. Sprints/Interations etc.
6. Hours spent
7. Current status
8. Issues solved
9. Current Issues
    
#

## Out of Scope Pitfalls

1. Will not have a GUI
2. Will not have edit capability
3. Will not support multiple export formats
4. Will not support multiple RDBMS
5. Will not have cross folder support only sub folder

#

## Design Highlights

### Phase 1
Establish the capability to build a CLI app with rust and push data to SQL. (M1-3)
  Program should start up from an exe and push a single piece of data to sql after data is entered into the app.

### Phase 2
Add features to build out CLI capability to full scope of the app. (M4, M5)
  Program should be able to setup a project, log a two issues and goals, then finish an issue and goal.

### Phase 3
Polish app to release state and subject myself to criticism. (M6, M7)

### Phase 4
Polish app to release state and subject myself to criticism. (M8-10)

#

## Milestones

### Finish CLI Rust Tutorial - M1
- Est. 2 hours

### Establish Ability to write to MySQL - M2
- Est. 8 hours
  
### Setup Rough interface and commands - M3
- Est. 16 hours

### Establish Ability to write/read files - M4
- Est. 12 hours

### Move logins and config settings to config file - M5
- Est. 24 hours (No experience here)

### Scaffold output file and SQL tables/procedures - M6
- Est. 2 hours

### Produce a simplified file - M7
- Est. 2 hours

### Build final CLI interface - M8
- Est. 16 hours

### Build final file output - M9
- Est. 24 hours
  
### Perform code review with Mentor and incorporate changes - M10
- Est. 8 hours

#

## References - APA Citation

Babich, N., &amp; Morales, J. (2020, April 22). Design documentation. Ideas. Retrieved August 6, 2022, from https://xd.adobe.com/ideas/principles/web-design/design-documentation/ 

Google. (n.d.). Design Documents. Design documents. Retrieved August 6, 2022, from https://www.chromium.org/chromium-os/chromiumos-design-docs/ 

Ludicchart. (2020, November 18). How to create software design documents. Lucidchart TechBlog. Retrieved August 6, 2022, from https://www.lucidchart.com/blog/how-to-create-software-design-documents 

Zhang, A. (2018, June 8). How to write a good software design doc. #SOFTWARE DEVELOPMENT. Retrieved August 6, 2022, from https://www.freecodecamp.org/news/how-to-write-a-good-software-design-document-66fcf019569c/ 