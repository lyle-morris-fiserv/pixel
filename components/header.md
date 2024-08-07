# Header

The header is the foundation for navigating and orienting your user to the user interface. The user interface header shell can be used by itself or combined with the left and right panels for more complex navigation.

## Usage

### When to use

- Identify the UI by name.
- Globally persistent location for navigational links and utilities.

| Variant                        | Purpose |
|:------------------------------ | :------ |
| Header base                    | Has a persistent site title that can be used to identify a single page UI (user interface). |
| Header with navigation         | Includes links and dropdowns for a simple navigation. |
| Header with actions            | Actions or utilities appear in the header as icon buttons to give users quick access to common utilities. |
| Header with side navigation    | The header can be paired with the UI shell left panel to offer a deeper level of navigation in a user interface. |

## Anatomy

The header spans the full width of the viewport and is the topmost element in the browser window. The header is persistent throughout the product experience.

For each UI shell component, left-to-right translates to product-to-global. The left side of the header contains items relevant at the product level. Moving to the right along the header, the functions become more global. Elements in the middle of the header should represent system-level controls. Elements on the right side of the header, such as the switcher, are the most global in their scope and span multiple products.

1. **Menu** - The hamburger icon is used to open product navigation such as the left panel. The hamburger menu is only needed when there is a collapsible left navigation.
2. **Branded logo** - Logo/graphic branding. 
3. **Branded name** - For Financial Institutions branding.
4. **Link** - Links in the header are supported as product navigation, if required. These links move to the side menu in narrow screen widths.
5. **Link selected** - Indicated what area the user is one with the application.
6. **Link sub-menu** - Sub-menus are supported as product navigation, if required. Include the down-pointing chevron after the link label. Sub-menus open on click and are closed by either selecting an item in the menu, clicking outside the menu area, or clicking on the menu label. When open, the chevron should point up. Sub-menu labels serve only to open the dropdown; they cannot link to another page in the product.
7. **Utilities** - These utilities are reserved for universal, system-level functions such as profile, search, notifications, and similar functions. Not every product on a system is required to show the same utilities, but it is recommended for a better cross-product user experience.

## Search

The header will have a global search that focuses on not just the page but the complete application. Please reference the global search pattern. When the user clicks the search icon, it should use majority of the header to provide the best experience for the user. In the example below we have deprioritized the primary links of the application - keeping the navbar, branding and utility actions.

When the user clicks the close icon for the search, the header will transition back to the original layout.
 
- **Option 1** - 60% of the header; Primary links deprioritized.
- **Option 2** - 100% of the header; All elements deprioritized.

## Placement

Icons are not a required element of the header, and a product may choose to use any set of icons for their UI. Icons should always be aligned to the right of the header with no gaps between icons. Header utilities are right aligned with no gaps. Below are standard utilities items that are used in the header. These options are recognized and standardized in product design by users.

Below are standard utilities items that are used in the header. These options are recognized and standardized in product design by users.

| # | Icon     | Placement |
| _ | :------- | :-------- |
| 1 | Search   | Search should always be positioned as the furthest left icon. This is to allow for an expanding search field that does not disrupt other icon positions. |
| 2 | Other    | The number of header icons a product uses may vary. This placement will help avoid disrupting the position of the core icons and inconsistencies as your user navigates between other product shell headers. |
| 3 | Help     | Help is positioned 5th from the right. |
| 4 | Alerts   | Notifications should be 4th from the right when paired with the account and switcher icon. |
| 5 | Account  | The account should be the 3rd from the right. This global link gives a user quick access to their account from anywhere in the product UI. |
| 6 | Settings | Settings is position 2nd from the right next to account. |
| 7 | Switcher | The switcher should always be positioned as the furthest right icon. This ensures the icon does not shift when navigating across systems. |

