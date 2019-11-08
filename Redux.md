<h1 align="center">Redux</h1>
<p align="center">
    <img width="200px" src=https://raw.githubusercontent.com/AndresMWeber/WebDefinitions/master/media/Redux.png>
</p>

# Contents
[`Redux Workflow`](#redux-workflow)

[`React-Redux`](#react-redux)

[`Rules of Reducers`](#rules-of-reducers)

## Redux Workflow
  * **Action Creator** - Changes the state of the app: produces an object.
  * **Action** - The action object that will run after action has been created from template Action Creator.
  * **Dispatch** - Receives any action and feeds to reducers.
  * **Reducers** - Process forms/data that comes in, modify and return processed data
  * **State** - Receives reducer data that gets added to a state object which waits until new actions to update next.
  
<p align="center">
    <img src=https://raw.githubusercontent.com/AndresMWeber/WebDefinitions/master/media/10_ReduxCycle.png>
</p>

[`^ Back to Top`](#contents)

## React-Redux
  * **Provider** - takes in the redux store/state as a prop at the top level around the App.
  * **Connect** - registers action creators and hooks them up with the Provider at the top level via the context system to allow the actions to affect the state.  Connect also is able to hook up Components with the prodiver’s redux state and also remap any redux state values to different prop names.

**Async/Sync Action Creators** - disallowed in redux actions: this is due to post-transpilation code returning a request object, not the plain object we are expecting.  You need middleware!

**Redux Thunk** - Middleware solution for asynchronous action creators to allow pausing of actions (enforcing synchronicity) between dispatch/reducer cycle and remove race conditions.

<p align="center">
    <img src=https://raw.githubusercontent.com/AndresMWeber/WebDefinitions/master/media/105_ReduxActions.png>
</p>

[`^ Back to Top`](#contents)

## Rules of Reducers

  1. Must return any value besides ‘undefined’
  2. Produces ‘state’, or data to be used inside of your app using only previous state and the action (reducers are pure) (NO API REQUESTS, USER INPUT OR DOM QUERYING etc)
  3. Must not reach ‘out of itself’ to decide what value to return
  4. Must not mutate its input ‘state’ argument
   
<p align="center">
    <img src=https://raw.githubusercontent.com/AndresMWeber/WebDefinitions/master/media/11_StateRules.png>
</p>

[`^ Back to Top`](#contents)