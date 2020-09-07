# SEO Fundamentals

This guide cover the fundamentals of enabling Search Engine Optimization for our projects; mostly using modern tools, but can also be used as a reference, on more unique project requirements.

## Content

- Content needs to be original, and it's best to take advantage of all HTML tags, like H1 for the page title, strong, em, blockquote, etc.
- It's best if HTML with the content is accessible at page load, instead of requiring Javascript. For that we can use a Static Site or Server Side Rendenring.
- We can suggest our clients to create a blog within the app to keep content fresh and recent; this improves the SEO.

## Meta tags

- We should populate the <head> with meta tags that coincide with the content at hand.
- Also add the extra meta tags that are used for Social Sharing like Facebook and Twitter.
- A useful tool in the case of React is [react-helmet](https://github.com/nfl/react-helmet) (and for Gatsby we have [gatsby-plugin-react-helmet](https://www.gatsbyjs.org/packages/gatsby-plugin-react-helmet/))

## Sitemap

- A map with the list of all your site links helps the bots to discover new pages.
- In the case of Gatsby we can use a tool like [gatsby-plugin-sitemap](https://www.gatsbyjs.org/packages/gatsby-plugin-sitemap/) (or [gatsby-plugin-advanced-sitemap](https://www.gatsbyjs.com/plugins/gatsby-plugin-advanced-sitemap/)

## Robots.txt

- Add and fill robots.txt on the project root with a tool like [gatsby-plugin-robots-txt](https://www.gatsbyjs.org/packages/gatsby-plugin-robots-txt/)

## Accessibility

- Enabling accessibility on a website not only provides a better experience for many user, but improves SEO ranking.
- Things to check are the contrast of text, font sizes, links, button, navigation and alt text for images.
- We can audit our website with a tool like [Siteimprove Accessibility Checker](https://chrome.google.com/webstore/detail/siteimprove-accessibility/efcfolpjihicnikpmhnmphjhhpiclljc)

## Audit tools

### Other tools to audit or analize our site are:

- Lighthouse (accessible on the Chrome browser dev tab)
- [Search Console](https://search.google.com/search-console/about)
- [Pingdom](https://tools.pingdom.com/)
- [SEO Checker](https://suite.seotesteronline.com/seo-checker)
