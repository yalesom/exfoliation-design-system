> Exfoliation, through the [Square360 Fundamental Toolkit][toolkit] ("Toolkit"), uses [Susy grid][susy-docs] for on-the-fly grid-math.

For example, `width: span(2 of 8)` will return the width of 2 columns relative to a 8-column space. By default, [page grids][susy] are 12 columns with 20px gutters and a 40px outside margin.

```hint
Most page layouts use **flexbox**, negating many of the core features of Susy (which relies on float). Susy, in our case, simply provides the mixins for our grid-math.
```
[Max-width][layout] for the main content area is 1344px. Headers and footers typically span the full width of the browser.

# Columns
Exfoliation relies on the Toolkit to establish [breakpoints][bp]. Column structures vary by breakpoint and are designated as follows:

| Breakpoint    | Width     | Columns  | Gutter | Outer Margin|
| ------------- | ------------- | ----- | ----- | ----- |
| *Default*   | 0px - 479px  | 4 | 20px  | 20px |
| **Phone, landscape** | 480px - 719px | 4 | 20px  | 20px  |
| **Tablet, portrait** | 720px - 799px | 6 | 20px  | 20px  |
| **Tablet, landscape**  | 800px - 1023px  |  9 | 20px  |  40px  |
| **Desktop** | 1024px - 1279px | 12 | 20px  | 40px  |
| **Big desktop**  | 1280px -   |  12 | 20px  |  40px  |

[toolkit]:https://bitbucket.org/sq360_sysadmin/s360-fundamental-toolkit
[bp]: https://bitbucket.org/sq360_sysadmin/s360-fundamental-toolkit/src/master/scss/core/_breakpoints.scss
[susy-docs]: http://oddbird.net/susy/docs/
[susy]: https://bitbucket.org/sq360_sysadmin/s360-fundamental-toolkit/src/master/scss/core/_susy.scss
[layout]: https://bitbucket.org/sq360_sysadmin/yale-som-theme/src/master/scss/core/_layout.scss
