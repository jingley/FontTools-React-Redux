# Introduction

This component is designed with Redux and React to add font adjusting buttons to a React app. The component utilizes the selected css font percentage that is saved in the redux store to manipulate the font size on every page during a session.

## Getting Started

### Props
`fontSize` contains the current fontSize percentage. This is provided by `ConnectFontTools` from the redux store.

`fontControllingClass` is the className of the base element you want to control the font of. This is provided as a prop by the developer where the component is declared. Ex. `<FontTools fontControllingClass="App-Body"/>`

### Declaration
The component need only be declared once in a single page React app. This should be done on a template page all the components utilize.
### Styling
Styles can be adjusted in the FontTools.css files to fit the theme of any app.

### Setup with Redux
The buttons dispatch the actions `fontUp` and `fontDown` from `'./actions'` respectively when clicked. In order for the actions to be handled, provide the `fontToolsReducer` from `'./reducers'` during creation of the redux store.
