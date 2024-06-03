Hey Andrew,
Multi-Part Form:
    - Data from the user is collected on each page. 
    - The user is well informed of what input to provide.
    - There is form validation and error message was informative
    - Next page routes to the correct page
    - Data is save on database after submit button is clicked
    - User can go back to home page to start a new feedback

Client code: 
    - There is component for each page
    - Used redux to store data, linked Provider and used logger middleware
    - Actions in reducers are in the correct case
    - used type and payload when sending data
    - reducers send new data

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

Met all the base goal requirements. The user is well informed about errors. Good Job.

---
| General Items | Complete? |
| --- | :---: |
| More than 15 git commits | yes |
| Commits are descriptive of the changes made or feature added | yes |
| Readme file updated | no |
| Appropriate amount of code comments | no |
| Code is consistently formatted | yes |
| Server code organized with router & module files | yes |
| Dispatch action to clear redux state on new survey | yes |

---
### Notes:

Met most of the requirements, had good amount of commits, and just needed to include code comments.
Good job.