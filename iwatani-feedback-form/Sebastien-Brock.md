- Multi-Part Form:  
  - [x] Able to add feedback
    - [x] Data collected on individual pages & components
    - [x] Click on next takes you to the next page in sequence
    - [x] Data saves in DB after *all* the parts are completed (not piecemeal)
    - [x] Thank you page takes you back to the first view
    - [x] Old Data is cleared on form completion

- Client code:
  - [x]  Individual components for each form part
  - [x]  Redux setup complete
    - [x] Store linked to react with `<Provider>`
    - [x] Store setup with reducer(s) and logger middleware 
  - [x] Reducers & Actions Working
    - [x] Actions are in SCREAMING_SNAKE_CASE and semantically named
    - [x] Actions have a `type` key, and `payload` if sending data
    - [x] Reducers are returning a new state, or the old state (not mutating)
    - [x] Reducers are using spread correctly (to keep old data, while adding new)
  - [x] Review Component shows at all times with current redux state
  - [x] React-Redux Working
    - [x] `connect`ing components correctly & dispatching Actions onClick
    - [x] `mapStateToProps` when data is needed from Redux for submission
  - [x] Axios POST request to add feedback


- Server code:   
  - [x] Router made for GET, POST


## General Items
Feedback should be provided for these items, but they do not impact scoring.
-- 15 commits
-- could've added more code comments
- Git 
  - [x] Multiple git commits showing incremental progress
  - [x] Commits are descriptive of the changes made or feature added 
  - [x] Has .gitignore with node_modules
  - [x] Readme file updated (assuming this is previously discussed)
- Code Style 
  - [x] Appropriate amount of code comments
  - [x] Code is consistently formatted
- Client
  - [x] Appropriate use of HTML tags
  - [x] Basic CSS styling with margins/padding


## Stretch Goals
First must be complete for score of _5 - Exceeds Expectations_

- Previous Steps
  - [x] allows a user to go to a previous step, either directly or by cycling backward thru the steps
  - [x] user can upate their score for a step
    - [x] new score is validated to not be empty
    - [x] redux is updated with new score
  - [x] user can continue on to review page and submit as in Base Mode


- Admin View
  - [x] All entries are visible with correct data from inputs
    - [ ] Most recent is at the top
  - [x] Can Delete an entry
    - [ ] User is prompted before deleting
  - [x] Axios GET request to get all feedback for `/admin` view in componentDidMount

  Busywork Goals, consider removing or making more useful

- [ ] Styling with Material UI
- [ ] Ability to flag a feedback item on `/admin` for further review
- [ ] Deployed to Heroku


## Markdown

```
Hey Brock,

General Feedback.

---
| Functional Requirements | Complete? |
| Yes | 
| Multi page form with client side routing and navigation (next button) | Yes |
| Data stored in Redux when navigating from page to page | Yes |
| User is notified when trying to leave a blank score | Yes |
| Review Component displays scores and comments from current redux state | Yes |
| Submit button sends data to the server via Axios | Yes |
| Confirmaion Page displays after data is POSTed to the server | Yes |
| Button on Confirmation Page clears Redux and starts a new survey | Yes |
| Views are broken down into components | Yes |

---
### Notes:

Notes on the above Functional Requirements.

---
| General Items | Complete? |
| Yes |
| More than 15 git commits | Yes |
| Commits are descriptive of the changes made or feature added | Kind of - could be a bit more descriptive |
| Readme file updated | Yes |
| Appropriate amount of code comments | Yes |
| Code is consistently formatted | Yes |
| Server code organized with router & module files | Yes |

---
### Notes:

Notes on General Items

You had exaclty 15 commits, you could be a bit more descriptive of the changes made. 

You had an appropriate amount of comments but it wouldn't hurt to add more. 

The application looks great, I like the css, good job.
