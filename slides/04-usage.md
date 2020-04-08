# Usage

## Installation

`ng add @scullyio/init`

- Adds Dependency
- Updates the Package.json with some `scripts` commands
- Creates a `scully.{{yourApp}}.config.js` file

## Scaffolding via Schematics

`ng generate @scullyio/init:blog`

- Adds the routes
- creates a `blog` folder

You can use `ng generate @scullyio/init:markdown` for more fine grained naming of things. (eg: news instead of blog)

## Routing

Generate a Routing module. (currently not done by Angular CLI):

`ng generate module home --route=home --module=app-routing`

Then add the home route:

```javascript
const routes: Routes = [
	// ...
	{
		path: "",
		loadChildren: () => import("./home/home.module").then(m => m.HomeModule)
	}
];
```

## Building

## `isScullyRunning()`

## Rule of Threes
