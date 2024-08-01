# Design Tokens

In the current highly competitive market, businesses strive to employ as many digital channels as possible to promote their products. While this may seem like a rational approach, it can lead to inconsistencies and confusion for customers when a business operates several web platforms. Fortunately, the advent of design systems has made this issue less challenging for both parties.

However, what about the internal aspects of the design and development process? Can a design system alone ensure the effective provision of all involved channels? The answer is no. Although employing a design system is a step in the right direction, it has its own drawbacks that become apparent when designs are transferred to the front end or undergo changes. To avoid such discrepancies, businesses should make use of design system tokens.

Design tokens allow businesses to establish a consistent design language across all digital channels by defining design attributes such as colors, typography, and spacing. This helps ensure that changes made to the design system are reflected across all channels consistently.

## Scalability

Design tokens refer to the style values of user interface (UI) elements, such as color, typography, spacing, and animation, which are necessary for building and maintaining a design system. Unlike hard-coded values, design tokens are dynamic and can be converted to any format, whether for a website, web application, or iOS application.

Each design token is given a name that reflects a specific design decision and its corresponding defined value. For instance, if a brand’s primary color is Magenta #BE3455, the design token could be expressed as 'primary-color = #BE3455', with 'primary-color' representing the name and '#BE3455' representing the value. When breaking down a digital product, one can see a pattern of feature-interface-component-design token, where the design tokens serve as dynamic rather than static values.
 
The dynamic nature of design tokens allows for easy modifications to be made. For example, if the trend shifts, and a brand wishes to change its primary color to Purple #6667AB, it can simply update the design token’s value to #6667AB, and the change will be reflected across all platforms and frameworks where they are utilized.

Overall, the shift towards using design tokens is driven by their dynamic nature, which allows for easy modification and scalability across various platforms and frameworks. This approach makes it easier to maintain a consistent and cohesive design system, particularly for larger projects or those that require frequent updates.

## Design tokens versus variables

It is essential to understand the difference between a regular variable and a design token. A regular variable, such as '$hyper-magenta = #BE3455', is used to structure design options but does not provide any information about how it is meant to be used. On the other hand, a design token, like 'primary.color = #BE3455', clearly indicates that Hyper Magenta is the primary color of the application. In this way, design tokens bridge the gap between naming and design property usage, which regular variables do not.

In addition, they are platform-agnostic, making them more adaptable and flexible regarding scaling design. Instead of storing the value in a CSS file and copying it to every app or website, they are usually kept in a separate file, such as JSON, and can be read into any codebase. This means that they can be used across various platforms, including websites, Android, and iOS applications, seamlessly.

Overall, design tokens provide several benefits over regular variables, including clearer communication of design property usage and more scalability and adaptability across different platforms.

## Benefits

In large-scale design projects, updating a single value can become time-consuming and tedious, especially when there are numerous design components involved. Furthermore, manually adjusting values can lead to errors if a designer overlooks any of them. To address these challenges, design system tokens offer significant benefits that can enhance the design process.

- **Advancing Flexibility and Automation**
Design tokens take the flexibility of reusable design elements to a new level. They enable designers to make changes in one place, and the new values automatically apply to all designs across different platforms, such as websites, apps, and other assets. This flexibility advances automation, making it a significant plus of using design system tokens.

- **Speeding Up the Hand-Off**
Design tokens can speed up the hand-off process from design to development. Since modifying numerous elements requires less effort and less time, designers can save time and focus on creativity. This advantage can be a deciding factor for most professionals since projects often takes time.

- **Simplifying the Development Process**
Integrating design tokens into the design system simplifies the development process. When designers update token files according to targeted platforms, developers can retrieve already updated files and use them in the project. This process eliminates the need for developers to look through their codebase for every instance where a particular value needs changing, making updates quicker and more manageable.

- **Boosting Consistency**
Using design tokens ensures consistency across all platforms. All values are managed from one place and distributed to different environments at once. This approach minimizes the risks of accidental errors during manual changes and provides a way to maintain complete control over the values.

- **Establishing a Single Source of Truth**
Design tokens establish a sole source of truth for design and development teams. This repository of all style choices and changes enables both teams to refer to it when needed, driving better communication and a more streamlined workflow.

In summary, using design system tokens can significantly leverage the design process by advancing flexibility and automation, speeding up the hand-off, simplifying the development process, boosting consistency, and establishing a sole source of truth.

## Using design tokens

Design tokens are a powerful tool for designers and developers to streamline the process of creating and updating digital products. However, before implementing them, it is essential to consider if they are the right fit for your project. In this article, we will discuss when to use design tokens and when they may not be helpful. We will also provide tips for developing and naming tokens, adhering to JSON format, and ensuring accessibility.

1. **Decide if Design Tokens are Right for You**
While design tokens can bring consistency and speed to your design and development processes, it is crucial to consider several points before implementing them. These include updating your product’s design with a design system, covering multiple products or platforms, and streamlining future updates. Conversely, if you do not have a design system or use hard-coded values, design tokens may not be the best option. Carefully considering these factors can save you time and effort overall.

2. **Interface Inventory**
If you decide to use design tokens, the first step is to deconstruct your product into components and categorize them. This inventory should include every element of your interface, from color and typography to spacing and more. This practice will allow you to develop tokens accurately and efficiently.

3. **Define Criteria**
To achieve consistency and efficiency, it is essential to have clear criteria for tokenizing style options. If an option is only used in one place, there may be no need to create a token. Tokenization is most effective when options are spread throughout your product and can be managed from one place. Defining these criteria will help you simplify and streamline your design system.

4. **Naming Conventions**
The effectiveness of design tokens relies on clear naming conventions that accurately reflect their usage. Category/Type/Item (CTI) naming conventions can optimize tokens hierarchically and facilitate more accurate design decisions. However, to use this naming convention, you need to know how to distinguish between global and alias tokens. Global tokens cover all instances of a particular style option, while alias tokens cover more specific uses. Adhering to clear naming conventions will help ensure that your design system is easy to use and maintain.

5. **Adhere to JSON Format**
Using JSON format to encode values can help you adjust design options quickly and easily for multiple preprocessors, including SaaS (Software as a Service). JSON files can also be an efficient asset for data interchange between web applications and servers, making it a smart solution for those who want fast, qualified transmission.

6. **Take Responsibility**
Having someone responsible for token provision is vital to ensuring the accuracy and effectiveness of your design tokens. This person can review, evaluate all suggestions, and curate tokens at all stages of the process. Collaborative decision-making is valuable, but an outside perspective can help make rational decisions.

7. **Accessibility**
Design tokens, like any other aspect of design, should be accessible to all users. Testing tokens for accessibility and conducting regular audits of your design system can help ensure that it meets the latest standards.

In summary, design tokens are a powerful tool for streamlining your design and development processes. Carefully considering their implementation and adhering to best practices will help make sure that your design system is efficient, effective, and accessible to all users.

## Token architecture

### Sizing

The sizing tokens help you control the proportions of your system’s components at the atom level for global consistency. There can impact height, weight, padding, and margin. Depending on the components defined in your initial system, the maturity of this template can include any additional components or attributes in the future.

The tokens should function as a common language during the product cycle. It is critical that the naming convention should be agreed upon between both development and design. Some tokens values can remain empty, using the token as a placeholder for other themes.

#### Base models

Base models are set at a global level of the token architecture. Applying a defined base unit helps make all components consistant in sizing and easier to work together.

| Token name                     | Pixel Light           | Pixel Dark            | Point Light | Point Dark |
| ------------------------------ | --------------------- | --------------------- | ----------- | ---------- |
|'$base_small'                   | 32px                  | 32px                  |             |            |
|'$base_medium'                  | 40px                  | 40px                  |             |            |
|'$base_large'                   | 48px                  | 48px                  |             |            |
|'$base_padding'                 | 16px                  | 16px                  |             |            |
|'$base_margin'                  | 8px                   | 8px                   |             |            |
|'$base_border'                  | 1px                   | 1px                   |             |            |
|'$base_border_radius'           | 4px                   | 4px                   |             |            |

#### Accordion

| Token name                     | Pixel Light           | Pixel Dark            | Point Light | Point Dark |
| ------------------------------ | --------------------- | --------------------- | ----------- | ---------- |
|'$accordion_small'              | (min-height:40px)     | (min-height:40px)     |             |            |
|'$accordion_medium'             | (min-height:48px)     | (min-height:48px)     |             |            |
|'$accordion_large'              | (min-height:56px)     | (min-height:56px)     |             |            |
|'$accordion_padding'            | '$base_padding'       | '$base_padding'       |             |            |
|'$accordion_margin'             | '$base_margin'        | '$base_margin'        |             |            |
|'$accordion_border'             | '$base_border'        | '$base_border'        |             |            |
|'$accordion_border_radius'      |                       |                       |             |            |

#### Avatar

| Token name                     | Pixel Light           | Pixel Dark            | Point Light | Point Dark |
| ------------------------------ | --------------------- | --------------------- | ----------- | ---------- |
|'$avatar_x_small'               | 28px                  | 28px                  |             |            |
|'$avatar_small'                 | 38px                  | 38px                  |             |            |
|'$avatar_medium'                | 48px                  | 48px                  |             |            |
|'$avatar_large'                 | 58px                  | 58px                  |             |            |
|'$avatar_x_large'               | 68px                  | 68px                  |             |            |
|'$avatar_xx_large'              | 88px                  | 88px                  |             |            |
|'$avatar_padding'               |                       |                       |             |            |
|'$avatar_margin'                |                       |                       |             |            |
|'$avatar_border'                | '$border_2'           | '$border_2'           |             |            |
|'$accordion_border_radius'      | 100%                  | 100%                  |             |            |

#### Badge

| Token name                     | Pixel Light           | Pixel Dark            | Point Light | Point Dark |
| ------------------------------ | --------------------- | --------------------- | ----------- | ---------- |
|'$badge_small'                  | 12px                  | 12px                  |             |            |
|'$badge_medium'                 | 18px                  | 18px                  |             |            |
|'$badge_large'                  | 28px                  | 28px                  |             |            |
|'$badge_padding'                |                       |                       |             |            |
|'$badge_margin'                 |                       |                       |             |            |
|'$badge_border'                 | '$border_1'           | '$border_1'           |             |            |
|'$badge_border_radius'          | 50px                  | 50px                  |             |            |

#### Bottom navigation

| Token name                     | Pixel Light           | Pixel Dark            | Point Light | Point Dark |
| ------------------------------ | --------------------- | --------------------- | ----------- | ---------- |
|'$bottom_nav_small'             |                       |                       |             |            |
|'$bottom_nav_medium'            |                       |                       |             |            |
|'$bottom_nav_large'             |                       |                       |             |            |
|'$bottom_nav_padding'           | '$spacing_8'          | '$spacing_8'          |             |            |
|'$botton_nav_margin'            | '$spacing_4'          | '$spacing_4'          |             |            |
|'$botton_nav_border'            | '$border_1'           | '$border_1'           |             |            |
|'$botton_nav_border_radius'     | 10px                  | 10px                  |             |            |

#### Breadcrumb

| Token name                     | Pixel Light           | Pixel Dark            | Point Light | Point Dark |
| ------------------------------ | --------------------- | --------------------- | ----------- | ---------- |
|'$breadcrumb_small'             |                       |                       |             |            |
|'$breadcrumb_medium'            |                       |                       |             |            |
|'$breadcrumb_large'             |                       |                       |             |            |
|'$breadcrumb_padding'           | '$base_padding'       | '$base_padding'       |             |            |
|'$breadcrumb_margin'            | '$base_margin'        | '$base_margin'        |             |            |
|'$breadcrumb_border'            | '$border_1'           | '$border_1'           |             |            |
|'$breadcrumb_border_radius'     |                       |                       |             |            |

#### Button

| Token name                     | Pixel Light           | Pixel Dark            | Point Light | Point Dark |
| ------------------------------ | --------------------- | --------------------- | ----------- | ---------- |
|'$button_small'                 | '$base_small'         | '$base_small'         |             |            |
|'$button_medium'                | '$base_medium'        | '$base_medium'        |             |            |
|'$button_large'                 | '$base_large'         | '$base_large'         |             |            |
|'$button_padding'               | '$base_padding'       | '$base_padding'       |             |            |
|'$button_margin'                | '$base_margin'        | '$base_margin'        |             |            |
|'$button_border'                | '$base_border'        | '$base_border'        |             |            |
|'$button_border_radius'         | '$base_border_radius' | '$base_border_radius' |             |            |

#### Button Group

| Token name                     | Pixel Light           | Pixel Dark            | Point Light | Point Dark |
| ------------------------------ | --------------------- | --------------------- | ----------- | ---------- |
|'$button_group_small'           | '$base_small'         | '$base_small'         |             |            |
|'$button_group_medium'          | '$base_medium'        | '$base_medium'        |             |            |
|'$button_group_large'           | '$base_large'         | '$base_large'         |             |            |
|'$button_group_padding'         | '$base_padding'       | '$base_padding'       |             |            |
|'$button_group_margin'          | '$base_margin'        | '$base_margin'        |             |            |
|'$button_group_border'          | '$base_border'        | '$base_border'        |             |            |
|'$button_group_border_radius'   | '$base_border_radius' | '$base_border_radius' |             |            |

#### Card

| Token name                     | Pixel Light           | Pixel Dark            | Point Light | Point Dark |
| ------------------------------ | --------------------- | --------------------- | ----------- | ---------- |
|'$card_header_small'            | (min-height:40px)     | (min-height:40px)     |             |            |
|'$card_footer_small'            | (min-height:40px)     | (min-height:40px)     |             |            |
|'$card_header_medium'           | (min-height:48px)     | (min-height:48px)     |             |            |
|'$card_footer_medium'           | (min-height:48px)     | (min-height:48px)     |             |            |
|'$card_header_large '           | (min-height:56px)     | (min-height:56px)     |             |            |
|'$card_footer_large '           | (min-height:56px)     | (min-height:56px)     |             |            |
|'$card_padding'                 | '$base_padding'       | '$base_padding'       |             |            |
|'$card_margin'                  | '$base_margin'        | '$base_margin'        |             |            |
|'$card_border'                  | '$base_border'        | '$base_border'        |             |            |
|'$card_border_radius'           | '$base_border_radius' | '$base_border_radius' |             |            |

#### Checkbox

| Token name                     | Pixel Light           | Pixel Dark.           | Point Light | Point Dark |
| ------------------------------ | --------------------- | --------------------- | ----------- | ---------- |
|'$checkbox_small'               | 24px                  | 24px                  |             |            |
|'$checkbox_medium'              |                       |                       |             |            |
|'$checkbox_large'               |                       |                       |             |            |
|'$checkbox_padding'             | '$base_padding'       | '$base_padding'       |             |            |
|'$checkbox_margin'              | '$base_margin'        | '$base_margin'        |             |            |
|'$checkbox_border'              | '$base_border'        | '$base_border'        |             |            |
|'$checkbox_border_radius'       | '$base_border_radius' | '$base_border_radius' |             |            |

#### Date Picker

| Token name                     | Pixel Light           | Pixel Dark            | Point Light | Point Dark |
| ------------------------------ | --------------------- | --------------------- | ----------- | ---------- |
|'$date_picker_small'            | '$base_small'         | '$base_small'         |             |            |
|'$date_picker_medium'           | '$base_medium'        | '$base_medium'        |             |            |
|'$date_picker_large'            | '$base_large'         | '$base_large'         |             |            |
|'$date_picker_padding'          | '$base_padding'       | '$base_padding'       |             |            |
|'$date_picker_margin'           | '$base_margin'        | '$base_margin'        |             |            |
|'$date_picker_border'           | '$base_border'        | '$base_border'        |             |            |
|'$date_picker_border_radius'    | '$base_border_radius' | '$base_border_radius' |             |            |

#### Dropdown

| Token name                     | Pixel Light           | Pixel Dark            | Point Light | Point Dark |
| ------------------------------ | --------------------- | --------------------- | ----------- | ---------- |
|'$dropdown_small'               | '$base_small'         | '$base_small'         |             |            |
|'$dropdown_medium'              | '$base_medium'        | '$base_medium'        |             |            |
|'$dropdown_large'               | '$base_large'         | '$base_large'         |             |            |
|'$dropdown_padding'             | '$base_padding'       | '$base_padding'       |             |            |
|'$dropdown_margin'              | '$base_margin'        | '$base_margin'        |             |            |
|'$dropdown_border'              | '$base_border'        | '$base_border'        |             |            |
|'$dropdown_border_radius'       | '$base_border_radius' | '$base_border_radius' |             |            |

#### File upload

| Token name                     | Pixel Light           | Pixel Dark            | Point Light | Point Dark |
| ------------------------------ | --------------------- | --------------------- | ----------- | ---------- |
|'$file_upload_small'            | '$base_small'         | '$base_small'         |             |            |
|'$file_upload_medium'           | '$base_medium'        | '$base_medium'        |             |            |
|'$file_upload_large'            | '$base_large'         | '$base_large'         |             |            |
|'$file_upload_padding'          | '$base_padding'       | '$base_padding'       |             |            |
|'$file_upload_margin'           | '$base_margin'        | '$base_margin'        |             |            |
|'$file_upload_border'           | '$base_border'        | '$base_border'        |             |            |
|'$file_upload_border_radius'    | '$base_border_radius' | '$base_border_radius' |             |            |

#### Header

| Token name                     | Pixel Light           | Pixel Dark            | Point Light | Point Dark |
| ------------------------------ | --------------------- | --------------------- | ----------- | ---------- |
|'$header_small'                 | (min-height:40px)     | (min-height:40px)     |             |            |
|'$header_medium'                | (min-height:48px)     | (min-height:48px)     |             |            |
|'$header_large'                 | (min-height:56px)     | (min-height:56px)     |             |            |
|'$header_padding'               | '$base_padding'       | '$base_padding'       |             |            |
|'$header_margin'                | '$base_margin'        | '$base_margin'        |             |            |
|'$header_border'                | '$base_border'        | '$base_border'        |             |            |
|'$header_border_radius'         |                       |                       |             |            |

#### Icons

| Token name                     | Pixel Light           | Pixel Dark            | Point Light | Point Dark |
| ------------------------------ | --------------------- | --------------------- | ----------- | ---------- |
|'$icon_small'                   | 20px                  | 20px                  |             |            |
|'$icon_medium'                  | 24px                  | 24px                  |             |            |
|'$icon_large'                   | 28px                  | 28px                  |             |            |

#### International phone

| Token name                     | Pixel Light           | Pixel Dark            | Point Light | Point Dark |
| ------------------------------ | --------------------- | --------------------- | ----------- | ---------- |
|'$int_phone_small'              | '$base_small'         | '$base_small'         |             |            |
|'$int_phone_medium'             | '$base_medium'        | '$base_medium'        |             |            |
|'$int_phone_large'              | '$base_large'         | '$base_large'         |             |            |
|'$int_phone_padding'            | '$base_padding'       | '$base_padding'       |             |            |
|'$int_phone_margin'             | '$base_margin'        | '$base_margin'        |             |            |
|'$int_phone_border'             | '$base_border'        | '$base_border'        |             |            |
|'$int_phone_border_radius'      | '$base_border_radius' | '$base_border_radius' |             |            |

#### Loader

| Token name                     | Pixel Light           | Pixel Dark            | Point Light | Point Dark |
| ------------------------------ | --------------------- | --------------------- | ----------- | ---------- |
|'$loader_small'                 |                       |                       |             |            |
|'$loader_medium'                |                       |                       |             |            |
|'$loader_large'                 |                       |                       |             |            |
|'$loader_padding'               |                       |                       |             |            |
|'$loader_margin'                | '$base_margin'        | '$base_margin'        |             |            |
|'$loader_border'                |                       |                       |             |            |
|'$loader_border_radius'         |  100%                 | 100%                  |             |            |

#### Notifications

| Token name                     | Pixel Light           | Pixel Dark            | Point Light | Point Dark |
| ------------------------------ | --------------------- | --------------------- | ----------- | ---------- |
|'$notification_small'           |                       |                       |             |            |
|'$notification_medium'          |                       |                       |             |            |
|'$notification_large'           |                       |                       |             |            |
|'$notification_padding'         | '$base_padding'       | '$base_padding'       |             |            |
|'$notification_margin'          | '$base_margin'        | '$base_margin'        |             |            |
|'$notification_border'          | '$base_border'        | '$base_border'        |             |            |
|'$notification_border_radius'   | '$base_border_radius' | '$base_border_radius' |             |            |

#### Pagination

| Token name                     | Pixel Light           | Pixel Dark            | Point Light | Point Dark |
| ------------------------------ | --------------------- | --------------------- | ----------- | ---------- |
|'$pagination_small'             | (min-height:40px)     | (min-height:40px)     |             |            |
|'$pagination_medium'            | (min-height:48px)     | (min-height:48px)     |             |            |
|'$pagination_large'             | (min-height:56px)     | (min-height:56px)     |             |            |
|'$pagination_padding'           | '$base_padding'       | '$base_padding'       |             |            |
|'$pagination_margin'            | '$base_margin'        | '$base_margin'        |             |            |
|'$pagination_border'            |                       |                       |             |            |
|'$pagination_border_radius'     |                       |                       |             |            |

#### Password input

| Token name                     | Pixel Light           | Pixel Dark            | Point Light | Point Dark |
| ------------------------------ | --------------------- | --------------------- | ----------- | ---------- |
|'$password_small'               | '$base_small'         | '$base_small'         |             |            |
|'$password_medium'              | '$base_medium'        | '$base_medium'        |             |            |
|'$password_large'               | '$base_large'         | '$base_large'         |             |            |
|'$password_padding'             | '$base_padding'       | '$base_padding'       |             |            |
|'$password_margin'              | '$base_margin'        | '$base_margin'        |             |            |
|'$password_border'              | '$base_border'        | '$base_border'        |             |            |
|'$password_border_radius'       | '$base_border_radius' | '$base_border_radius' |             |            |

#### Progress indicator

| Token name                     | Pixel Light           | Pixel Dark            | Point Light | Point Dark |
| ------------------------------ | --------------------- | --------------------- | ----------- | ---------- |
|'$progress_small'               |                       |                       |             |            |
|'$progress_medium'              |                       |                       |             |            |
|'$progress_large'               |                       |                       |             |            |
|'$progress_padding'             | '$base_padding'       | '$base_padding'       |             |            |
|'$progress_margin'              | '$base_margin'        | '$base_margin'        |             |            |
|'$progress_border'              | '$base_border'        | '$base_border'        |             |            |
|'$progress_border_radius'       | '$base_border_radius' | '$base_border_radius' |             |            |

#### Radio

| Token name                     | Pixel Light           | Pixel Dark.           | Point Light | Point Dark |
| ------------------------------ | --------------------- | --------------------- | ----------- | ---------- |
|'$radio_small'                  | 24px                  | 24px                  |             |            |
|'$radio_medium'                 |                       |                       |             |            |
|'$radio_large'                  |                       |                       |             |            |
|'$radio_padding'                | '$base_padding'       | '$base_padding'       |             |            |
|'$radio_margin'                 | '$base_margin'        | '$base_margin'        |             |            |
|'$radio_border'                 | '$base_border'        | '$base_border'        |             |            |
|'$radio_border_radius'          |                       |                       |             |            |

#### Search input

| Token name                     | Pixel Light           | Pixel Dark            | Point Light | Point Dark |
| ------------------------------ | --------------------- | --------------------- | ----------- | ---------- |
|'$search_input_small'           | '$base_small'         | '$base_small'         |             |            |
|'$search_input_medium'          | '$base_medium'        | '$base_medium'        |             |            |
|'$search_input_large'           | '$base_large'         | '$base_large'         |             |            |
|'$search_input_padding'         | '$base_padding'       | '$base_padding'       |             |            |
|'$search_input_margin'          | '$base_margin'        | '$base_margin'        |             |            |
|'$search_input_border'          | '$base_border'        | '$base_border'        |             |            |
|'$search_input_border_radius'   | '$base_border_radius' | '$base_border_radius' |             |            |

#### Stepper

| Token name                     | Pixel Light           | Pixel Dark            | Point Light | Point Dark |
| ------------------------------ | --------------------- | --------------------- | ----------- | ---------- |
|'$stepper_small'                | '$base_small'         | '$base_small'         |             |            |
|'$stepper_medium'               | '$base_medium'        | '$base_medium'        |             |            |
|'$stepper_large'                | '$base_large'         | '$base_large'         |             |            |
|'$stepper_padding'              | '$base_padding'       | '$base_padding'       |             |            |
|'$stepper_margin'               | '$base_margin'        | '$base_margin'        |             |            |
|'$stepper_border'               | '$base_border'        | '$base_border'        |             |            |
|'$stepper_border_radius'        | '$base_border_radius' | '$base_border_radius' |             |            |

#### Table

| Token name                     | Pixel Light           | Pixel Dark            | Point Light | Point Dark |
| ------------------------------ | --------------------- | --------------------- | ----------- | ---------- |
|'$table_small'                  | (min-height:40px)     | (min-height:40px)     |             |            |
|'$table_medium'                 | (min-height:48px)     | (min-height:48px)     |             |            |
|'$table_large'                  | (min-height:56px)     | (min-height:56px)     |             |            |
|'$table_padding'                | '$base_padding'       | '$base_padding'       |             |            |
|'$table_margin'                 | '$base_margin'        | '$base_margin'        |             |            |
|'$table_border'                 | '$base_border'        | '$base_border'        |             |            |
|'$table_border_radius'          |                       |                       |             |            |

#### Tab navigation

| Token name                     | Pixel Light           | Pixel Dark            | Point Light | Point Dark |
| ------------------------------ | --------------------- | --------------------- | ----------- | ---------- |
|'$tab_small'                    | '$base_small'         | '$base_small'         |             |            |
|'$tab_medium'                   | '$base_medium'        | '$base_medium'        |             |            |
|'$tab_large'                    | '$base_large'         | '$base_large'         |             |            |
|'$tab_padding'                  | '$base_padding'       | '$base_padding'       |             |            |
|'$tab_margin'                   | '$base_border'        | '$base_border'        |             |            |
|'$tab_border_radius'            | '$base_border_radius' | '$base_border_radius' |             |            |

#### Tag

| Token name                     | Pixel Light           | Pixel Dark            | Point Light | Point Dark |
| ------------------------------ | --------------------- | --------------------- | ----------- | ---------- |
|'$tag_x_small'                  | 18px                  | 18px                  |             |            |
|'$tag_small'                    | 22px                  | 22px                  |             |            |
|'$tag_medium'                   | 28px                  | 28px                  |             |            |
|'$tag_large'                    | 32px                  | 32px                  |             |            |
|'$tag_x_large'                  | 40px                  | 40px                  |             |            |
|'$tag_padding'                  |                       |                       |             |            |
|'$tag_margin'                   | '$base_margin'        | '$base_margin'        |             |            |
|'$tag_border'                   | '$border_1'           | '$border_1'           |             |            |
|'$tag_border_radius'            | 100px                 | 100px                 |             |            |

#### Textarea

| Token name                     | Pixel Light           | Pixel Dark            | Point Light | Point Dark |
| ------------------------------ | --------------------- | --------------------- | ----------- | ---------- |
|'$textarea_small'               |                       |                       |             |            |
|'$textarea__medium'             |                       |                       |             |            |
|'$textarea__large'              |                       |                       |             |            |
|'$textarea__padding'            | '$base_padding'       | '$base_padding'       |             |            |
|'$textarea__margin'             | '$base_margin'        | '$base_margin'        |             |            |
|'$textarea__border'             | '$base_border'        | '$base_border'        |             |            |
|'$textarea__border_radius'      | '$base_border_radius' | '$base_border_radius' |             |            |

#### Toggle switch

| Token name                     | Pixel Light           | Pixel Dark            | Point Light | Point Dark |
| ------------------------------ | --------------------- | --------------------- | ----------- | ---------- |
|'$toggle_small'                 |                       |                       |             |            |
|'$toggle__medium'               |                       |                       |             |            |
|'$toggle__large'                |                       |                       |             |            |
|'$toggle__padding'              | '$base_padding'       | '$base_padding'       |             |            |
|'$toggle__margin'               | '$base_margin'        | '$base_margin'        |             |            |
|'$toggle__border'               | '$base_border'        | '$base_border'        |             |            |
|'$toggle__border_radius'        | '$base_border_radius' | '$base_border_radius' |             |            |

#### Tooltip

| Token name                     | Pixel Light           | Pixel Dark            | Point Light | Point Dark |
| ------------------------------ | --------------------- | --------------------- | ----------- | ---------- |
|'$tooltip_small'                |                       |                       |             |            |
|'$tooltip__medium'              |                       |                       |             |            |
|'$tooltip__large'               |                       |                       |             |            |
|'$tooltip__padding'             | '$base_padding'       | '$base_padding'       |             |            |
|'$tooltip__margin'              | '$base_margin'        | '$base_margin'        |             |            |
|'$tooltip__border'              |                       |                       |             |            |
|'$tooltip__border_radius'       | '$base_border_radius' | '$base_border_radius' |             |            |


### Borders

The border tokens help you control the proportions of your system’s components at the atom level for global consistency. This is a supplemental token structure for other tokens. Depending on the components defined in your initial system, the maturity of this template can include any additional components or attributes in the future.

The tokens should function as a common language during the product cycle. It is critical that the naming convention should be agreed upon between both development and design. Some tokens values can remain empty, using the token as a placeholder for other themes.

| Token name                     | Pixel Light           | Pixel Dark            | Point Light | Point Dark |
| ------------------------------ | --------------------- | --------------------- | ----------- | ---------- |
|'$border_1'                     | 1px                   | 1px                   |             |            |
|'$border_2                      | 2px                   | 2px                   |             |            |
|'$border_3                      | 3px                   | 3px                   |             |            |
|'$border_4'                     | 4px                   | 4px                   |             |            |
|'$border_5'                     | 5px                   | 5px                   |             |            |
|'$border_6'                     | 6px                   | 6px                   |             |            |
|'$border_7'                     | 7px                   | 7px                   |             |            |
|'$border_8'                     | 8px                   | 8px                   |             |            |
|'$border_9                      | 9px                   | 9px                   |             |            |
|'$border_10                     | 10px                  | 10px                  |             |            |
|'$border_11'                    | 11px                  | 11px                  |             |            |
|'$border_12'                    | 12px                  | 12px                  |             |            |
|'$border_13'                    | 13px                  | 13px                  |             |            |
|'$border_14'                    | 14px                  | 14px                  |             |            |

### Spacing

The spacing tokens help you control the proportions of your system’s components at the atom level for global consistency. This is a supplemental token structure for other tokens. Depending on the components defined in your initial system, the maturity of this template can include any additional components or attributes in the future.

The tokens should function as a common language during the product cycle. It is critical that the naming convention should be agreed upon between both development and design. Some tokens values can remain empty, using the token as a placeholder for other themes.

| Token name                     | Pixel Light           | Pixel Dark            | Point Light | Point Dark |
| ------------------------------ | --------------------- | --------------------- | ----------- | ---------- |
|'$spacing_1'                    | 1px                   | 1px                   |             |            |
|'$spacing_2                     | 2px                   | 2px                   |             |            |
|'$spacing_3                     | 3px                   | 3px                   |             |            |
|'$spacing_4'                    | 4px                   | 4px                   |             |            |
|'$spacing_5'                    | 5px                   | 5px                   |             |            |
|'$spacing_6'                    | 6px                   | 6px                   |             |            |
|'$spacing_7'                    | 7px                   | 7px                   |             |            |
|'$spacing_8'                    | 8px                   | 8px                   |             |            |
|'$spacing_9                     | 9px                   | 9px                   |             |            |
|'$spacing_10                    | 10px                  | 10px                  |             |            |
|'$spacing_11'                   | 11px                  | 11px                  |             |            |
|'$spacing_12'                   | 12px                  | 12px                  |             |            |
|'$spacing_13'                   | 13px                  | 13px                  |             |            |
|'$spacing_14'                   | 14px                  | 14px                  |             |            |
|'$spacing_15                    | 15px                  | 15px                  |             |            |
|'$spacing_16'                   | 16px                  | 16px                  |             |            |
|'$spacing_17'                   | 17px                  | 17px                  |             |            |
|'$spacing_18'                   | 18px                  | 18px                  |             |            |
|'$spacing_19'                   | 19px                  | 19px                  |             |            |
|'$spacing_20                    | 20px                  | 20px                  |             |            |
|'$spacing_21'                   | 21px                  | 21px                  |             |            |
|'$spacing_22'                   | 22px                  | 22px                  |             |            |
|'$spacing_23'                   | 23px                  | 23px                  |             |            |
|'$spacing_24'                   | 24px                  | 24px                  |             |            |

### Palettes

The color palettes help you define the structured colors that are used with various color layer tokens of your system’s components at the atom level for global consistency. Depending on the components defined in your initial system, the maturity of this template can include any additional components or attributes in the future.

The tokens should function as a common language during the product cycle. It is critical that the naming convention should be agreed upon between both development and design. Some tokens values can remain empty, using the token as a placeholder for other themes.

Palettes can be modified, or additional palettes can be added to your token architecture. All palette colors provide WCAG contrast measurement (ratio >3:1) with background and foreground, which is outlined below.

#### Black and white

| Token name                     | Background            | Foreground            | WCAG Ratio  |
| ------------------------------ | --------------------- | --------------------- | ----------- |
|'$white'                        | '#FFFFFF'             | '#000000'             | 00.21:1     | 
|'$black'                        | '#000000'             | '#FFFFFF'             | 00.21:1     | 

#### Red

| Token name                     | Background            | Foreground            | WCAG Ratio  |
| ------------------------------ | --------------------- | --------------------- | ----------- |
|'$red_900'                      | '#C00000'             | '#FFFFFF'             | 06.47:1     | 
|'$red_800'                      | '#CE1A12'             | '#FFFFFF'             | 05.55:1     | 
|'$red_700'                      | '#DB231B'             | '#FFFFFF'             | 04.92:1     |
|'$red_600'                      | '#ED3020'             | '#000000'             | 05.04:1     | 
|'$red_500'                      | '#FB3C1E'             | '#000000'             | 05.76:1     | 
|'$red_400'                      | '#F74D40'             | '#000000'             | 06.09:1     | 
|'$red_300'                      | '#EE6F68'             | '#000000'             | 07.01:1     | 
|'$red_200'                      | '#F69892'             | '#000000'             | 09.82:1     | 
|'$red_100'                      | '#FFCCCE'             | '#000000'             | 14.78:1     | 
|'$red_050'                      | '#FFEAED'             | '#000000'             | 18.24:1     | 
|'$red_A100'                     | '#FFF7F8'             | '#000000'             | 19.91:1     | 

#### Pink

| Token name                     | Background            | Foreground            | WCAG Ratio  |
| ------------------------------ | --------------------- | --------------------- | ----------- |
|'$pink_900'                     | '#880E4F'             | '#FFFFFF'             | 09.44:1     | 
|'$pink_800'                     | '#AD1457'             | '#FFFFFF'             | 06.96:1     | 
|'$pink_700'                     | '#C2185B'             | '#FFFFFF'             | 05.87:1     |
|'$pink_600'                     | '#D81B60'             | '#FFFFFF'             | 04.94:1     | 
|'$pink_500'                     | '#E91E63'             | '#000000'             | 04.83:1     | 
|'$pink_400'                     | '#EC407A'             | '#000000'             | 05.58:1     | 
|'$pink_300'                     | '#F06292'             | '#000000'             | 06.86:1     | 
|'$pink_200'                     | '#F48FB1'             | '#000000'             | 09.41:1     | 
|'$pink_100'                     | '#F8BBD0'             | '#000000'             | 13.01:1     |
|'$pink_050'                     | '#FCE4EC'             | '#000000'             | 17.44:1     | 
|'$pink_A100'                    | '#FDEFF4'             | '#000000'             | 18.82:1     | 



### Color

The color tokens help you control the visual layer of your system’s components at the atom level for global consistency. Depending on the components defined in your initial system, the maturity of this template can include any additional components or attributes in the future.

The tokens should function as a common language during the product cycle. It is critical that the naming convention should be agreed upon between both development and design. Some tokens values can remain empty, using the token as a placeholder for other themes.


#### Background

| Token name                     | Pixel Light           | Pixel Dark            | Point Light | Point Dark |
| ------------------------------ | --------------------- | --------------------- | ----------- | ---------- |
|'$background'                   | '$white'              | '$black'              |             |            |
|'$background_brand'             | '$orange_500'         | '$oranage_500'        |             |            |
|'$background_hover'             |                       |                       |             |            |
|'$background_inverse'           |                       |                       |             |            |
|'$background_inverse_hover'     |                       |                       |             |            |
|'$background_selected'          |                       |                       |             |            |
|'$background_seected_hover'     |                       |                       |             |            |

#### Border

| Token name                     | Pixel Light           | Pixel Dark            | Point Light | Point Dark |
| ------------------------------ | --------------------- | --------------------- | ----------- | ---------- |
|'$border_interactive'           | '$blue_800'           | '$blue_600'           |             |            |
|'$border_subtle_1'              | '$gray_300'           | '$gray_800'           |             |            |
|'$border_subtle_2'              |                       |                       |             |            |
|'$border_subtle_3'              |                       |                       |             |            |
|'$border_subtle_selected_1'     |                       |                       |             |            |
|'$border_subtle_selected_2'     |                       |                       |             |            |
|'$border_subtle_selected_3'     |                       |                       |             |            |
|'$border_strong_1'              | '$gray_400'           | '$gray_600'           |             |            |
|'$border_strong_2'              |                       |                       |             |            |
|'$border_strong_3'              |                       |                       |             |            |
|'$border_strong_selected_1'     |                       |                       |             |            |
|'$border_strong_selected_2'     |                       |                       |             |            |
|'$border_strong_selected_3'     |                       |                       |             |            |
|'$border_card_1'                |                       |                       |             |            |
|'$border_card_2'                |                       |                       |             |            |
|'$border_card_3'                |                       |                       |             |            |
|'$border_inverse'               | '$gray_700'           | '$gray_100'           |             |            |
|'$border_disabled'              | '$gray_300'           | '$gray_500'           |             |            |

#### Button

| Token name                     | Pixel Light           | Pixel Dark            | Point Light | Point Dark |
| ------------------------------ | --------------------- | --------------------- | ----------- | ---------- |
|'$button_primary'               | '$blue_800'           | '$blue_600'           |             |            |
|'$button_primary_hover'         | '$blue_700'           | '$blue_500'           |             |            |
|'$button_primary_selected'      | '$blue_900'           | '$blue_800'           |             |            |
|'$button_secondary'             | '$blue_800'           | '$white'              |             |            |
|'$button_secondary_hover'       | '$blue_700'           | 'rgba($white,.25)'    |             |            |
|'$button_secondary_selected'    | '$blue_900'           | 'rgba($white,.25)'    |             |            |
|'$button_tertiary'              | 'rgba($blue_800,.00)' | 'rgba($white,.00)'    |             |            |
|'$button_tertiary_hover'        | 'rgba($blue_800'.25)' | 'rgba($white,.25)'    |             |            |
|'$button_tertiary_selected'     | 'rgba($blue_800'.25)' | 'rgba($white,.25)'    |             |            |
|'$button_danger'                | '$red_800'            | '$red_700'            |             |            |
|'$button_danger_hover'          | '$red_700'            | '$red_600'            |             |            |
|'$button_danger_selected'       | '$red_400'            | '$red_900'            |             |            |
|'$button_seperator'             |                       |                       |             |            |
|'$button_danger_selected'       | '$gray_400'           | '$gray_600'           |             |            |

#### Field

| Token name                     | Pixel Light           | Pixel Dark            | Point Light | Point Dark |
| ------------------------------ | --------------------- | --------------------- | ----------- | ---------- |
|'$field_1'                      | '$white'              | '$black'              |             |            |
|'$field_2'                      |                       |                       |             |            |
|'$field_3'                      |                       |                       |             |            |
|'$field_hover_1'                |                       |                       |             |            |
|'$field_hover_2'                |                       |                       |             |            |
|'$field_hover_3'                |                       |                       |             |            |
|'$field_disabled_1'             | '$gray_100'           | '$gray_900'           |             |            |
|'$field_disabled_2'             |                       |                       |             |            |
|'$field_disabled_3'             |                       |                       |             |            |
|'$fieldset_1'                   | '$gray_50'            | '$gray_800'           |             |            |
|'$fieldset_2                    |                       |                       |             |            |
|'$fieldset_3'                   |                       |                       |             |            |

#### Focus

| Token name                     | Pixel Light           | Pixel Dark            | Point Light | Point Dark |
| ------------------------------ | --------------------- | --------------------- | ----------- | ---------- |
|'$focus'                        | '$blue_800'           | '$white'              |             |            |
|'$focus_highlight'              | '$blue_A100'          | 'rgba($white,.25)'    |             |            |
|'$focus_inset'                  |                       |                       |             |            |
|'$focus_inverse'                | '$white'              | '$blue_600'           |             |            |
|'$focus_inverse_highlight'      | 'rgba($white,.10)'    | 'rgba($blue_600,.10)' |             |            |

#### Icon

| Token name                     | Pixel Light           | Pixel Dark            | Point Light | Point Dark |
| ------------------------------ | --------------------- | --------------------- | ----------- | ---------- |
|'$icon_primary'                 | '$gray_900'           | '$gray_100'           |             |            |
|'$icon_secondary'               | '$gray_700'           | '$gray_300'           |             |            |
|'$icon_on_color'                | '$white'              | '$white'              |             |            |
|'$icon_on_color_disabled'       | 'rgba($white,.50)'    | 'rgba($white,.50)'    |             |            |
|'$icon_interactive'             | '$blue_700'           | '$blue_600'           |             |            |
|'$icon_inverse'                 | '$white'              | '$black'              |             |            |
|'$icon_disabled'                | '$gray_500'           | 'gray_600'            |             |            |

#### Layer

| Token name                     | Pixel Light            | Pixel Dark             | Point Light | Point Dark |
| ------------------------------ | ---------------------- | ---------------------- | ----------- | ---------- |
|'$layer_1'                      | '$white'               | '$gray_900'            |             |            |
|'$layer_2'                      | '$slate_50'            | '$gray_800'            |             |            |
|'$layer_3'                      | '$white'               | '$gray_900'            |             |            |
|'$layer_hover_1'                | '$slate_50'            | '$gray_800'            |             |            |
|'$layer_hover_2'                | '$slate_100'           | '$gray_700'            |             |            |
|'$layer_hover_3'                | '$slate_50'            | '$gray_600'            |             |            |
|'$layer_selected_1'             | '$blue_900'            | '$gray_900'            |             |            |
|'$layer_selected_2'             | '$blue_900'            | '$gray_900'            |             |            |
|'$layer_selected_3'             | '$blue_900'            | '$gray_900'            |             |            |
|'$layer_selected_hover_1'       |                        |                        |             |            |
|'$layer_selected_hover_2'       |                        |                        |             |            |
|'$layer_selected_hover_3'       |                        |                        |             |            |
|'$layer_disabled_1'             | '$gray_100'            |'$gray_800'             |             |            |
|'$layer_disabled_2'             |                        |                        |             |            |
|'$layer_disabled_3'             |                        |                        |             |            |

#### Layer accent

| Token name                     | Pixel Light            | Pixel Dark             | Point Light | Point Dark |
| ------------------------------ | ---------------------- | ---------------------- | ----------- | ---------- |
|'$layer_accent_1'               | '$gray_300'            | '$gray_800'            |             |            |
|'$layer_accent_2'               |                        |                        |             |            |
|'$layer_accent_3'               |                        |                        |             |            |
|'$layer_accent_hover_1'         |                        |                        |             |            |
|'$layer_accent_hover_2'         |                        |                        |             |            |
|'$layer_accent_hover_3'         |                        |                        |             |            |
|'$layer_accent_selected_1'      |                        |                        |             |            |
|'$layer_accent_selected_2'      |                        |                        |             |            |
|'$layer_accent_selected_3'      |                        |                        |             |            |

#### Link

| Token name                     | Pixel Light            | Pixel Dark             | Point Light | Point Dark |
| ------------------------------ | ---------------------- | ---------------------- | ----------- | ---------- |
|'$link_primary'                 | '$blue_700'            | '$blue_400'            |             |            |
|'$link_primary_hover'           | '$blue_800'            | '$blue_300'            |             |            |
|'$link_primary_selected'        | '$blue_900'            | '$blue_900'            |             |            |
|'$link_secondary'               |                        |                        |             |            |
|'$link_secondary_hover'         |                        |                        |             |            |
|'$link_secondary_selected'      |                        |                        |             |            |
|'$link_inverse'                 | '$blue_500'            | '$blue_600'            |             |            |
|'$link_inverse_hover'           |                        |                        |             |            |
|'$link_inverse_selected'        |                        |                        |             |            |
|'$link_visited'                 |                        |                        |             |            |
|'$link_disabled'                | '$gray_500'            | '$gray_500'            |             |            |

#### Support

| Token name                     | Pixel Light            | Pixel Dark             | Point Light | Point Dark |
| ------------------------------ | ---------------------- | ---------------------- | ----------- | ---------- |
|'$support_error'                | '$red_800'             | '$red_700'             |             |            |
|'$support_error_bg'             | '$red_A100'            | 'rgba($red_700,.10)'   |             |            |
|'$support_success'              | '$green_900'           | '$green_700'           |             |            |
|'$support_success_bg'           | '$green_A100'          | 'rgba($green_700,.10)' |             |            |
|'$support_warning'              | '$orange_500'          | '$orange_400'          |             |            |
|'$support_warning_bg'           | '$orange_A100'         | 'rgba($orange_400,.10)'|             |            |
|'$support_information'          | '$blue_800'            | '$blue_600'            |             |            |
|'$support_information_bg'       | '$blue_A100'           | '$rgba($blue_600,.10)' |             |            |

#### Text

| Token name                     | Pixel Light            | Pixel Dark             | Point Light | Point Dark |
| ------------------------------ | ---------------------- | ---------------------- | ----------- | ---------- |
|'$text_primary'                 | '$gray_900'            | '$gray_100'            |             |            |
|'$text_secondary'               | '$gray_700'            | '$gray_300'            |             |            |
|'$text_placeholder'             | '$gray_500'            | '$gray_600'            |             |            |
|'$text_on_color'                | '$white'               | '$white'               |             |            |
|'$text_on_color_disabled'       | '$rgba($white,.50)'    | 'rgba($white,.50)'     |             |            |
|'$text_inverse'                 | '$white'               | '$black'               |             |            |
|'$text_disabled'                | '$gray_500'            | '$gray_600'            |             |            |

#### Miscellaneous

| Token name                     | Pixel Light            | Pixel Dark             | Point Light | Point Dark |
| ------------------------------ | ---------------------- | ---------------------- | ----------- | ---------- |
|'$interative'                   | '$blue_800'            | '$blue_600'            |             |            |
|'$highlight'                    |                        |                        |             |            |
|'$overlay'                      | 'rgba($black,.50)'     | 'rgba($black,.50)'     |             |            |
|'$skeleton_element'             | '$gray_400'            | '$gray_800'            |             |            |
|'$skeleton_background'          | '$gray_200'            | 'gray_900'             |             |            |

