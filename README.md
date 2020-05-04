# Introduction

This component is designed with Redux and React to add font adjusting buttons to a React app.

## Getting Started

### Props
`fontSize` this prop is passed from `mapStateToProps` in ConnectFontTools, and has the current fontSize percentage to adjust to
`fontControllingClass` this is the className of the base element you want to control the font of. For example: "App-Body".
the component traverses every child of that element and adjusts font's of those that do not have explcitly declared fonts in CSS.

### Styling
Styles can be adjusted in the FontTools.css files to fit the theme of any app.

### Setup with Redux
This assume you use the `fontToolsReducer` and `fontUp`/`fontDown` actions from the `./actions` and `./reducers` folders when your Redux store.
