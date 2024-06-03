## Base Required Features 

- Multi-Part Form:  
  - [x] Able to add feedback
    - [x] Data collected on individual pages & components
    - [x] Click on next takes you to the next page in sequence
    - [x] Data saves in DB after *all* the parts are completed (not piecemeal)
    - [x] Thank you page takes you back to the first view

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
  - [x] React-Redux Working
    - [x] `useDispatch` in components correctly & dispatching Actions onClick
    - [x] `useSelector` when data is needed from Redux for submission
  - [x] Axios POST request to add feedback

- Server code:   
  - [x] Router, with a `POST` endpoint to submit feedback


## General Items
Feedback should be provided for these items, but they do not impact scoring.

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

- Previous Steps
  - [ ] allows a user to go to a previous step, either directly or by cycling backward thru the steps
  - [ ] user can update their score for a step
    - [ ] new score is validated to not be empty
    - [ ] redux is updated with new score
  - [ ] user can continue on to review page and submit as in Base Mode


- Admin View
  - [ ] All entries are visible with correct data from inputs
    - [ ] Most recent is at the top
  - [ ] Can Delete an entry
    - [ ] User is prompted before deleting
  - [ ] Axios GET request to get all feedback for `/admin` view in componentDidMount

- [ ] Styling with Material UI
- [ ] Ability to flag a feedback item on `/admin` for further review
- [ ] Deployed to Heroku

## Markdown

```
Hey Eyan, great job on the project. I like the button hover effect that makes then turn blue when you hover over them to click. I would've maybe done a bit more with the CSS/font style/graphics, but other than that this is a solid project. Lots of descriptive code comments, lots of descriptive commits, and everything seems to be functioning properly for the base goals. Well done. 

```
---
| Functional Requirements | Complete? |
| --- | --- |
| Multi page form with client side routing and navigation (next button) | YES |
| Data stored in Redux when navigating from page to page | YES |
| User is notified when trying to leave a blank score | YES |
| Review Component displays scores and comments from current redux state | YES |
| Submit button sends data to the server via Axios | YES |
| Confirmation Page displays after data is POSTed to the server | YES |
| Button on Confirmation Page starts a new survey | YES |
| Views are broken down into components | YES |

---
### Notes:

Great work on getting everything functioning properly. 

---
| General Items | Complete? |
| --- | :---: |
| More than 15 git commits | NO, it was 15 exactly though. |
| Commits are descriptive of the changes made or feature added | YES |
| Readme file updated | YES |
| Appropriate amount of code comments | YES |
| Code is consistently formatted | YES |
| Server code organized with router & module files | YES |
| Dispatch action to clear redux state on new survey | NO |

---
### Notes:

There were exactly 15 git commits. There is no dispatch to clear the redux state because it's starting off as an empty array, so I'm not sure if you would actually need one to reset everything. 

```
