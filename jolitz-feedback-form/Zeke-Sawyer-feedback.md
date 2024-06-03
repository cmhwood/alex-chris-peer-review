Hey Sawyer,

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

Notes on the above Functional Requirements.

---
| General Items | Complete? |
| --- | :---: |
| More than 15 git commits | no |
| Commits are descriptive of the changes made or feature added | yes |
| Readme file updated | yes |
| Appropriate amount of code comments | no |
| Code is consistently formatted | no |
| Server code organized with router & module files | no |
| Dispatch action to clear redux state on new survey | no |

---
### Notes:

Notes on General Items

The code works pretty well, I do like how your comment component will prevent the user from typing too long of a comment.

My general notes on formatting is there is a bit of flip-flopping with quotations, and single quotes in the react components, as can be seen here. 

```
<div className='Input-box'>
       <div className='header-container'>
       <Typography variant="h5" gutterBottom>How well are you being supported?</Typography>
      </div>
    <Input
    type="number"
    min="1"
    max="5"
    step="1"
    placeholder='Choose 1-5'
    value={supportedValue} 
    onChange={(evt) => setSupportedValue(evt.target.value)} 
    />
    <div className='button-container'>
    <Button variant="contained" onClick={handleSupported}>Next</Button>
    </div>
    </div>
```

The intellisense for react is pretty weird, and I think I may have done the same thing. Just something to keep in mind.
Another issue with formatting I see is that there is a ton of unnecessary whitespace in some areas of the code. The biggest offender is App.jsx where there is about five lines of whitespace inside the function. I usually only have up to two lines of whitespace at most. I sometimes use three lines of whitespace, but that is for when I know I am going to revisit the code later to add something to fill that space.

There is also some funky indentation, and curly brackets going on in each of your number forms, as can be seen here
```
function handleSupported() {
      if (supportedValue >= 1 && supportedValue <= 5) {
        dispatch({type: 'SET_SUPPORTED', payload: supportedValue});
        console.log(supportedValue, 'was selected for how supported they feel');
        history.push('/comments')
    } else {
      alert('Please enter a value between 1 and 5 to continue.')
    }}
```
This can be confusing if someone is trying to figure out where this code starts and ends. This issue can easily be fixed by keeping the curly brackets from touching each other, and using command f to auto format your code.

Moving on to some formatting on the server side. Having any functions after app.listen feels smelly to me. Obviously the code works just fine here, but I just don’t like having anything after app.listen. It feels like it could cause a bug somehow.

Looking at the reducer, the default state type is different than the actual variable type you want, and that can cause problems. Take for example the feelingReducer. Its default state is an empty array. This can cause problems because the state is supposed to be a number. If you call a function that is specific to numbers on feelingReducer at the beginning of the program, this will cause a crash because Array does not have the same functions as Number.

Remember to get into the habit of commenting your code as you go along. I have noticed you have comments in the review page, which I guess would be when you were finishing up the program. But comments are mostly missing from the rest of the code. While the code in this project is pretty straightforward, commenting is a very good habit to have, especially when you move on to more abstract programming. I can tell you from experience what reading my old code that I didn’t comment is like. It can take quite a while before I can even start writing, because I’m trying to figure why I’m doing anything in my code, or even what my code is doing.

Your git commits are pretty solid, though I would not recommend committing half finished code. I like to think of commits as checkpoints that I know for sure work. If any problems arise, or the codebase sets itself on fire, it is easier to rollback to a program I know works by doing it this way.

Overall, solid work. Just need to buff out some edges.
