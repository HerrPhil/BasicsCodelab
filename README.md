# BasicsCodelab

- the Surface composable can be used anywhere to configure UI/UX for composables.
- (eg) set background color of a Text composable
- Material 2/3 is an opinionated framework; it will do work on your behalf if it makes sense.
    - Surface will pick a font color for content to complement a background; if background is dark, then color for content is light
- from the inter tubes:

"Use the Surface composable in Android Jetpack Compose when you need a container for your content that applies Material Design styles,
such as elevation, shape, border, and background color, while ensuring proper content color and theme integration.
It is particularly useful as a root layout for components, providing a consistent and semantically clear way to represent a material surface,
Which is the central metaphor in Material Design."

"Surface simplifies the code compared to manually applying modifiers like
background, border, shadow, and clip, as it handles these aspects internally and
automatically adjusts colours for elevation, especially in dark themes. It also
respects the light/dark theme modes of your app, automatically adapting its
appearance. For example, it is commonly used to wrap content like Text or
Column to create styled containers with rounded corners, shadows, and borders."

Surface can only hold one direct child. Combine with Box to achieve more complex layouts.

For @Preview compostables, it is possible to have more than one @Preview annotation per preview @Composable function.

For example, show the light/dark previews of one composable function.

For very long lists that populate a Column, use LazyColumn; LazyColumn only composes what is visible in the viewport.

To test re-composition state, switch from light to dark mode. Similar to what happens if the app's configuration changes, like from portrait to landscape.
