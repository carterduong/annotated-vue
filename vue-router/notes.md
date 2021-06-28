# intuition 

vue router bridges the create/destroy lifecycle hooks of Vue components, with the browser's URL controls

<router-view> renders a component based on the current URL

# typescript
https://basarat.gitbook.io/typescript/

- superset of js -> valid js is valid ts
- implicit or explicit typing
- enforce the shape of an object with an interface
- ? indicates optional variable

# types

## RouterOptions
- where the user's router config touches vue-router?
- an array of RouteConfigs
- RouterMode can only be one of 3 strings: `'hash' | 'history' | 'abstract'`

## RouteConfig
- can be RouteConfigSingleView or RouteConfigMultipleViews, 
- RouteConfigSingleView and RouteConfigMultipleViews extend _RouteConfigBase
- _RouteConfig's only required var is `path: string`
- what's the diff between RouteConfigSingleView and RouteConfigMultipleViews?
	- RouteConfigMultipleViews accepts only Dictionaries of components/props

# index.js
- contains the call to installation, Router member and static vars, and API surface area

constructor() 
- given RouterOptions, init members 

