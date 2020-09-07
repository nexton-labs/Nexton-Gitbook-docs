# Sass Stylesheet Guide Line

- Generally, we recommend that you don’t reuse the same CSS classes across different components. For example, instead of using a .Button CSS class in `<AcceptButton>` and `<RejectButton>` components, we recommend creating a `<Button>` component with its own .Button styles, that both `<AcceptButton>` and `<RejectButton>` can render (but not inherit).

- Following this rule often makes CSS preprocessors less useful, as features like mixins and nesting are replaced by component composition. You can, however, integrate a CSS preprocessor if you find it valuable.

# Styles Are Scoped

- React projects tend to break down the structure of the DOM into a lot of components, which means you’re going to have a lot of SCSS files. This is ok! It takes a little getting used to, but we have come to really like this approach to managing styles because everything we need for a component is in a single directory. Here is an example of what a button component could look like:

```
App.scss
/components
  /Button
    Button.js
    Button.tests.js
    Button.scss
```

- Additional we can have a global SCSS that define the main properties and varaibles

# SCSS Files Are Small

- Keeping the SCSS files small allows us to read the style rules more easily. A long, multi-nested SCSS can be hard to follow or overwhelming to people who are not as comfortable with dense style rules. Instead, keep it short and simple.

- It also seems that we have had a much higher success rate of removing unused styles with this approach. If you’re finding your style rules too lengthy, consider refactoring the React code.

# Keep it Responsive

- We have been adding the media queries directly to the rule definition. This has made both refactoring and altering an element’s styles simpler, since it allows you to go to one place in the SCSS to modify the rules for all layouts instead of having to traverse a file where the element may be defined multiple times. Doing this can work for both desktop and mobile-first approaches. Below is an example of this pattern, where you can easily see the .div-element-name’s border-radius being increased at each layout size.

```SCSS
.div-element-name{
  background: orange;
  border-radius: 5px;

  @media only screen and (max-width: $large-screen) {
    border-radius: 25px;
  }

  @media only screen and (max-width: $small-screen) {
    border-radius: 50px;
  }

  &:active{}
  &:focus{}
  &:hover{}

}
```

# SASS Use

- Install SASS `npm install node-sass`
- Create a Sass file

```SCSS
//mysass.scss
$myColor: red;

h1 {
  color: $myColor;
}
```

- Import the Sass file the same way as you imported a CSS file.

```JS
import './App.scss';
```

[SASS Detailed Guide Line](https://sass-guidelin.es)
