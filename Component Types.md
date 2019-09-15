# Component Types

While all components are Vue Components, we should try to break down components into specific types. This helps keep components to being "single responsibility" and helps keep components easy to reuse and reason about.

## Types
- Presentational
  - Element
  - Layout
- Container
  - Service
  - Feature
- Views


## Presentational
Presentational Components are components whose responsibility are to display the item you are trying to create.

They are responsible for:
**Markup** - The HTML that gets shown.
**Styling** - The CSS/Stylus for displaying the forms
**Event Handling/UI State Management** - Managing Basic State such as Toggle, Hover, Click, etc.

When you are organizing a Component Library you should try to maximize reusability. To do this, we can break down presentational components into further subgroups.

- Elements
- Layouts

### Elements
Elements are small pieces of the UI that you can reuse everywhere in the app. 

**Basic Elements**
- Button
- Title
- Progress Spinner
- Icon

**More Sophisticated Elements**
Elements are composable so you can make more complex elements, but the idea is to have them as reusable as possible.

Eg. "Card" Element could be made up of an:
- Image Element
- Button Element
- Box Element
- Title Element


### Layout Components
Layout Elements are one strategy of structuring your components. Layout Components are, as their name suggests, just for laying out content.

While Layouts can be achieved with simple CSS class names, if you want better encapsulation/want to stop css leaking into your layouts through global classes, using scoped styling within a component can work better.

Examples of Different Layouts might be:

- Columns
- Grid
- Masonry (Pinterest Like)

### Location
:::
src/
└─ components/
	└─ General
:::


## Todo...

- How to design Elements
- How to design Layouts
- How to design Features