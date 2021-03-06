<!--docs:
title: "Line Ripple"
layout: detail
section: components
excerpt: "The line ripple is used to highight user specified text above it."
path: /catalog/input-controls/line-ripple/
-->

# Line Ripple

The line ripple is used to highlight user specified text above it. When a the line ripple is active, the line’s color and thickness vary.

## Design & API Documentation

<ul class="icon-list">
  <li class="icon-list-item icon-list-item--spec">
    <a href="https://material.io/guidelines/components/text-fields.html#text-fields-layout">Material Design guidelines: Text Fields Layout</a>
  </li>
</ul>

## Usage

### HTML Structure

```html
<div class="mdc-line-ripple"></div>
```

### Usage within `mdc-text-field`

```html
<div class="mdc-text-field">
  <input type="text" id="my-text-field-id" class="mdc-text-field__input">
  <label class="mdc-text-field__label" for="my-text-field-id">Hint text</label>
  <div class="mdc-line-ripple"></div>
</div>
```

### CSS Classes

CSS Class | Description
--- | ---
`mdc-line-ripple` | Mandatory
`mdc-line-ripple--active` | Styles the line ripple as an active line ripple
`mdc-line-ripple--deactivating` | Styles the line ripple as a deactivating line ripple. 

### Sass Mixins

### `MDCLineRipple`

`activate() => void` | Proxies to the foundations `activate()` method.
`deactivate() => void` |  Proxies to the foundations `deactivate()` method.
`setRippleCenter(number: xCoordinate) => void` | Proxies to the foundations `setRippleCenter(number: xCoordinate)` method.

### `MDCLineRippleAdapter`

Method Signature | Description
--- | ---
`addClass(className: string) => void` | Adds a class to the root element
`removeClass(className: string) => void` | Removes a class from the root element
`setAttr(attr: string, value: string) => void` | Sets an attribute with a given value on the root element
`registerEventHandler(evtType: string, handler: EventListener) => void` | Registers an event listener on the root element for a given event
`deregisterEventHandler(handler: EventListener) => void` | Deregisters an event listener on the root element for a given event

### `MDCLineRippleFoundation`

Method Signature | Description
--- | ---
`activate() => void` | Activates the line ripple
`deactivate() => void` |  Deactivates the line ripple
`setRippleCenter(number: xCoordinate) => void` | Sets the center of the ripple to the `xCoordinate` given.
`handleTransitionEnd(evt: Event) => void` | Handles a transition end event
