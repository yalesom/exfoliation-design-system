> Exfoliation relies on the [Square360 Fundamental Toolkit][toolkit] to establish [breakpoints][bp].

[Max-width][layout] for the main content area is 1344px. Headers and footers typically span the full width of the browser.

# Columns

Column structures vary by breakpoint and are designated as follows:

| Breakpoint            | Width           | Columns | Gutter | Outer Margin |
| --------------------- | --------------- | ------- | ------ | ------------ |
| _Default_             | 0px - 479px     | 4       | 20px   | 20px         |
| **Phone, landscape**  | 480px - 719px   | 4       | 20px   | 20px         |
| **Tablet, portrait**  | 720px - 799px   | 6       | 20px   | 20px         |
| **Tablet, landscape** | 800px - 1023px  | 9       | 20px   | 40px         |
| **Desktop**           | 1024px - 1279px | 12      | 20px   | 40px         |
| **Big desktop**       | 1280px -        | 12      | 20px   | 40px         |

[toolkit]: https://bitbucket.org/sq360_sysadmin/s360-fundamental-toolkit
[bp]: https://bitbucket.org/sq360_sysadmin/s360-fundamental-toolkit/src/master/scss/core/_breakpoints.scss
[layout]: https://bitbucket.org/sq360_sysadmin/yale-som-theme/src/master/scss/core/_layout.scss
