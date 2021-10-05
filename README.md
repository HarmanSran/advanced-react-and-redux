Blurb by me (note that some sub directories are based on various online courses - see nested READMEs for citations):

# React and Redux Snippets
Various exercises and snippets with React v16+ and Redux v4+

## When to use Redux
Redux is often **not** immediately necessary in a UI built with React, and is often overused (use state and context hooks first).

However, Redux is one (of many) solutions to simplify state management in particular scenarios, e.g.:
* Manage data from REST API endpoints (e.g. async loading, caching, and separating fetching and view layers) - similar to functionalities provided by Apollo’s GQL libraries
* Manage state that is expected to be readily visible to **all** components of the React Tree rooted at the Redux Provider (e.g. theme data, user profile, modal states)

[@reduxjs/toolkit](https://www.npmjs.com/package/@reduxjs/toolkit) helps reduce boilerplate notorious in applications using Redux.

React’s OOTB state and context should still be used where it makes more sense to keep the state scoped non-globally (generally, moving state to Redux by default is a bad idea).
