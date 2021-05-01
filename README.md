# Yelp-Roulette
[Yelp Roulette Site](http://yelp-roulette.me/Yelp-Roulette/)
### Requirements: 
1. The user should be able to press a button to generate a restaurant in one click/touch.
2. Interface should be very simply designed and very streamlined in presenting the restaurant information.
3. System should be able to get user's location data, or allow user to type in a city and state. 
4. System should be able to take user to restaurant's Yelp page after restaurant has been generated.

### Use Cases:
![Use Case Diagram - Individual](https://user-images.githubusercontent.com/69657272/112183043-3dbc2480-8bd4-11eb-8d54-3aa09ac380b7.png)


| Name           |  Input Location |
|----------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| ID             | uc01  |
| Description    | The user will input their location in a city, state-abrreviation format |
| Triggers       | User choosing to input a location, rather than just being geolocated by the system|
| Postconditions | User's location data will then be used to generate the restaurant|
| Main Course    | System prompts the user to enter a location from which to generate a restaurant from.            |

| Name           | Generate a Restaurant                                                                                                                |
|----------------|-------------------------------------------------------------------------------------------------------------------------------------------|
| ID             | uc02                                                                                                                                      |
| Description    | The user prompts the system to begin generation of the restaurant                                                                         |
| Triggers       | Clicking button that indicates initiation of roulette       |
| Postconditions | System will have prepared a generated restaurant for the user to view                                                                     |
| Main Course    | System presents a button that will serve to initiate restaurant generation for the user |

| Name           | Access Yelp Page of Generated Restaurant                                                                                           |
|----------------|----------------------------------------------------------------------------------------------------------------|
| ID             | uc03                                                                                                           |
| Description    | The system will give users a clickable link to access Yelp page of restaurant that was generated                       |
| Triggers       | Restaurant being generated                                                                                                |
| Postconditions | User will now have option to view yelp page of the generated restaurabt in its entirety                         |
| Main Course    | System displays link upon generation of resataurant which will take the user to the Yelp page once clicked |



### SPMP *(Software Project Management Plan)*
<details>
  <summary>Contents</summary>
    
  1. [Introduction](https://github.com/LanoCodes/Individual-Project-COSC412/blob/main/README.md#introduction)
  2. [Project Organization](https://github.com/LanoCodes/Individual-Project-COSC412/blob/main/README.md#project-organization)
  3. [Managerial Process](https://github.com/LanoCodes/Individual-Project-COSC412/blob/main/README.md#managerial-process)
  4. [Technical Process](https://github.com/LanoCodes/Individual-Project-COSC412/blob/main/README.md#technical-process)
  5. [Description of Work Packages](https://github.com/LanoCodes/Individual-Project-COSC412/blob/main/README.md#description-of-work-packages)
  
</details>

#### Introduction
1. Project Overview
>The purpose of this system is to be able to take the fuss out of picking a new place to eat and give the user a restaurant nearby that they "must" go to, i.e. Roulette. It will not allow the user to choose any preferences about the restaurant beforehand, such as the type of food served, whether or not it has a bar, etc. Instead, the user's location will be determined, or the user will specify a city and and have a restaurant be picked for them.
2. Project Deliverables
- All items to be delivered:
    -  Class Diagram
    -  Use Cases
    -  Tool Rundown
    -  Mock up of site
    -  Bootstrap rendition of the site
    -  Connection etablished to Yelp's Fusion API
    -  Successful in-site test of core function; display a result from Fusion
      -  Milestones: 
        - Have mockup copleted: 4/9
        - Have bootstrap rendition made: 4/12
        - Get output squared away & user friendly: 4/28
        - Have site hosted & up: 4/30
3. Evolution of the SPMP
- Should the system be a success and more features/pivots in function become wanted:
    -  The plan will than be reworked and then be based on an already running system, rather than as a project being built from the ground up
- If costs to run/host/test project becomes exorbitant:
    -  Update professor immediately and seek alternative demonstration methods to alleviate burden. GitHub offers the ability to host projects, so this may not be a major concern. However, should this occur a reworking of the project plan will need to be done accommodate this.
  

4. Reference Materials 
- [Yelp's development portal](https://www.yelp.com/developers)
- [MDN Web Docs](https://developer.mozilla.org/en-US/)
- [Browserify's README](https://github.com/browserify/browserify)

5. Definition and Acronyms
- SPMP: Software Project Management Plan
- “The System”: Refers to the piece of software we intend to build
- API: Application Programming Interface

#### Project Organization
1. Process Model
  - Agile process model
  ![Agile Development Diagram](https://user-images.githubusercontent.com/69657272/112192422-4fee9080-8bdd-11eb-8f2e-a64335fce865.png)

2. Organizational Structure
- Delano Powell, student, is in charge of all project facets. 
  - Reports to course professor, as this project is in development on assignment for school
- General project oversight comes from the Professor

3. Organizational Interfaces
- GitHub:
  - GitHub is the proposed hosting service version control service
- Yelp
  -  Yelp is the provider for the API that will be used for the core of this project

4. Project Responsibilities
- Delano Powell is in charge of all duties, deliverables, and project overall

#### Managerial Process
1. Management Objectives
- Management Philosophy:
    - Commit to doing the best job possible in the time allotted
    - Personal accountability should be the root of everything done throughout the project
    - Meet mistakes/errors often as necessary, early.

2.  Assumptions, Dependencies, and Constraints
  - Constraints:
    - There will be a limit on how many times the app will be able to run using my personal credentials when the app is live. However, the amount of people exposed to this app will only encompass class participants at most. That is well within range for demonstration.
  - Dependencies: 
    - The app is entirely dependent on Yelp's Fusion API. Should that crash/fail, there will bbe no alternative.
  - Assumptions:
    - Yelp's Fusion API will not make a drastic change to their restaurant endpoints
      -  They have remained stable for some time

3. Risk Management
- Scope Creep:
  -  In an effort to mitigate potential scope creep, I will strive for an agile process that truly refuses to tack on new features until the project has completed a working iteration.

4. Monitoring and Controlling Mechanisms
- Gantt Chart:
  -  The [Gantt Chart](https://app.clickup.com/8645017/v/g/6-65360568-7?pr=14764423) for this project will be the primary mode of tracking progress and controlling development rate 

5. Staffing Plan
- As mentioned, all positions relevant to this project is the sole responsibility of Delano Powell
  -  Staff total: 1
    -  Staff: Delano Powell

#### Technical Process
1. Methods, Tools, and Techniques
- Tools: 
    - Yelp's Fusion API
    - GitHub Pages
    - HTML5, CSS, JS
    - Bootstrap
    - Heroku
    - Namecheap
    - Browserify
    - NodeJS & npm

2. Software Documentation
- This repo will serve as the site for software documention. 
- Being that Agile developent is in use, a lot of just-in-time will be used.
  - This repo will be updated with any new documentation as they are created throughout the lifescycle of this project
3. Project Support Functions
- Plan to ensure quality assurance:
  - Tester individuals will be used to run the system individually and I will document their findings throughout their usage time in a document to come.
- Verification and Validation plan
    - Error testing thoughout each iteration
    - Regularly checking in on Yelp's API health to ensure on status
    - Regularly testing host site link(s) to make sure site is live 
#### Description of Work Packages
1. Work Breakdown Structure(WBS):
  - ![WBS](https://user-images.githubusercontent.com/69657272/112224956-6fe47b00-8c02-11eb-8a75-80ccd99d1a50.png)
2. Dependencies Between Tasks:
  - Testing tasks are all dependent on completion of Implementation tasks

