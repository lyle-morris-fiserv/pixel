# Size and spacing

The sizing tokens help you control the proportions of your system’s components at the atom level for global consistency. There can impact height, weight, padding, and margin. Depending on the components defined in your initial system, the maturity of this template can include any additional components or attributes in the future.

The tokens should function as a common language during the product cycle. It is critical that the naming convention should be agreed upon between both development and design. Some tokens values can remain empty, using the token as a placeholder for other themes.

>[!Note]
> If you are looking for tokens related to component colors, please reference the [color guidelines](color.md) for the Pixel design system.

## Component specifications

### Base models

| Token name                      | Light theme           | Dark theme            |
| :------------------------------ | :-------------------- | :-------------------- |
| `$base_small`                   | 32px                  | 32px                  |
| `$base_medium `                 | 40px                  | 40px                  |
| `$base_large`                   | 48px                  | 48px                  |
| `$base_padding`                 | `$spacing_16`         | `$spacing_16`         |
| `$base_margin`                  | `$spacing_8`          | `$spacing_8`          |
| `$base_border`                  | `$border_1`           | `$border_1`           |
| `$base_border_radius`           | 4px                   | 4px                   |

### [Accordion](./components/accordion.md)

| Token name                      | Light theme           | Dark theme            |
| :------------------------------ | :-------------------- | :-------------------- |
| `$accordion_small`              | (min-height:40px)     | (min-height:40px)     |
| `$accordion_medium `            | (min-height:48px)     | (min-height:48px)     |
| `$accordion_large`              | (min-height:56px)     | (min-height:56px)     |
| `$accordion_padding`            | `$base_padding`       | `$base_padding`       |
| `$accordion_margin`             | `$base_margin`        | `$base_margin`        |
| `$accordion_border`             | `$base_border`        | `$base_border`        |
| `$accordion_border_radius`      |                       |                       |

### [Avatar](components/avatar.md)

| Token name                      | Light theme           | Dark theme            |
| :------------------------------ | :-------------------- | :-------------------- |
| `$avatar_x_small`               | 28px                  | 28px                  |
| `$avatar_small `                | 38px                  | 38px                  |
| `$avatar_medium`                | 48px                  | 48px                  |
| `$avatar_large`                 | 58px                  | 58px                  |
| `$avatar_x_large`               | 68px                  | 68px                  |
| `$avatar_xx_large`              | 88px                  | 88px                  |
| `$avatar_padding`               |                       |                       |
| `$avatar_margin`                |                       |                       |
| `$avatar_border`                | `$border_2`           | `$border_2`           |
| `$avatar_border_radius`         | 100px                 | 100px                 |

### [Badge](components/badge.md)

| Token name                      | Light theme           | Dark theme            |
| :------------------------------ | :-------------------- | :-------------------- |
| `$badge_small `                 | 12px                  | 12px                  |
| `$badge_medium`                 | 18px                  | 18px                  |
| `$badge_large`                  | 28px                  | 28px                  |
| `$badge_padding`                |                       |                       |
| `$badge_margin`                 |                       |                       |
| `$badge_border`                 | `$border_1`           | `$border_1`           |
| `$badge_border_radius`          | 50px                  | 50px                  |

### [Bottom Navigation](components/bottom_navigation.md)

| Token name                      | Light theme           | Dark theme            |
| :------------------------------ | :-------------------- | :-------------------- |
| `$bottom_nav_small `            |                       |                       |
| `$bottom_nav_medium`            |                       |                       |
| `$bottom_nav_large`             |                       |                       |
| `$bottom_nav_padding`           | `$spacing_8`          | `$spacing_8`          |
| `$bottom_nav_margin`            | `$spacing_4`          | `$spacing_4`          |
| `$bottom_nav_border`            | `$border_1`           | `$border_1`           |
| `$bottom_nav_border_radius`     | 10px                  | 10px                  |

### [Breadcrumb](components/breadcrumb.md)

| Token name                      | Light theme           | Dark theme            |
| :------------------------------ | :-------------------- | :-------------------- |
| `$breadcrumb_small `            |                       |                       |
| `$breadcrumb_medium`            |                       |                       |
| `$breadcrumb_large`             |                       |                       |
| `$breadcrumb_padding`           | `$base_padding`       | `$base_padding`       |
| `$breadcrumb_margin`            | `$based_margin`       | `$base_margin`        |
| `$breadcrumb_border`            | `$border_1`           | `$border_1`           |
| `$breadcrumb_border_radius`     |                       |                       |

### [Button](components/button.md)

| Token name                      | Light theme           | Dark theme            |
| :------------------------------ | :-------------------- | :-------------------- |
| `$button_small `                | `$base_small`         | `$base_small`         |
| `$button_medium`                | `$base_medium`        | `$base_medium`        |
| `$button_large`                 | `$base_large`         | `$base_large`         |
| `$button_padding`               | `$base_padding`       | `$base_padding`       |
| `$button_margin`                | `$base_margin`        | `$base_margin`        |
| `$button_border`                | `$base_border`        | `$base_border`        |
| `$button_border_radius`         | `$base_border_radius` | `$base_border_radius` |








