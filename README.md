# ReactStateDiceExercise
This Exercise practices working with props, defaultProps, state and simple click Event in React.
## Roll Dice
Build an app that lets us roll a pair of dice. 
### *Step 1: Component Structure*
Make two Components: 
- **Rolldice** a parent component (rendered by App) that renders the dice and a button to roll.
- **Die** an individual die that takes props and displays the correct face of the die based on props.
### *Stept 2: Making Dice*
We intall Font Awesome and we have the six images; with fas fa-dice-one through fas fa-dice-six represents dice with differents faces from 1-6.
To intall go to public/index.html and in the `<head>` the font awesome CDN.
### *Step 3: Rolling Dice*
The *RollDice* component shoul have:
- the state for both of the dice
- a roll() method that tolls them to randomly get a new ewsult
Can use *defaultProps* to set an array of six possible faces for each die, then update the state causing the dice re-render to the appropriate values.
Remember that these values will have to be translated into fas fa-dice-one through six for the child component to receive the appropriate class name throught its props.
### *Animation*
The solution displays an animation every time the dice are rolled.
Anew piece of state is necessary to say wheter the dice are currently rolling or not.
This is done by appending a class containgn a CSS animatin, and then removing it after one second
### *Changing Button Text*
The button can also dynamically change its text and become disabled until the animation has completed