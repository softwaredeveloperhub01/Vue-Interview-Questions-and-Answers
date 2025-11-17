# Vue Interview Questions and Answers

> Vue Interviews – Top Questions &amp; Answers for Web Developers

---

# ## **1. What is Vue.js?**

Vue.js is a progressive JavaScript framework used to build user interfaces. It focuses on the **view layer**, allowing you to start small and scale into full applications using tools like **Vue Router** and **Vuex/Pinia**.

---

## **2. What makes Vue different from React or Angular?**

* **Vue is easier to learn** (HTML + JS + CSS).
* **Lightweight** runtime.
* Uses **two-way binding** like Angular and **component-based UI** like React.
* More flexible with API choices (Options API & Composition API).

---

## **3. What is the Virtual DOM in Vue?**

The Virtual DOM is a lightweight JS representation of the real DOM. Vue updates only **changed nodes**, making rendering faster and more efficient.

---

## **4. What is the main difference between Vue 2 and Vue 3?**

Vue 3 introduced:

* **Composition API**
* Better performance
* Tree-shaking
* Fragments & Teleport
* Proxy-based reactivity (faster and more accurate)

---

## **5. What is the Composition API?**

A new way in Vue 3 to organize logic using **setup()** and reusable functions. It helps create cleaner, more scalable components.

---

## **6. What is the Options API?**

The traditional Vue API using options like `data()`, `methods`, `computed`, and `watch`.

---

## **7. When should you use Composition API over Options API?**

Use Composition API when:

* You have large components
* Complex logic needs to be organized
* Logic must be reused across components

---

## **8. What is a Vue component?**

A reusable UI block defined using HTML, CSS, and JavaScript.

---

## **9. What are Single File Components (SFCs)?**

Files with `.vue` extension containing:

* `<template>`
* `<script>`
* `<style>`

They keep component logic clean and modular.

---

## **10. What is `v-bind` used for?**

It binds dynamic data to attributes.
Example:

```html
<img v-bind:src="imageUrl" />
```

---

## **11. What shorthand is used for `v-bind`?**

The colon `:`

```html
<img :src="imageUrl" />
```

---

## **12. What does `v-model` do?**

Creates **two-way data binding**, commonly used with inputs.

---

## **13. What lifecycle hooks exist in Vue 3?**

Options API:

* beforeCreate
* created
* beforeMount
* mounted
* beforeUpdate
* updated
* beforeUnmount
* unmounted

Composition API:

* onMounted
* onUpdated
* onUnmounted
* onBeforeMount
* onBeforeUpdate
  … and more.

---

## **14. What is a computed property?**

A cached value based on reactive data.

---

## **15. What is a watcher?**

A watcher runs code when a specific data property changes. Useful for API calls or expensive operations.

---

## **16. What is Vue Router?**

Vue’s official routing library for building single-page applications.

---

## **17. What are dynamic routes?**

Routes with parameters:

```
/users/:id
```

---

## **18. What is a route guard?**

Functions that check access before entering a route—useful for authentication.

---

## **19. What is Vuex?**

A state management library for Vue 2 & Vue 3 following the Flux pattern.

---

## **20. What is Pinia?**

Pinia is the new recommended state management library for Vue 3—lighter, simpler, and more modular than Vuex.

---

## **21. Why was Pinia introduced?**

To offer:

* TypeScript support
* Modular stores
* Better DevTools
* Simpler usage

---

## **22. What is a reactive variable in Vue 3?**

Using `ref()` or `reactive()` for reactivity.
Example:

```js
const count = ref(0);
```

---

## **23. Difference between `ref` and `reactive`?**

* `ref` → single value
* `reactive` → objects/arrays

---

## **24. What is a template in Vue?**

HTML containing interpolations and directives to render dynamic content.

---

## **25. What is a directive in Vue?**

Special HTML markers starting with `v-` like:

* `v-if`
* `v-for`
* `v-model`

---

## **26. What does `v-if` do?**

Conditionally renders or removes elements from the DOM.

---

## **27. Difference between `v-if` and `v-show`?**

* `v-if` removes/adds elements.
* `v-show` toggles CSS `display`.

---

## **28. What is `v-for` used for?**

To loop through arrays or objects.

---

## **29. Why is a `key` important in `v-for`?**

It helps Vue track DOM elements efficiently.

---

## **30. What is a slot?**

Slot is a content placeholder allowing components to accept external HTML.

---

## **31. What are named slots?**

Slots with custom names:

```html
<slot name="header"></slot>
```

---

## **32. What is scoped slot?**

Slots that receive data from the child component.

---

## **33. What is Teleport in Vue 3?**

A feature to render part of a component in another part of the DOM (e.g., modal root).

---

## **34. What are fragments in Vue 3?**

Components that return multiple root elements.

---

## **35. What is the purpose of `setup()`?**

Entry point for Composition API logic.

---

## **36. What are composables?**

Reusable logic functions like:

```
useFetch()
useAuth()
```

---

## **37. What is the reactivity caveat fixed in Vue 3?**

Vue 2 could not detect:

* new object keys
* array index changes
  Vue 3 fixed this using proxies.

---

## **38. How do you make API calls in Vue?**

Using `fetch`, `axios`, or inside hooks like `onMounted()`.

---

## **39. What is a mutation in Vuex?**

A synchronous way to modify state.

---

## **40. What is an action in Vuex?**

Handles async logic before committing mutations.

---

## **41. What is a getter in Vuex?**

Computed values for the store.

---

## **42. What is a store in Pinia?**

A modular state container created using `defineStore`.

---

## **43. Difference between Vuex and Pinia?**

Pinia is:

* Simpler
* No mutations
* Fully TS ready
* DevTools friendly

---

## **44. How do you optimize performance in Vue?**

* use computed
* memoize heavy values
* lazy-loading routes
* avoid unnecessary watchers
* use `v-once` for static content

---

## **45. What is `v-on`?**

Used to attach event listeners.
Shorthand: `@`

---

## **46. What is `$refs`?**

A way to access DOM elements directly.

---

## **47. What is a mixin?**

Old reuse pattern before Composition API.
Avoid in Vue 3—use composables instead.

---

## **48. What is a plugin in Vue?**

Globally adds functionality like UI libraries or custom services.

---

## **49. What is tree-shaking?**

Vue 3 removes unused code during build for smaller bundles.

---

## **50. What is hydration in Vue SSR?**

Matching client JS to server-rendered HTML.

---

## **51. What is Nuxt.js?**

A framework built on Vue for SSR, routing, and full-stack applications.

---

## **52. What is a watcher effect?**

Automatically tracks reactive dependencies inside `watchEffect()`.

---

## **53. What is `watchEffect()`?**

Runs logic whenever its dependencies change—no need to specify values.

---

## **54. What is `defineProps` in Vue 3?**

Used inside `<script setup>` to declare props.

---

## **55. What is `defineEmits`?**

Defines custom events for parent-child communication.

---

## **56. What is a shallowRef()?**

Reactive reference but tracks only the top-level value.

---

## **57. What is suspense in Vue?**

Allows async components with fallback loading UI.

---

## **58. What is `toRefs()`?**

Converts a reactive object’s properties into individual refs.

---

## **59. What is `provide/inject`?**

Way to share data deeply across component trees.

---

## **60. What is the difference between props and state?**

* Props → passed from parent
* State → owned by component/store

---

## **61. What is a global component?**

A component registered once and used anywhere.

---

## **62. What is a local component?**

Registered inside another component.

---

## **63. How do you emit an event?**

```js
emit("submit", data)
```

---

## **64. Difference between `$emit` and a callback function?**

`$emit` triggers events; callbacks pass functions as props.

---

## **65. When is `v-once` useful?**

For static content that never changes.

---

## **66. What is `v-cloak`?**

Prevents flash of uncompiled template.

---

## **67. What is lazy loading in Vue?**

Load components or routes only when needed.

---

## **68. What is code splitting?**

Breaking the bundle into smaller chunks for faster loading.

---

## **69. What is `is` attribute used for?**

Dynamic component rendering.

---

## **70. What is `keep-alive`?**

Caches component state when switching between views.

---

## **71. When do you use `<transition>`?**

For adding animations to elements entering or leaving the DOM.

---

## **72. What is `<transition-group>`?**

For list animations.

---

## **73. What is `$nextTick`?**

Executes code after DOM updates.

---

## **74. What is the runtime-only build?**

Vue without template compiler—used with precompiled templates.

---

## **75. What is the runtime+compiler build?**

Includes template compiler for in-browser template building.

---

## **76. What is deep watching?**

Watching nested objects using:

```js
deep: true
```

---

## **77. What is a reactive dependency?**

A value that triggers updates when changed.

---

## **78. What is the main purpose of the `key` attribute?**

Helps Vue efficiently update DOM elements in lists.

---

## **79. What is a higher-order component (HOC)?**

A component pattern that returns another component.

---

## **80. Why avoid mutating props directly?**

It violates one-way data flow.

---

## **81. How can you prevent prop mutation?**

Use computed setter or local data copies.

---

## **82. What is the difference between `async setup()` and normal setup?**

`async setup()` lets you await API calls before rendering.

---

## **83. What is an async component?**

A component loaded with dynamic import.

---

## **84. What is Virtual Scrolling?**

Render only visible DOM elements for huge lists.

---

## **85. How do you debug Vue applications?**

Using Vue DevTools extension.

---

## **86. What is a render function?**

A JavaScript function that returns VNodes instead of templates.

---

## **87. When to use a render function?**

When dynamic template generation is required.

---

## **88. What is JSX in Vue?**

An alternative to templates using JavaScript XML syntax.

---

## **89. What is `shallowReactive()`?**

Similar to `reactive()` but only tracks the top-level properties.

---

## **90. What is a controlled component?**

A component whose input value is bound using `v-model`.

---

## **91. What is the purpose of `emits` option?**

To define event names and validate payloads.

---

## **92. How do you reuse logic without mixins?**

Using composables.

---

## **93. What is the difference between `slot` and `props`?**

* Props → data passing
* Slots → template passing

---

## **94. What is ESM build of Vue?**

Vue packaged in ES module format.

---

## **95. What is the globalProperties API?**

Adds global variables or functions to Vue application.

---

## **96. What is a watcher cleanup function?**

A return function inside `watch()` to stop listening.

---

## **97. What is a template ref?**

Used to reference DOM elements in Composition API via `ref()`.

---

## **98. When use SSR in Vue?**

For SEO, faster first paint, and content-heavy apps.

---

## **99. What is hydration mismatch?**

When client-side DOM doesn’t match server-rendered DOM.

---

## **100. Why should one choose Vue for modern apps?**

Vue offers:

* Flexibility
* Clean architecture
* Fast performance
* Easy learning curve
* Strong ecosystem
* Long-term stability (Vue 3 foundation)

---