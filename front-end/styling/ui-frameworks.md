# UI Frameworks

## Benefits of Using a Front-end UI Framework

Using a Front-end Framework has a lot of benefits.

* They provide a solid foundation for responsive design.
* Components of the UI have a base style to be extended \(forms, buttons, menus, etc.\).
* The base styles persist throughout.
* They provide a consistent UI design for developers.
* Good looking UI, even out-of-the-box.
* Components of the UI have a base style to be extended \(forms, buttons, menus, etc.\)
* The base styles persist throughout.
* Code is reliable and tested.
* Cross-browser compatibility is built-in, so you know where it will work.

## Material UI Framework

* Material UI is added in our [**Starter React Proyect V2**](https://github.com/nexton-labs/react-starter-v2) for all the new projects that we create at Nexton.
* Material Design is a design language that was first introduced by Google in 2014. It’s a visual language that makes use of grid-based layouts, responsive animations and transitions, padding, and depth effects such as lighting and shadows.
* The goal for Material Design is down to three things: Create, Unify and Customize.
* With Create, Material Design aims to provide a visual language that synthesizes the classic principles of good design.
* With Unify, it aims to develop a single underlying system that unifies the user experience across platforms, devices, and input methods.
* With Customize, it provides a visual language and a flexible foundation for innovation and brand expression.

### CSS Baseline

* If you’ve been writing front-end code, you should already know what aboutnormalize.css. If not, it’s a collection of HTML element and attribute style normalizations. Material-UI provides its own version of normalize.css which is CssBaseline, a component that provides an elegant, consistent, and simple baseline to build upon.
* The CSSBaseline does the following:
  * The margin in all browsers is removed
  * The default Material Design background color is applied
  * Font antialiasing is enabled for better display of the Roboto font
  * No base font-size is declared on the , but 16px is assumed \(browser default\)

### Grid

* Material Design’s responsive UI is based on a 12-column grid layout. This grid creates visual consistency between layouts.
* The grid system features the following:
* It uses Flexbox
* There are two types of layout: containers and items
* Item widths are set in percentages, so they’re always fluid and sized relative to their parent element
* Items have padding to create the spacing between individual items.
* There are five grid breakpoints: xs, sm, md, lg, and xl

[Click here to check detailed documentation](https://material-ui.com/components/grid/)

### Icons

* Icons are a huge part of material design, they are used in buttons to convey an action, to convey information e.t.c. It’s used to symbolize a command, file, device, or directory.
* Icons are also used to represent actions like trash, print, and save, and are commonly found in app bars, toolbars, buttons, and lists.
* Icons in Material-UI can be rendered using two methods; Icon for rendering font icons, and SvgIcon for rendering SVG paths.
* The SvgIcon component takes an SVG path element as its child and converts it to a React component that displays the path, and allows the icon to be styled and respond to mouse events. That can be seen in the example below:
* Material-UI also has a package that ships with preset icons to be used in your React app. It’s a different package entirely, and it includes the official Material icons converted to SvgIcon components.

[Click here to check detailed documentation](https://material-ui.com/components/icons/#icons) [MAterial UI Icons Library](https://material-ui.com/components/material-icons/#material-icons)

### Buttons

Since material-ui components are in isolation, you’ll need to import the Button component.

```jsx
import Button from '@material-ui/core/Button';
<Button color="primary">Hello World</Button>
```

The Button component can take on many props such as color, variant, size e.t.c. You can check out the full list [here](https://material-ui.com/api/button/).

### Material-UI components

* Material-ui has a lot of UI components that helps to build a material design themed React app. Let’s go over some of the material-ui components. Each of the components has an example and you can click on their respective CodeSandbox links to see the code.

#### App bars

-The App bar, formerly known as the action bar in Android, it acts as a header navigation menu. It is a toolbar that’s used for branding, navigation, search, and actions. To use the App bar, these two components are needed from material-ui:

```jsx
import AppBar from '@material-ui/core/AppBar';
import Toolbar from '@material-ui/core/Toolbar';
```

[Click here to check detailed documentation](https://material-ui.com/components/app-bar/)

#### Navigation

* Bottom navigation menus are placed at the bottom and they make it easy to switch between top-level views in a single tap.
* The navigation menu is characterized by three to five actions, each containing an icon and a label. Although it’s important to note that only navigation bars with three actions should contain both an icon and a label.

[Click here to check detailed documentation](https://material-ui.com/components/bottom-navigation/)

#### Tabs

* Tabs make it easy to explore and switch between different views. A tab component can be a simple tab with no additions as seen in the first example below or a scrollable tab with multiple tabs.
* A tab can also just consist of icons as titles/labels.

[Click here to check detailed documentation](https://material-ui.com/components/tabs/)

#### Lists

* Lists present multiple line items vertically as a single continuous element.
* Lists are made up of a continuous column of rows. Each row contains a tile. Primary actions fill the tile, and supplemental actions are represented by icons and text.

[Click here to check detailed documentation](https://material-ui.com/components/tabs/)

#### Cards

* A card is a sheet of material that serves as an entry point to more detailed information.
* Cards are a convenient means of displaying content composed of different elements. Cards are used to display information that can be easily glanced at and usually has a Call To Action.

[Click here to check detailed documentation](https://material-ui.com/components/cards/)

#### Modal

* The modal component provides a solid foundation for creating dialogs, popovers, lightboxes e.t.c
* Whenever a modal button is clicked on, it does the following:
* Manages dialog stacking when one-at-a-time just isn’t enough
* Creates a backdrop, for disabling interaction below the modal
* It properly manages focus; moving to the modal content, and keeping it there until the modal is closed
* It disables scrolling of the page content while open
* Adds the appropriate ARIA roles are automatically

[Click here to check detailed documentation](https://material-ui.com/components/modal/)

#### Grid list

* Grid lists are an alternative to standard list views seen above. A grid list consists of a repeated pattern of cells arrayed in a vertical and horizontal layout and it usually prominently features images.
* An advanced example of a Grid list can be seen below, it features the use of the GridListTileBar to add an overlay to each GridListTile. The overlay can accommodate a title, subtitle and secondary action – in this example an IconButton which could be used to convey more information.

[Click here to check detailed documentation](https://material-ui.com/components/grid-list/)

#### Tables

* Data tables display sets of raw data. They usually appear in desktop enterprise products.
* A data table contains a header row at the top that lists column names, followed by rows for data.
* For accessibility, the first column is set to be a  element, with a scope of "row". This enables screen readers to identify a cell’s value by it’s row and column name.
* An advanced usage of Tables can be seen in the example below. It uses checkboxes, which accompanies each row, if the user needs to select or manipulate data. It also uses clickable rows for selection.

[Click here to check detailed documentation](https://material-ui.com/components/tables/)

## Using Other Frameworks

* Some projects at Nexton may require another frameworks like.
* [Rebass](https://rebassjs.org)
* [Bootstrap](https://getbootstrap.com) - [React Bootstrap](https://react-bootstrap.github.io)

