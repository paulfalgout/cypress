---
title: siblings
comments: false
---

Get sibling DOM elements.

# Syntax

```javascript
.siblings()
.siblings(selector)
.siblings(options)
.siblings(selector, options)
```

## Usage

`.siblings()` requires being chained off another cy command that *yields* a DOM element or DOM elements.

**{% fa fa-check-circle green %} Valid Usage**

```javascript
cy.get('td').siblings()           // Yield all td's siblings
cy.get('li').siblings('.active')  // Yield all li's siblings with class '.active'
```

**{% fa fa-exclamation-triangle red %} Invalid Usage**

```javascript
cy.siblings('.error')     // Errors, cannot be chained off 'cy'
cy.location().siblings()  // Errors, 'location' does not yield DOM element
```

## Arguments

**{% fa fa-angle-right %} selector**  ***(String selector)***

A selector used to filter matching DOM elements.

**{% fa fa-angle-right %} options**  ***(Object)***

Pass in an options object to change the default behavior of `.siblings()`.

Option | Default | Notes
--- | --- | ---
`log` | `true` | Whether to display command in Command Log
`timeout` | {% url `defaultCommandTimeout` configuration#Timeouts %} | Total time to retry getting the element

## Yields

`.siblings()` yields the new DOM elements found by the command.

## Timeout

`.siblings()` will continue to look for the sibling element(s) for the duration of the {% url `defaultCommandTimeout` configuration#Timeouts %}.

# Examples

## Siblings

**Get the siblings of each li**

```html
<ul>
  <li>Home</li>
  <li>Contact</li>
  <li class="active">Services</li>
  <li>Price</li>
</ul>
```

```javascript
// yields all other li's in list
cy.get('.active').siblings()
```

## Selector

**Get siblings of element with class `active`**

```javascript
// yields <li class="active">Services</li>
cy.get('li').siblings('.active')
```

# Command Log

**Get the siblings of element with class `active`**

```javascript
cy.get('.left-nav').find('li.active').siblings()
```

The commands above will display in the command log as:

![Command Log](/img/api/siblings/find-siblings-of-dom-elements-to-test.png)

When clicking on `siblings` within the command log, the console outputs the following:

![Console Log](/img/api/siblings/console-log-of-sibling-elements.png)

# See also

- {% url `.prev()` prev %}
- {% url `.next()` next %}