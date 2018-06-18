# angular-simple-nav-menu

Directives for AngularJS (version 1.x) to ease the creation of the typical navigation menu.

It is composed by 3 directives:

1.  `<nav-menu>`: layer that will appear and disappear.
2.  `<nav-item>`: layer that, when clicked, will make the `<nav-menu>` appear and disappear. Use it when the element must be inside the `<nav-menu>` layer.
3.  `<nav-button>`: layer that, when clicked, will make the `<nav-menu>` appear and disappear. Use it when the element must be outside the `<nav-menu>` layer.

## 1. Installation

#### 1. Import the module from NPM:

~$ `npm install --save angular-simple-nav-menu`

#### 2. Import the module from your AngularJS application

##### 2.1. In your HTML:

...and after having imported the AngularJS (v.1.x):

```html
<script src="node_modules/angular-simple-nav-menu/src/module.simple-nav-menu.js"></script>
<link   href="node_modules/angular-simple-nav-menu/src/module.simple-nav-menu.css" rel="stylesheet" type="text/css" />
```

##### 2.2. In your JavaScript, when you initialize the application:

```js
angular.module("MyApp", ["SimpleNavModule"]);
```

## 2. Usage

This is a self-explanatory example, using the directives as elements:

```html
	<nav-button class="nav-button">Shows/Hides the navigation menu when it is clicked.</nav-button>
	<nav-menu class="nav-menu">
		<h1>Title of the navigation menu</h1>
		<nav-item>Item 1 of the navigation menu. Shows/Hides the navigation menu when it is clicked.</nav-item>
		<nav-item>Item 2 of the navigation menu. Shows/Hides the navigation menu when it is clicked.</nav-item>
		<nav-item>Item 3 of the navigation menu. Shows/Hides the navigation menu when it is clicked.</nav-item>
		<nav-item>Item 4 of the navigation menu. Shows/Hides the navigation menu when it is clicked.</nav-item>
	</nav-menu>
```

You only need to know that:

* The directives can be used as attributes too.

* The width of the **`.nav-menu`** is set to **`250px`** in the css file. Override it from other stylesheet, or directly from the source file if you need to adapt it to other dimensions.

* The only 2 CSS rules applied are: **`.nav-menu--inner--api`** and **`.nav-menu--inner--api.activated`**. The CSS file is less than 10 lines, so you can modify it, but it should not be necessary, except for the `width` of the **`<nav-menu>`**.

## 3. Test

Currently, there are no test for this project.

However, you can open a very simple example if you go to: `test/simple-example.html`

It is important that your browser lets you load files from external CDN and from other (upper) paths for it to work. If so, you will be able to run the example okay.

## 4. Conclusion

Use this library as you like, this is a very simple module that can ease a bit the typical navigation menu for an AngularJS application.
