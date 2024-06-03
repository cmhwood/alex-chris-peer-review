Hey Said,

General Feedback.

---
| Functional Requirements | Complete? |
| --- | :---: |
| Multi page form with client side routing and navigation (next button) | yes |
| Data stored in Redux when navigating from page to page | yes |
| User is notified when trying to leave a blank score | yes |
| Review Component displays scores and comments from current redux state | yes |
| Submit button sends data to the server via Axios | yes |
| Confirmation Page displays after data is POSTed to the server | yes |
| Button on Confirmation Page starts a new survey | yes |
| Views are broken down into components | yes |

---
### Notes:

Nice job Said! Great work on the validation!

---
| General Items | Complete? |
| --- | :---: |
| More than 15 git commits | no |
| Commits are descriptive of the changes made or feature added | yes |
| Readme file updated | yes |
| Appropriate amount of code comments | no |
| Code is consistently formatted | yes |
| Server code organized with router & module files | yes |
| Dispatch action to clear redux state on new survey | no |

---
### Notes:

Could use some more documentation in your components. Also you have cases in your reducers to reset the data but the routes are not used. These can be called in your handleSubmit .then() in the review page when the data is successfully sent to the database.

Overall, good job on this project!
