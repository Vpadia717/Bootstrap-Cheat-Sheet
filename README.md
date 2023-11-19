# Bootstrap Cheat Sheet

![GitHub](Github.webp)

Welcome to the Bootstrap Cheat Sheet, your go-to guide for mastering Bootstrap and creating stunning web pages with ease!

## Check out Live Demo

[Live Demo](https://vpadia717.github.io/Bootstrap-Cheat-Sheet/)

## Table of Contents

- [Introduction](#introduction)
- [Breakpoint](#breakpoint)
- [Options](#options)
- [Grid](#grid)
- [Margin](#margin)
- [Padding](#padding)
- [Table](#table)
- [Buttons](#buttons)
- [Badges](#badges)
- [Jumpbotron](#jumpbotron)
- [Breadcrumbs](#breadcrumbs)

## Introduction

Bootstrap, founded by <code>Twitter</code>, is a robust and <b>widely-used</b>, <i>open-source</i> <mark>front-end</mark> framework that streamlines and accelerates web development. It is built on HTML, CSS, and JavaScript and provides a responsive grid system, pre-designed components, and a plethora of utility classes.

<details>
<summary>Introduction to Bootstrap</summary>
Bootstrap is a popular open-source front-end framework that simplifies the process of designing and developing responsive and mobile-first web pages. Here's a brief overview of key concepts and features:
  
- **What is Bootstrap?**
  - Bootstrap is a powerful and flexible front-end framework developed by Twitter.
  - It provides a collection of HTML, CSS, and JavaScript components, making it easy to create modern and visually appealing websites.

- **Key Features:**

  - **Responsive Design:**
    - Bootstrap follows a responsive design approach, ensuring that web pages look good on various devices and screen sizes.
  - **Pre-designed Components:**
    - Bootstrap offers a rich set of pre-designed components such as navigation bars, buttons, forms, and more, saving developers time and effort.
  - **Grid System:**
    - The grid system in Bootstrap facilitates the creation of responsive and flexible layouts, allowing developers to create complex designs with ease.
  - **Customizable Styles:**
    - Bootstrap's styling is highly customizable, allowing developers to easily modify the appearance of components to match their design preferences.
  - **JavaScript Plugins:**
    - Bootstrap includes a variety of JavaScript plugins for common functionalities like modals, carousels, and tooltips, enhancing the interactive aspects of a website.

- **Getting Started:**
  - To get started with Bootstrap, include the Bootstrap CSS and JavaScript files in your HTML document. You can either download the files or use a CDN for quicker integration.
- **Documentation:**
  - Bootstrap provides comprehensive documentation with examples and guidelines for each component. It's a valuable resource for developers to explore and master Bootstrap.
- **Community and Support:**
  - Bootstrap has a vibrant community of developers who actively contribute to its development. There are also forums and online communities where developers can seek help and share their knowledge.

Bootstrap is an excellent choice for both beginners and experienced developers, offering a solid foundation for creating modern and visually appealing web applications.

# Bootstrap CDN Links

Below are the CDN links for Bootstrap CSS and JS. You can include these links in your HTML file to easily integrate Bootstrap into your project.

| Description | Link                                                                           |
| ----------- | ------------------------------------------------------------------------------ |
| CSS         | `https://cdn.jsdelivr.net/npm/bootstrap@5.3.2/dist/css/bootstrap.min.css`      |
| JS          | `https://cdn.jsdelivr.net/npm/bootstrap@5.3.2/dist/js/bootstrap.bundle.min.js` |

</details>

## Breakpoint

Bootstrap breakpoints are predefined points in the viewport width where the layout of a website can be adjusted to accommodate different screen sizes. These breakpoints play a crucial role in creating responsive designs. Here's an overview of Bootstrap breakpoints:

<details>
  <summary>Breakpoint</summary>
  
## Extra Small (xs)
- **Class Prefix:** `col`
- **Viewport Range:** `<576px`
- **Usage:** Suitable for mobile devices. Columns with the `col` class will stack vertically.

## Small (sm)

- **Class Prefix:** `sm`
- **Viewport Range:** `≥576px`
- **Usage:** Ideal for small devices like tablets. Adds responsiveness to columns with the `sm` class.

## Medium (md)

- **Class Prefix:** `md`
- **Viewport Range:** `≥768px`
- **Usage:** Commonly used for larger tablets and desktops. Applies styles to columns with the `md` class.

## Large (lg)

- **Class Prefix:** `lg`
- **Viewport Range:** `≥992px`
- **Usage:** Suitable for larger desktops and laptops. Styles applied to columns with the `lg` class.

## Extra Large (xl)

- **Class Prefix:** `xl`
- **Viewport Range:** `≥1200px`
- **Usage:** Ideal for extra-large screens. Columns with the `xl` class will have specific styles.

## Responsive Utilities

Bootstrap provides additional responsive utility classes for hiding or showing content based on breakpoints.

- `d-sm-none`: Hide on small screens.
- `d-md-block`: Display as a block on medium screens.

## How to Use

Apply the appropriate class prefixes to your HTML elements based on the desired breakpoint.

```HTML
<div class="container">
  <h1 class="mt-3">Responsive Columns Example</h1>

  <div class="row">
    <!-- Extra Small (xs) -->
    <div class="col-12 col-sm-6 col-md-4 col-lg-3 col-xl-2 bg-primary text-white p-3">
      <p>Column 1</p>
    </div>

    <!-- Small (sm) -->
    <div class="col-12 col-sm-6 col-md-4 col-lg-3 col-xl-2 bg-secondary text-white p-3">
      <p>Column 2</p>
    </div>

    <!-- Medium (md) -->
    <div class="col-12 col-sm-6 col-md-4 col-lg-3 col-xl-2 bg-info text-white p-3">
      <p>Column 3</p>
    </div>

    <!-- Large (lg) -->
    <div class="col-12 col-sm-6 col-md-4 col-lg-3 col-xl-2 bg-warning text-white p-3">
      <p>Column 4</p>
    </div>

    <!-- Extra Large (xl) -->
    <div class="col-12 col-sm-6 col-md-4 col-lg-3 col-xl-2 bg-danger text-white p-3">
      <p>Column 5</p>
    </div>
  </div>
</div>
```

</details>

## Options

Quickly customize Bootstrap with built-in variables to easily toggle global CSS preferences for controlling style and behavior. Customize Bootstrap with our built-in custom variables file and easily toggle global CSS preferences with new <code>$enable-\*</code> Sass variables. Override a variable’s value and recompile with <code>npm run test</code> as needed.

<details>
  <summary>Options</summary>
  
Bootstrap offers a range of customizable options that empower you to tailor your web development projects. Below is a detailed table summarizing key variables, their values, and descriptions for these options.

| Variable                         | Values                             | Description                                                                                                                                                                                                                                    |
| -------------------------------- | ---------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **$spacer**                      | `1rem` (default), or any value > 0 | Specifies the default spacer value to programmatically generate our [spacer utilities](https://getbootstrap.com/docs/5.3/utilities/spacing/).                                                                                                  |
| **$enable-dark-mode**            | `true` (default) or `false`        | Enables built-in [dark mode support](https://getbootstrap.com/docs/5.3/customize/color-modes/#dark-mode) across the project and its components.                                                                                                |
| **$enable-rounded**              | `true` (default) or `false`        | Enables predefined `border-radius` styles on various components.                                                                                                                                                                               |
| **$enable-shadows**              | `true` or `false` (default)        | Enables predefined decorative `box-shadow` styles on various components. Does not affect `box-shadow`s used for focus states.                                                                                                                  |
| **$enable-gradients**            | `true` or `false` (default)        | Enables predefined gradients via `background-image` styles on various components.                                                                                                                                                              |
| **$enable-transitions**          | `true` (default) or `false`        | Enables predefined `transition`s on various components.                                                                                                                                                                                        |
| **$enable-reduced-motion**       | `true` (default) or `false`        | Enables the [`prefers-reduced-motion` media query](https://getbootstrap.com/docs/5.3/getting-started/accessibility/#reduced-motion), which suppresses certain animations/transitions based on the users’ browser/operating system preferences. |
| **$enable-grid-classes**         | `true` (default) or `false`        | Enables the generation of CSS classes for the grid system (e.g., `.row`, `.col-md-1`, etc.).                                                                                                                                                   |
| **$enable-container-classes**    | `true` (default) or `false`        | Enables the generation of CSS classes for layout containers. (New in v5.2.0)                                                                                                                                                                   |
| **$enable-caret**                | `true` (default) or `false`        | Enables pseudo-element caret on `.dropdown-toggle`.                                                                                                                                                                                            |
| **$enable-button-pointers**      | `true` (default) or `false`        | Adds “hand” cursor to non-disabled button elements.                                                                                                                                                                                            |
| **$enable-rfs**                  | `true` (default) or `false`        | Globally enables [RFS](https://getbootstrap.com/docs/5.3/getting-started/rfs/).                                                                                                                                                                |
| **$enable-validation-icons**     | `true` (default) or `false`        | Enables `background-image` icons within textual inputs and some custom forms for validation states.                                                                                                                                            |
| **$enable-negative-margins**     | `true` or `false` (default)        | Enables the generation of [negative margin utilities](https://getbootstrap.com/docs/5.3/utilities/spacing/#negative-margin).                                                                                                                   |
| **$enable-deprecation-messages** | `true` (default) or `false`        | Set to `false` to hide warnings when using any of the deprecated mixins and functions that are planned to be removed in `v6`.                                                                                                                  |
| **$enable-important-utilities**  | `true` (default) or `false`        | Enables the `!important` suffix in utility classes.                                                                                                                                                                                            |
| **$enable-smooth-scroll**        | `true` (default) or `false`        | Applies `scroll-behavior: smooth` globally, except for users asking for reduced motion through [`prefers-reduced-motion`](https://getbootstrap.com/docs/5.3/getting-started/accessibility/#reduced-motion) media query.                        |

## Usage Example

To use these options, include the Bootstrap stylesheet and JavaScript files in your HTML file. Here's a basic example:

```HTML
<body class="bg-light text-dark p-4">
  <div class="container">
    <h1 class="mt-4">Bootstrap Options Example</h1>
    <div class="p-4 mb-4 bg-white rounded">
      <h2 class="mb-3">Section 1</h2>
      <p>
        This is a custom box with predefined Bootstrap styles. It utilizes
        options such as background-color, text color, padding, border, and
        border-radius.
      </p>
    </div>
    <div class="p-4 mb-4 bg-white rounded">
      <h2 class="mb-3">Section 2</h2>
      <p>
        Another custom box with similar styling. Bootstrap options make it easy
        to create consistent and visually appealing designs.
      </p>
    </div>
  </div>
</body>
```

</details>

## Grid

Basic grid layouts to get you familiar with building within the Bootstrap grid system.
In these examples the `.themed-grid-col` class is added to the columns to add some theming. This is not a class that is available in Bootstrap by default.

<details>
  <summary>Grid</summary>
  
  Basic grid layouts to get you familiar with building within the Bootstrap grid system.
  
  In these examples the `.themed-grid-col` class is added to the columns to add some theming. This is not a class that is available in Bootstrap by default.
  
  ### Five grid tiers
  
  There are five tiers to the Bootstrap grid system, one for each range of devices we support. Each tier starts at a minimum viewport size and automatically applies to the larger devices unless overridden.
  
  #### Different Text for Different Column Sizes

```html
<div class="row mb-3 text-center">
  <div class="col-4 themed-grid-col">.col-4 - Small</div>
  <div class="col-4 themed-grid-col">.col-4 - Small</div>
  <div class="col-4 themed-grid-col">.col-4 - Small</div>
</div>
```

### Medium

```html
<div class="row mb-3 text-center">
  <div class="col-sm-4 themed-grid-col">.col-sm-4 - Medium</div>
  <div class="col-sm-4 themed-grid-col">.col-sm-4 - Medium</div>
  <div class="col-sm-4 themed-grid-col">.col-sm-4 - Medium</div>
</div>
```

### Large

```html
<div class="row mb-3 text-center">
  <div class="col-md-4 themed-grid-col">.col-md-4 - Large</div>
  <div class="col-md-4 themed-grid-col">.col-md-4 - Large</div>
  <div class="col-md-4 themed-grid-col">.col-md-4 - Large</div>
</div>
```

### Extra Large

```html
<div class="row mb-3 text-center">
  <div class="col-lg-4 themed-grid-col">.col-lg-4 - Extra Large</div>
  <div class="col-lg-4 themed-grid-col">.col-lg-4 - Extra Large</div>
  <div class="col-lg-4 themed-grid-col">.col-lg-4 - Extra Large</div>
</div>
```

### Extra Extra Large

```html
<div class="row mb-3 text-center">
  <div class="col-xl-4 themed-grid-col">.col-xl-4 - Extra Extra Large</div>
  <div class="col-xl-4 themed-grid-col">.col-xl-4 - Extra Extra Large</div>
  <div class="col-xl-4 themed-grid-col">.col-xl-4 - Extra Extra Large</div>
</div>
```

### Extra Extra Extra Large

```html
<div class="row mb-3 text-center">
  <div class="col-xxl-4 themed-grid-col">
    .col-xxl-4 - Extra Extra Extra Large
  </div>
  <div class="col-xxl-4 themed-grid-col">
    .col-xxl-4 - Extra Extra Extra Large
  </div>
  <div class="col-xxl-4 themed-grid-col">
    .col-xxl-4 - Extra Extra Extra Large
  </div>
</div>
```

### Three equal columns

Get three equal-width columns starting at desktops and scaling to large desktops. On mobile devices, tablets, and below, the columns will automatically stack.

```html
<div class="row mb-3 text-center">
  <div class="col-md-4 themed-grid-col">.col-md-4</div>
  <div class="col-md-4 themed-grid-col">.col-md-4</div>
  <div class="col-md-4 themed-grid-col">.col-md-4</div>
</div>
```

### Three equal columns alternative

By using the `.row-cols-*` classes, you can easily create a grid with equal columns.

```html
<div class="row row-cols-md-3 mb-3 text-center">
  <div class="col themed-grid-col">
    <code>.col</code> child of <code>.row-cols-md-3</code>
  </div>
  <div class="col themed-grid-col">
    <code>.col</code> child of <code>.row-cols-md-3</code>
  </div>
  <div class="col themed-grid-col">
    <code>.col</code> child of <code>.row-cols-md-3</code>
  </div>
</div>
```

### Three unequal columns

Get three columns starting at desktops and scaling to large desktops of various widths. Remember, grid columns should add up to twelve for a single horizontal block. More than that, columns start stacking no matter the viewport.

```html
<div class="row mb-3 text-center">
  <div class="col-md-3 themed-grid-col">.col-md-3</div>
  <div class="col-md-6 themed-grid-col">.col-md-6</div>
  <div class="col-md-3 themed-grid-col">.col-md-3</div>
</div>
```

### Two columns

Get two columns starting at desktops and scaling to large desktops.

```html
<div class="row mb-3 text-center">
  <div class="col-md-8 themed-grid-col">.col-md-8</div>
  <div class="col-md-4 themed-grid-col">.col-md-4</div>
</div>
```

### Full width, single column

No grid classes are necessary for full-width elements.

### Two columns with two nested columns

Per the documentation, nesting is easy—just put a row of columns within an existing column. This gives you two columns starting at desktops and scaling to large desktops, with another two (equal widths) within the larger column.

At mobile device sizes, tablets, and down, these columns and their nested columns will stack.

```html
<div class="row mb-3 text-center">
  <div class="col-md-8 themed-grid-col">
    <div class="pb-3">.col-md-8</div>
    <div class="row">
      <div class="col-md-6 themed-grid-col">.col-md-6</div>
      <div class="col-md-6 themed-grid-col">.col-md-6</div>
    </div>
  </div>
  <div class="col-md-4 themed-grid-col">.col-md-4</div>
</div>
```

### Mixed: mobile and desktop

The Bootstrap v5 grid system has six tiers of classes: xs (extra small, this class infix is not used), sm (small), md (medium), lg (large), xl (x-large), and xxl (xx-large). You can use nearly any combination of these classes to create more dynamic and flexible layouts.

Each tier of classes scales up, meaning if you plan on setting the same widths for md, lg, xl, and xxl, you only need to specify md.

```html
<div class="row mb-3 text-center">
  <div class="col-md-8 themed-grid-col">.col-md-8</div>
  <div class="col-6 col-md-4 themed-grid-col">. col-6 .col-md-4</div>
</div>

<div class="row mb-3 text-center">
  <div class="col-6 col-md-4 themed-grid-col">.col-6 .col-md-4</div>
  <div class="col-6 col-md-4 themed-grid-col">.col-6 .col-md-4</div>
  <div class="col-6 col-md-4 themed-grid-col">.col-6 .col-md-4</div>
</div>

<div class="row mb-3 text-center">
  <div class="col-6 themed-grid-col">.col-6</div>
  <div class="col-6 themed-grid-col">.col-6</div>
</div>
```

### Mixed: mobile, tablet, and desktop

```html
<div class="row mb-3 text-center">
  <div class="col-sm-6 col-lg-8 themed-grid-col">.col-sm-6 .col-lg-8</div>
  <div class="col-6 col-lg-4 themed-grid-col">.col-6 .col-lg-4</div>
</div>

<div class="row mb-3 text-center">
  <div class="col-6 col-sm-4 themed-grid-col">.col-6 .col-sm-4</div>
  <div class="col-6 col-sm-4 themed-grid-col">.col-6 .col-sm-4</div>
  <div class="col-6 col-sm-4 themed-grid-col">.col-6 .col-sm-4</div>
</div>
```

### Gutters

With `.gx-*` classes, the horizontal gutters can be adjusted.

```html
<div class="row row-cols-1 row-cols-md-3 gx-4 text-center">
  <div class="col themed-grid-col">
    <code>.col</code> with <code>.gx-4</code> gutters
  </div>
  <div class="col themed-grid-col">
    <code>.col</code> with <code>.gx-4</code> gutters
  </div>
  <div class="col themed-grid-col">
    <code>.col</code> with <code>.gx-4</code> gutters
  </div>
  <div class="col themed-grid-col">
    <code>.col</code> with <code>.gx-4</code> gutters
  </div>
  <div class="col themed-grid-col">
    <code>.col</code> with <code>.gx-4</code> gutters
  </div>
  <div class="col themed-grid-col">
    <code>.col</code> with <code>.gx-4</code> gutters
  </div>
</div>
```

Use the `.gy-*` classes to control the vertical gutters.

```html
<div class="row row-cols-1 row-cols-md-3 gy-4 text-center">
  <div class="col themed-grid-col">
    <code>.col</code> with <code>.gy-4</code> gutters
  </div>
  <div class="col themed-grid-col">
    <code>.col</code> with <code>.gy-4</code> gutters
  </div>
  <div class="col themed-grid-col">
    <code>.col</code> with <code>.gy-4</code> gutters
  </div>
  <div class="col themed-grid-col">
    <code>.col</code> with <code>.gy-4</code> gutters
  </div>
  <div class="col themed-grid-col">
    <code>.col</code> with <code>.gy-4</code> gutters
  </div>
  <div class="col themed-grid-col">
    <code>.col</code> with <code>.gy-4</code> gutters
  </div>
</div>
```

With `.g-*` classes, the gutters in both directions can be adjusted.

```html
<div class="row row-cols-1 row-cols-md-3 g-3 text-center">
  <div class="col themed-grid-col">
    <code>.col</code> with <code>.g-3</code> gutters
  </div>
  <div class="col themed-grid-col">
    <code>.col</code> with <code>.g-3</code> gutters
  </div>
  <div class="col themed-grid-col">
    <code>.col</code> with <code>.g-3</code> gutters
  </div>
  <div class="col themed-grid-col">
    <code>.col</code> with <code>.g-3</code> gutters
  </div>
  <div class="col themed-grid-col">
    <code>.col</code> with <code>.g-3</code> gutters
  </div>
  <div class="col themed-grid-col">
    <code>.col</code> with <code>.g-3</code> gutters
  </div>
</div>
```

### Containers

Additional classes added in Bootstrap v4.4 allow containers that are 100% wide until a particular breakpoint. v5 adds a new `xxl` breakpoint.

```html
<div class="container themed-container text-center">.container</div>
<div class="container-sm themed-container text-center">.container-sm</div>
<div class="container-md themed-container text-center">.container-md</div>
<div class="container-lg themed-container text-center">.container-lg</div>
<div class="container-xl themed-container text-center">.container-xl</div>
<div class="container-xxl themed-container text-center">.container-xxl</div>
<div class="container-fluid themed-container text-center">.container-fluid</div>
```

</details>

## Margin

Margin `m` is the space outside the border of an element. It creates space around an element, pushing other elements away.

- <b>Purpose:</b> It controls the spacing between elements and between an element and its parent or neighboring elements.
- <b>Positive Values:</b> Increase the space.
- <b>Negative Values:</b> Bring elements closer.

<details>
  <summary>Margin</summary>

```HTML
<div id="collapseTwo" class="accordion-collapse collapse" data-bs-parent="#accordionExample">
  <div class="accordion-body">
    <main class="container mb-2">
      <h1>Margin</h1>
      <p class="mt-3">
        Margin <code>m</code> is the space outside the border of an element. It creates space around an element, pushing other elements away.
      </p>
      <ul class="mt-3">
        <li>
          <p>
            <strong>Purpose: </strong> It controls the spacing between elements and between an element and its parent or neighboring elements.
          </p>
        </li>
        <li>
          <p>
            <strong>Positive Values: </strong> Increase the space.
          </p>
        </li>
        <li>
          <p>
            <strong>Negative Values: </strong> Bring elements closer.
          </p>
        </li>
      </ul>

      <div class="container text-center">
        <div class="row">
          <div class="col-md-3 p-2">
            <div class="example rounded-pill pt-3 pb-3 bg-primary text-white" data-bs-toggle="tooltip" data-bs-placement="top" title="Margin: 1rem renders (16px) on all sides">
              m-3
            </div>
          </div>
          <!-- ... (other columns) ... -->
        </div>
      </div>
      <p class="mt-3 mb-3">
        The below table shows complete and comprehensive conversion from <code>rem</code> to <code>px</code>
      </p>
      <div class="list-group">
        <!-- ... (list items) ... -->
      </div>
    </main>
  </div>
</div>
```

</details>

## Padding

Padding `p` is the space inside the border of an element. It creates space between the content of an element and its border.

- <b>Purpose:</b> It controls the spacing between the content and the border of an element.
- <b>Positive Values:</b> Increase the space between content and border.
- <b>Negative Values:</b> Not applicable; padding cannot be negative.

<details>
  <summary>Padding</summary>

```HTML
<div id="collapseTwo" class="accordion-collapse collapse" data-bs-parent="#accordionExample">
  <div class="accordion-body">
    <main class="container mb-2">
      <h1>Padding</h1>
      <p class="mt-3">
        Padding <code>p</code> is the space inside the border of an element. It creates space between the content of an element and its border.
      </p>
      <ul class="mt-3">
        <li>
          <p>
            <strong>Purpose: </strong> It controls the spacing between the content and the border of an element.
          </p>
        </li>
        <li>
          <p>
            <strong>Positive Values: </strong> Increase the space between content and border.
          </p>
        </li>
        <li>
          <p>
            <strong>Negative Values: </strong> Not applicable; padding cannot be negative.
          </p>
        </li>
      </ul>
      <div class="container text-center">
        <div class="row">
          <div class="col-md-3 p-2">
            <div class="example rounded-pill pt-3 pb-3 bg-primary text-white" data-bs-toggle="tooltip" data-bs-placement="top" title="Padding: renders 1rem (16px) on all sides">
              p-3
            </div>
          </div>
          <!-- ... (other columns) ... -->
        </div>
      </div>
      <p class="mt-3 mb-3">
        The below table shows complete and comprehensive conversion from <code>rem</code> to <code>px</code>
      </p>
      <div class="list-group">
        <!-- ... (list items) ... -->
      </div>
      <script>
        var tooltipTriggerList = [].slice.call(document.querySelectorAll('[data-bs-toggle="tooltip"]'));
        var tooltipList = tooltipTriggerList.map(function (tooltipTriggerEl) {
          return new bootstrap.Tooltip(tooltipTriggerEl);
        });
      </script>
    </main>
  </div>
</div>
```

</details>

## Table

In the context of web development and HTML, a table is an HTML element used to organize and display data in a structured format. It consists of rows and columns where data can be placed. The basic structure of an HTML table includes the `<table>` element, which contains one or more `<tr>` (table row) elements. Within each `<tr>`, you define individual cells using `<td>` (table data/cell) elements for regular cells or `<th>` (table header cell) elements for header cells. The latter is typically used in the first row or first column to label the data in the table.

<details>
  <summary>Table</summary>

## Simple Table

```HTML
<table class="table mb-3">
  <thead>
    <tr>
      <th scope="col">#</th>
      <th scope="col">First</th>
      <th scope="col">Last</th>
      <th scope="col">Handle</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th scope="row">1</th>
      <td>Mark</td>
      <td>Otto</td>
      <td>@mdo</td>
    </tr>
    <tr>
      <th scope="row">2</th>
      <td>Jacob</td>
      <td>Thornton</td>
      <td>@fat</td>
    </tr>
    <tr>
      <th scope="row">3</th>
      <td colspan="2">Larry the Bird</td>
      <td>@twitter</td>
    </tr>
  </tbody>
</table>
```

## Colored Tables

```HTML
<table class="table mb-3">
  <thead>
    <tr>
      <th scope="col">Class</th>
      <th scope="col">Heading</th>
      <th scope="col">Heading</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th scope="row">Default</th>
      <td>Cell</td>
      <td>Cell</td>
    </tr>

    <tr class="table-primary">
      <th scope="row">Primary</th>
      <td>Cell</td>
      <td>Cell</td>
    </tr>
    <tr class="table-secondary">
      <th scope="row">Secondary</th>
      <td>Cell</td>
      <td>Cell</td>
    </tr>
    <tr class="table-success">
      <th scope="row">Success</th>
      <td>Cell</td>
      <td>Cell</td>
    </tr>
    <tr class="table-danger">
      <th scope="row">Danger</th>
      <td>Cell</td>
      <td>Cell</td>
    </tr>
    <tr class="table-warning">
      <th scope="row">Warning</th>
      <td>Cell</td>
      <td>Cell</td>
    </tr>
    <tr class="table-info">
      <th scope="row">Info</th>
      <td>Cell</td>
      <td>Cell</td>
    </tr>
    <tr class="table-light">
      <th scope="row">Light</th>
      <td>Cell</td>
      <td>Cell</td>
    </tr>
    <tr class="table-dark">
      <th scope="row">Dark</th>
      <td>Cell</td>
      <td>Cell</td>
    </tr>
  </tbody>
</table>
```

## Stripped Tables

```HTML
<table class="table table-striped mb-3">
  <thead>
    <tr>
      <th scope="col">#</th>
      <th scope="col">First</th>
      <th scope="col">Last</th>
      <th scope="col">Handle</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th scope="row">1</th>
      <td>Mark</td>
      <td>Otto</td>
      <td>@mdo</td>
    </tr>
    <tr>
      <th scope="row">2</th>
      <td>Jacob</td>
      <td>Thornton</td>
      <td>@fat</td>
    </tr>
    <tr>
      <th scope="row">3</th>
      <td colspan="2">Larry the Bird</td>
      <td>@twitter</td>
    </tr>
  </tbody>
</table>
```

## Colored Stripped Tables

```HTML
<table class="table table-dark table-striped mb-3">
  <thead>
    <tr>
      <th scope="col">#</th>
      <th scope="col">First</th>
      <th scope="col">Last</th>
      <th scope="col">Handle</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th scope="row">1</th>
      <td>Mark</td>
      <td>Otto</td>
      <td>@mdo</td>
    </tr>
    <tr>
      <th scope="row">2</th>
      <td>Jacob</td>
      <td>Thornton</td>
      <td>@fat</td>
    </tr>
    <tr>
      <th scope="row">3</th>
      <td colspan="2">Larry the Bird</td>
      <td>@twitter</td>
    </tr>
  </tbody>
</table>
```

## Nested Tables

```HTML
<table class="table table-striped table-bordered mb-3">
  <thead>
    <tr>
      <th scope="col">#</th>
      <th scope="col">First</th>
      <th scope="col">Last</th>
      <th scope="col">Handle</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th scope="row">1</th>
      <td>Mark</td>
      <td>Otto</td>
      <td>@mdo</td>
    </tr>
    <tr>
      <td colspan="4">
        <table class="table">
          <thead>
            <tr>
              <th scope="col">Header</th>
              <th scope="col">Header</th>
              <th scope="col">Header</th>
            </tr>
          </thead>
          <tbody>
            <tr>
              <th scope="row">A</th>
              <td>First</td>
              <td>Last</td>
            </tr>
            <tr>
              <th scope="row">B</th>
              <td>First</td>
              <td>Last</td>
            </tr>
            <tr>
              <th scope="row">C</th>
              <td>First</td>
              <td>Last</td>
            </tr>
          </tbody>
        </table>
      </td>
    </tr>
    <tr>
      <th scope="row">3</th>
      <td>Larry</td>
      <td>the Bird</td>
      <td>@twitter</td>
    </tr>
  </tbody>
</table>
```

## Responsive Tables

```HTML
<div class="table-responsive mb-2">
  <table class="table">
    <thead>
      <tr>
        <th scope="col">#</th>
        <th scope="col">Heading</th>
        <th scope="col">Heading</th>
        <th scope="col">Heading</th>
        <th scope="col">Heading</th>
        <th scope="col">Heading</th>
        <th scope="col">Heading</th>
        <th scope="col">Heading</th>
        <th scope="col">Heading</th>
        <th scope="col">Heading</th>
      </tr>
    </thead>
    <tbody>
      <tr>
        <th scope="row">1</th>
        <td>Cell</td>
        <td>Cell</td>
        <td>Cell</td>
        <td>Cell</td>
        <td>Cell</td>
        <td>Cell</td>
        <td>Cell</td>
        <td>Cell</td>
        <td>Cell</td>
      </tr>
      <tr>
        <th scope="row">2</th>
        <td>Cell</td>
        <td>Cell</td>
        <td>Cell</td>
        <td>Cell</td>
        <td>Cell</td>
        <td>Cell</td>
        <td>Cell</td>
        <td>Cell</td>
        <td>Cell</td>
      </tr>
      <tr>
        <th scope="row">3</th>
        <td>Cell</td>
        <td>Cell</td>
        <td>Cell</td>
        <td>Cell</td>
        <td>Cell</td>
        <td>Cell</td>
        <td>Cell</td>
        <td>Cell</td>
        <td>Cell</td>
      </tr>
    </tbody>
  </table>
</div>
```

</details>

## Buttons

A button is a user interface element that users can interact with to perform actions or trigger events. In web development, buttons are typically created using HTML `<button>` elements and can be styled using CSS to enhance their appearance. Buttons can be clicked or tapped by users to submit forms, navigate to different pages, or trigger other JavaScript functions.

<details>
  <summary>Buttons</summary>

## Default Button

```HTML
<button type="button" class="btn btn-primary flex-fill mb-2 mx-2">
  Primary Button
</button>
<button type="button" class="btn btn-secondary flex-fill mb-2 mx-2">
  Secondary Button
</button>
<button type="button" class="btn btn-success flex-fill mb-2 mx-2">
  Success Button
</button>
<button type="button" class="btn btn-danger flex-fill mb-2 mx-2">
  Danger Button
</button>
<button type="button" class="btn btn-warning flex-fill mb-2 mx-2">
  Warning Button
</button>
<button type="button" class="btn btn-info flex-fill mb-2 mx-2">
  Info Button
</button>
<button type="button" class="btn btn-light flex-fill mb-2 mx-2">
  Light Button
</button>
<button type="button" class="btn btn-dark flex-fill mb-2 mx-2">
  Dark Button
</button>
```

## Small Buttons

```HTML
<button type="button" class="btn btn-primary flex-fill mb-2 mx-2 btn-sm">
  Primary Button
</button>
<button type="button" class="btn btn-secondary flex-fill mb-2 mx-2 btn-sm">
  Secondary Button
</button>
<button type="button" class="btn btn-success flex-fill mb-2 mx-2 btn-sm">
  Success Button
</button>
<button type="button" class="btn btn-danger flex-fill mb-2 mx-2 btn-sm">
  Danger Button
</button>
<button type="button" class="btn btn-warning flex-fill mb-2 mx-2 btn-sm">
  Warning Button
</button>
<button type="button" class="btn btn-info flex-fill mb-2 mx-2 btn-sm">
  Info Button
</button>
<button type="button" class="btn btn-light flex-fill mb-2 mx-2 btn-sm">
  Light Button
</button>
<button type="button" class="btn btn-dark flex-fill mb-2 mx-2 btn-sm">
  Dark Button
</button>
```

## Large Buttons

```HTML
<button type="button" class="btn btn-primary flex-fill mb-2 mx-2 btn-lg">
  Primary Button
</button>
<button type="button" class="btn btn-secondary flex-fill mb-2 mx-2 btn-lg">
  Secondary Button
</button>
<button type="button" class="btn btn-success flex-fill mb-2 mx-2 btn-lg">
  Success Button
</button>
<button type="button" class="btn btn-danger flex-fill mb-2 mx-2 btn-lg">
  Danger Button
</button>
<button type="button" class="btn btn-warning flex-fill mb-2 mx-2 btn-lg">
  Warning Button
</button>
<button type="button" class="btn btn-info flex-fill mb-2 mx-2 btn-lg">
  Info Button
</button>
<button type="button" class="btn btn-light flex-fill mb-2 mx-2 btn-lg">
  Light Button
</button>
<button type="button" class="btn btn-dark flex-fill mb-2 mx-2 btn-lg">
  Dark Button
</button>
```

## Outlined Buttons

```HTML
<button type="button" class="btn btn-outline-primary flex-fill mb-2 mx-2">
  Primary Button
</button>
<button type="button" class="btn btn-outline-secondary flex-fill mb-2 mx-2">
  Secondary Button
</button>
<button type="button" class="btn btn-outline-success flex-fill mb-2 mx-2">
  Success Button
</button>
<button type="button" class="btn btn-outline-danger flex-fill mb-2 mx-2">
  Danger Button
</button>
<button type="button" class="btn btn-outline-warning flex-fill mb-2 mx-2">
  Warning Button
</button>
<button type="button" class="btn btn-outline-info flex-fill mb-2 mx-2">
  Info Button
</button>
<button
  type="button"
  class="btn btn-outline-light flex-fill mb-2 mx-2 text-dark"
>
  Light Button
</button>
<button type="button" class="btn btn-outline-dark flex-fill mb-2 mx-2">
  Dark Button
</button>
```

</details>

## Badges

A badge, on the other hand, is a small visual element used to represent additional information or status. In web development, badges are often implemented using HTML and CSS. They are typically small rectangles or circles with text or icons inside and are commonly used to highlight features, indicate notifications, or display counts (such as the number of unread messages). Bootstrap, a popular front-end framework, provides a set of predefined styles for badges, making it easy to integrate them into a website with a consistent and visually appealing design.

<details>
  <summary>Badges</summary>

```HTML
<span class="badge bg-primary flex-fill mb-2 mx-2">Primary Badge</span>
<span class="badge bg-secondary flex-fill mb-2 mx-2">Secondary Badge</span>
<span class="badge bg-success flex-fill mb-2 mx-2">Success Badge</span>
<span class="badge bg-danger flex-fill mb-2 mx-2">Danger Badge</span>
<span class="badge bg-warning flex-fill mb-2 mx-2">Warning Badge</span>
<span class="badge bg-info flex-fill mb-2 mx-2">Info Badge</span>
<span class="badge bg-light flex-fill mb-2 mx-2 text-dark">Light Badge</span>
<span class="badge bg-dark flex-fill mb-2 mx-2">Dark Badge</span>
```

</details>

## Jumpbotron

A <b>jumpbotron</b> is a prominent and flexible Bootstrap component designed to showcase key content or information on a webpage. It is often used at the top of a page or at the beginning of a major section to grab the user's attention.

Here are some key features and characteristics of a Bootstrap jumbotron:

- <b>Large Header:</b> The jumbotron typically includes a large, attention-grabbing header to convey the main message or purpose of the section.
- <b>Subtext:</b> It often includes a subtext or a brief description below the header to provide additional context or information.
- <b>Background Styling:</b> Jumbotrons have a customizable background, allowing you to use colors, images, or even SVG graphics to enhance the visual appeal.
- <b>Responsive Design:</b> Bootstrap's jumbotron is designed to be responsive, meaning it scales well on different devices and screen sizes.
- <b>Call-to-Action (CTA) Buttons:</b> Jumpbotrons commonly include one or more call-to-action buttons, prompting users to take a specific action.
- <b>Flexible Structure:</b> While the basic structure includes a header and subtext, you can customize the jumbotron to include additional elements like images, icons, or other HTML content.

Here's a breakdown of the components used in the provided example:

- <b>SVG Symbols:</b> These are reusable graphic symbols defined in the SVG <code>&lt;symbol&gt;</code> element. They can be referenced and reused throughout the HTML document.
- <b>Container:</b> The <code>&lt;div class="container"&gt;</code> element is a Bootstrap container that wraps the content, providing spacing and responsiveness. - <b>Jumbotron Styling:</b> The jumbotron is styled using Bootstrap classes such as <code> text-center</code> , <code>bg-body-tertiary</code> , and <code>rounded-3</code>. These classes control the text alignment, background color, and border radius.
- <b>Icons:</b> SVG icons from Bootstrap's icon library <code>bi</code> are used for visual elements. For example, the Bootstrap logo and an arrow-right icon. - <b>Buttons:</b> Bootstrap's button classes (<code>btn</code> , <code>btn-primary</code> , <code>btn-outline-secondary</code> , etc.) are used to create interactive buttons with different styles.
- <b>Responsive Design:</b> The use of Bootstrap's responsive utility classes (<code>col-lg-8</code> , <code>d-inline-flex</code> , etc.) ensures that the content adapts to different screen sizes.
- <b>JS Interaction:</b> The use of Bootstrap's JavaScript for components like the close button <code>btn-close </code> adds interactive elements to the jumbotron.

<details>
  <summary>Jumpbotrun</summary>

## Jumbotron with icon

```HTML
<div class="container">
  <div class="mt-3 mb-3 p-3 text-center">
    <img
      src="https://icons.getbootstrap.com/assets/img/icons-hero.png"
      width="200"
      class="mt-3 mb-3"
      alt=""
    />
    <h1 class="mt-2 mb-3">Jumbotron with icon</h1>
    <p class="fs-5 text-muted mb-3">
      This is a custom jumbotron featuring an SVG image at the top, some longer
      text that wraps early thanks to a responsive <code>.col-*</code> class,
      and a customized call to action.
    </p>
    <div class="d-flex gap-2 justify-content-center">
      <button class="p-3 btn btn-primary rounded-pill">Call to action</button>
      <button class="btn p-3 btn-outline-secondary rounded-pill">
        Secondary link
      </button>
    </div>
  </div>
</div>
```

## Placeholder jumbotron

```HTML
<div class="container my-5">
  <div class="mt-3 mb-3 p-3 text-center text-muted">
    <h1 class="mt-2">Placeholder jumbotron</h1>
    <p class="mx-auto mb-4">
      This faded back jumpbotron is useful for placeholder content. It's also a
      great way to add a bit of context to a page or section when no content is
      available and to encourage visitors to take a specific action.
    </p>
    <button class="btn btn-primary mb-5 p-3 rounded-pill">
      Call to action
    </button>
  </div>
</div>
```

## Full-width jumpbotrun

```HTML
<div class="container py-5 text-center">
  <h1 class="mt-2">Full-width jumpbotrun</h1>
  <p class="mx-auto lead">
    This takes the basic jumpbotrun above and makes its background edge-to-edge
    with a
    <code>.container</code> inside to align content. Similar to above, it's been
    recreated with built-in grid and utility classes.
  </p>
</div>
```

## Basic jumpbotrun

```HTML
<div class="container my-5">
  <div class="p-5 text-center">
    <h1 class="mt-2">Basic jumpbotrun</h1>
    <p class="lead">
      This is a simple Bootstrap jumpbotrun that sits within a
      <code>.container</code>, recreated with built-in utility classes.
    </p>
  </div>
</div>
```

</details>

## Breadcrumbs

Breadcrumbs are a navigation aid that provides users with a trail of links, typically displayed horizontally at the top of a webpage. They indicate the path from the homepage to the current page, aiding users in navigation and improving overall user experience.

### Key Features and Characteristics

- **Navigation Trail:** Breadcrumbs show the hierarchical path from the homepage to the current page, providing users with a clear navigation trail.

- **User Orientation:** Users can easily understand their location within the website's structure and navigate back to higher-level pages.

- **Accessibility:** Breadcrumbs enhance accessibility by providing additional context to screen readers, contributing to a more inclusive user experience.

- **SEO Benefits:** Search engines may use breadcrumb trails to understand the structure of a website, indirectly improving SEO.

### Components

- **Container:** The `<div class="container">` element is a Bootstrap container that wraps the content, providing spacing and responsiveness.

- **Heading:** The `<h1>` element is used to create a heading for the breadcrumbs section.

- **Paragraphs:** `<p>` elements are used for introductory text and feature descriptions.

- **Lists:** `<ul>` and `<ol>` elements are used for listing key features and components.

<details>
  <summary>Breadcrumbs</summary>

## Exhibit A

```HTML
<nav aria-label="breadcrumb">
  <ol class="breadcrumb mt-3">
    <li class="breadcrumb-item"><a href="#">Home</a></li>
    <li class="breadcrumb-item">
      <a href="#">Category</a>
    </li>
    <li class="breadcrumb-item active" aria-current="page">Current Page</li>
  </ol>
</nav>
```

## Exhibit B

```HTML
<nav aria-label="breadcrumb">
  <ol class="breadcrumb mt-3">
    <li class="breadcrumb-item"><a href="#">Home</a></li>
    <li class="breadcrumb-item">
      <a href="#">Products</a>
    </li>
    <li class="breadcrumb-item">
      <a href="#">Category</a>
    </li>
    <li class="breadcrumb-item active" aria-current="page">Product Details</li>
  </ol>
</nav>
```

## Exhibit C

```HTML
<nav aria-label="breadcrumb">
  <ol class="breadcrumb">
    <li class="breadcrumb-item">
      <a class="text-dark text-decoration-none"
        ><svg
          xmlns="http://www.w3.org/2000/svg"
          width="16"
          height="16"
          fill="currentColor"
          class="bi bi-house-door-fill"
          viewBox="0 0 16 16"
        >
          <path
            d="M6.5 14.5v-3.505c0-.245.25-.495.5-.495h2c.25 0 .5.25.5.5v3.5a.5.5 0 0 0 .5.5h4a.5.5 0 0 0 .5-.5v-7a.5.5 0 0 0-.146-.354L13 5.793V2.5a.5.5 0 0 0-.5-.5h-1a.5.5 0 0 0-.5.5v1.293L8.354 1.146a.5.5 0 0 0-.708 0l-6 6A.5.5 0 0 0 1.5 7.5v7a.5.5 0 0 0 .5.5h4a.5.5 0 0 0 .5-.5Z"
          />
        </svg>
        Home</a
      >
    </li>
    <li class="breadcrumb-item">
      <a class="text-dark text-decoration-none"
        ><svg
          xmlns="http://www.w3.org/2000/svg"
          width="16"
          height="16"
          fill="currentColor"
          class="bi bi-box"
          viewBox="0 0 16 16"
        >
          <path
            d="M8.186 1.113a.5.5 0 0 0-.372 0L1.846 3.5 8 5.961 14.154 3.5 8.186 1.113zM15 4.239l-6.5 2.6v7.922l6.5-2.6V4.24zM7.5 14.762V6.838L1 4.239v7.923l6.5 2.6zM7.443.184a1.5 1.5 0 0 1 1.114 0l7.129 2.852A.5.5 0 0 1 16 3.5v8.662a1 1 0 0 1-.629.928l-7.185 2.874a.5.5 0 0 1-.372 0L.63 13.09a1 1 0 0 1-.63-.928V3.5a.5.5 0 0 1 .314-.464L7.443.184z"
          />
        </svg>
        Category</a
      >
    </li>
    <li class="breadcrumb-item active" aria-current="page">
      <svg
        xmlns="http://www.w3.org/2000/svg"
        width="16"
        height="16"
        fill="currentColor"
        class="bi bi-file-earmark-text-fill"
        viewBox="0 0 16 16"
      >
        <path
          d="M9.293 0H4a2 2 0 0 0-2 2v12a2 2 0 0 0 2 2h8a2 2 0 0 0 2-2V4.707A1 1 0 0 0 13.707 4L10 .293A1 1 0 0 0 9.293 0zM9.5 3.5v-2l3 3h-2a1 1 0 0 1-1-1zM4.5 9a.5.5 0 0 1 0-1h7a.5.5 0 0 1 0 1h-7zM4 10.5a.5.5 0 0 1 .5-.5h7a.5.5 0 0 1 0 1h-7a.5.5 0 0 1-.5-.5zm.5 2.5a.5.5 0 0 1 0-1h4a.5.5 0 0 1 0 1h-4z"
        />
      </svg>
      Current Page
    </li>
  </ol>
</nav>
```

</details>

## License

This repository is licensed under the [![MIT License](https://img.shields.io/badge/License-MIT-green.svg)](https://choosealicense.com/licenses/mit/) [MIT License](LICENSE), ensuring flexibility and freedom for developers to use, modify, and distribute the content.

Feel free to explore, contribute, and enhance your Bootstrap skills with this comprehensive cheat sheet.

Happy coding 💻👨🏻‍💻!
