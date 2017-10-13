## Lab Exercises

#### Part 1: Redux 

*  [Step 1: Redux Emulation](step-1-redux-emulator.md)
*  [Step 2: Using the Redux Library](step-2-use-createStore.md)
*  [Step 3: Using Action Creators](step-3-use-action-creators.md)
*  [Step 4: Using Middleware](step-4-use-middleware.md)
*  [Step 5: Using Thunks for Async Actions](step-5-thunks-for-async-voting.md)

#### Part 2: **ngrx**

*  [Step 1: Using **ngrx**](https://github.com/thoughtram/angular-master-class-exercise-descriptions/blob/master/exercises/ngrx/step-1-use-ngrx.md)
*  [Step 2: Select and Edit Actions](https://github.com/thoughtram/angular-master-class-exercise-descriptions/blob/master/exercises/ngrx/step-2-select-and-edit.md)
*  [Step 3: Use Router Guard with Actions](https://github.com/thoughtram/angular-master-class-exercise-descriptions/blob/master/exercises/ngrx/step-3-create-contact-exists-guard.md)
*  [Step 4: Refactor Query Selectors](https://github.com/thoughtram/angular-master-class-exercise-descriptions/blob/master/exercises/ngrx/step-4-extract-selectors-and-use-reselect.md)
*  [Step 5: Apply Middleware](https://github.com/thoughtram/angular-master-class-exercise-descriptions/blob/master/exercises/ngrx/step-5-apply-middleware.md)
*  [Step 6: Using Effects for Async Actions](https://github.com/thoughtram/angular-master-class-exercise-descriptions/blob/master/exercises/ngrx/step-6-async-with-effects.md)
*  [Step 7: Refactor to Facade Architecture](https://github.com/thoughtram/angular-master-class-exercise-descriptions/blob/master/exercises/ngrx/step-7-reactor-to-facade-architecture.md)

----

Redux promotes a simple one-way data flow for applications; where views dispatch actions, 
stores process actions using reducers and then notify view listeners when the store state has changed.

For our application, we can see below how: 

*  the View is composed of nested components.
*  the **StatusComponent** view on subscribes/watches the **Store** for vote changes
*  the **VoterComponent** view dispatches actions to the **Store**.

<br/>&nbsp;

![redux_voter_flow](https://cloud.githubusercontent.com/assets/210413/25229730/0acdd494-2597-11e7-8852-91f3527ac2f9.jpg)

<br/>&nbsp;

## Scenario

To explore the concepts of the Redux patterns, let's use the following Angular application where visitors can vote to support the Tea Tax Act passed in 1773 by Parliment, England.


![VoterApplication](https://cloud.githubusercontent.com/assets/210413/25202424/fbc0e10c-251a-11e7-8247-485e70a2a059.jpg)

Let's use the Redux API to build an simple Voting application using stores, reducers, dispatched actions, and middleware. 

<br/>&nbsp;

