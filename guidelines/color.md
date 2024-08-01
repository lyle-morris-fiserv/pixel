# Color

The default themes are derived from the design system's color palette. The slate blue family is dominant in the default themes, making use of subtle shifts in value to organize content into distinct zones. The core blue family serves as the primary action color across all Fiserv products and experiences. Additional colors are used sparingly and purposefully.

Colors in the neutral gray palette are layered on top of each other to create depth and spatial associations. The layering model defines the logic of how colors stack on top of each other in a UI when using the Pixel theming capabilities. Aspects of the layering model are built directly into the themes, color tokens, and components.

The layering model differs between the light and dark themes.

- In the light themes, layers alternate between $white and $slate_50 with each added layer.
- In the dark themes, layers become one step lighter with each added layer.

## Implementing color

This Pixel uses tokens and themes to manage color. Tokens are role-based, and themes specify the color values that serve those roles in the UI.

| Term | Definition |
|:---|:---|
| Theme | A theme is a collection of colors designed to create a specific aesthetic. Themes control the color value assigned to a token.|
| Token | A token is the role-based identifier that assigns a color. Unlike hex codes, tokens apply universally across themes. For example, $layer_1, $border_subtle, $support_error.|
| Role | A role is the systematic usage of a color assigned to a token. Roles cannot be changed between themes.|
| Value | A value is the unique visual attribute (hex code, rgba value) assigned to a token through the use of themes.

