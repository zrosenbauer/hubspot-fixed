# hubspot-fixed

A hacky but efficient way to hide sidebar items in HubSpot and create a half-way decent darkmode.

## How to "fix" HubSpot

1. Install the [Custom CSS by Dennis](https://chromewebstore.google.com/detail/custom-css-by-denis/cemphncflepgmgfhcdegkbkekifodacd) chrome extension
2. Add the CSS using the chrome extension (comment out or remove the IDs you want to keep)
```css
#marketing-toggle,
#workspaces-toggle,
#commerce-branch-v5-toggle,
#automation-toggle,
#web-content-toggle,
#sales-reports-list,
#forecasting,
#service-reports-list { 
  display: none; 
}

a:has(#upgradeArrow) {
  display: none;
}
```
3. Profit

## How to add a better darkmode

1. Install the [HubSpot Dark AF](https://chromewebstore.google.com/detail/hubspot-dark-af/kijodgofeoecfagdajkeeopenhiobghj) chrome extension
2. Add the following CSS using the chrome extension to fix certain issues
```css
/* Fix the nav icons */
#hs-vertical-nav-root button svg,
#hs-vertical-nav-root a svg {
  stroke: #000;
}
```
3. Profit
