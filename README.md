
# React-Redux




## FAQ

#### Why Redux is needed ??

-> When you have large application with lost of components interdependent upon each other, then in such case maintaining state for each components is very difficult. Also If you want to shift the components the you Also have to change the state of that components and other components related to it. So using React-Redux makes this job very easy. Basically it solve the props drilling.

#### How does Redux solve this problem??

-> Using redux we dont store the state in components rather than we store the state in the container called **Redux Store**. Components makes a subscription to the change with the Redux so that even if the other components make the changes to the state if can easy be handled by other components.

#### Redux Architecture  ??

![image](https://github.com/jemmyasjd/React_Redux/assets/118959810/b163d3d4-4b26-4abb-aa03-0043d7ad85eb)

-> Whenever we make changes to the UI it goes to the it make call to the event dispatcher which in return create the action and send it to the redux store. Redux store update the value with the current value and then send the updated value to all the components that has subscribed for the change.



## Commands and Methods: 


-> **createStore from redux lib** : use to create the redux store.

-> **Provider from react-redux lib** : Act as a provider for the app which use the store as props

-> **reducer** : it is function that act as a reducer which has two parameter : state and action

-> **useDispatch from react-redux lib** : act as a event dispatcher for the actions.

-> **useSelector from react-redux lib**: use to select the value from the redux store.

however this all methods are just for the basic information about how the redux architecture work in actuall. But in practical we use the Redux toolkit which makes our work easy and simpler.


-------------------------------------------------------------------

Redux toolkit Methods: 

-> **configureStore**: use to create the redux store using redux toolkit.

-> **createSlice** : In redux toolkit we make the reducer using the concept of sicer. this method is used to create the slice. Which take name,initital state and reducer as a object parameter. In reducer we make the methods which take state and action as a input to change the state based on the action. 

-> **createSelector** : use to create the selector for easy convinence 

-> **useDispatch** : in redux toolkit we dont need to mention explicitely we just directly pass action from the slice as a parameter.

-> **useSelector from react-redux lib**: use to select the value from the redux store.

-> **action.payload** : it contains change what we had done through dispatcher.

