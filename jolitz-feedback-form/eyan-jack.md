# Weekend Challenge 11 - React-Redux Feedback Form

- Review the code from your partner and give relevant feedback
- Complete the Markdown section and submit that in the notes section on the assignment app. (Make sure you include who's code you reviewed.)

Hey, Jack!

You crushed the base goals! Great job, man! Not too many things I would change. One of the main ones is the amount of comments on the page. I think it is super nice as a reader to know what your code is doing. However, I would say it is quite a bit more than needed. Maybe just simplify your comments a little more to talk about what the code block is doing(if there is one) and not go line by line. Overall your code is actually really clean. I thought it was super easy to read through overall which is great. 

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
As far as feedback is considered for the general items, I think you have the exact same amount of commits I do haha. So I have to say I think it is a great amount of commits. You have some really good commit comments. But some do trail off a little bit. Overall though they were very concise. Your Readme.md file is great. I would say you could add some pictures in there too! I like the purple vibe of your project, show it off! Styling also looks great.

- Git 
  - [ ] More than 15 git commits showing incremental progress,
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

The stretch goal was good! I think the only missing thing was getting the stored state to show up in the input when the user went back. Once the user goes back and updates their score and it is correctly stored in state and can go to the review page. Great Job on that, Jack!

- Previous Steps
  - [x] allows a user to go to a previous step, either directly or by cycling backward thru the steps
  - [x] user can update their score for a step
    - [ ] new score is validated to not be empty
    - [x] redux is updated with new score
  - [x] user can continue on to review page and submit as in Base Mode
