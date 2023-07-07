<details>
<summary>Mobile First vs Desktop First Designs</summary>

- Should we begin writing css for desktop or mobile?
- Traditionally, desktop first is followed, with responsiveness done afterwards.
- Media queries are used for responsiveness.
- Desktop first media queries test against max width, mobile first uses min width.

- Mobile first forces us to really think about the mobile experience by reducing our apps to the absolute essentials.
</details>

<details>
<summary>Max-width vs min-width</summary>

- Desktop first: we might start writing css for screens 1200px+ width.
    - Desktop involves max-width queries i.e. "this style applies up until a max screen width of Xpx"
    - In these media queries we just override global css at different breakpoints.
    - If a screen size fits into 2 breakpoints (i.e. 500px fits into 600px breakpoint and 900px breakpoint), both styles apply - so the last takes precedence (cascade).

- Mobile first: we write css for screens <600px width
    - Mobile involves min-width queries i.e. "this style applies as long as the screen size is larger than Xpx"
    - This means a 500px screen does not apply the styles meant for things above 600px.

    - pros
        - 100% optimised for mobile experience
        - reduces websites and apps to the absolute essentials
        - results in smaller, faster and more efficient products
        - prioritizes content over aesthetic design(?)
    - cons
        - desktop version might feel overly empty and simplistic
        - more difficult and counterintuitive to develop
        - less creative freedom, making it more difficult to create distinctive products
        - Clients want to see a desktop version of the site as a prototype
        - Do your users even use the mobile internet? What's the purpose of your website?

- No matter what, both must be kept in mind.
</details>

<details>
<summary>Selecting Breakpoints</summary>

- Bad method - using the widths of popular devices (particularly apply products).
- Good method - grouping popular devices together and figuring out breakpoints.
- Perfect method - Ignore devices and only look at your content and your design. Begin at one size, change screen size until your design breaks and looks stupid (then add a breakpoint) (?).
</details>
