# Storybook Design System Documentation

(with **React**)

This project aims to fully understand the capabilities and limitations of Storybook.js and what it can provide for both designers and developers alike.

# The Why

> Storybook is a tool for UI development. It makes development faster and easier by isolating components. This allows you to work on one component at a time. You can develop entire UIs without needing to start up a complex dev stack, force certain data into your database, or navigate around your application.

Storybook has been a great addition to the teams I've worked for in professional settings. Many times have I been asked _"How do I implemented XYZ?"_ or _"Does ABC support this other use case?"_. Having the ability to interact in a live demo-like setting, even at the isolated component level, has excelled us leaps and bounds ahead of where we were even a few years ago. Providing visual testing, component integration testing, and even some contextual/conditional render testing allows for my frontend software engineers to take a back seat and let the design system do the work of defining the rails. Documentation is key to making developers' lives easier - and Storybook is the solution right now.

> Documentation is crucial for design system adoption. It consolidates usage guidelines to help developers, designers, PMs and other stakeholders ship predictable UIs.

# The How

Whatever is being built should have a proper design system behind it to keep a consolidated look and feel. Many times have I come across a professional setting where teams were developing in silos or teams found disparate 3rd-party solutions. External solutions are fine - don't get me wrong - but there should be a single source a truth if everyone is going to be working toward the same goal.

> Storybook helps you **document** components for reuse and automatically **visually test** your components to prevent bugs. Extend Storybook with an ecosystem of **addons** that help you do things like fine-tune responsive layouts or verify accessibility.

> Storybook integrates with most popular JavaScript UI frameworks and (experimentally) supports server-rendered component frameworks

Components allow us to consolidate in a way that's reusable and expandible to future use cases. There are four categories[<sup>1</sup>](https://medium.com/eightshapes-llc/documenting-components-9fe59b80c015) that a component can be documented into:

1. **Description** - details exactly what a component is for
1. **Examples** - coded references for different variants
1. **Design reference** - guides for when to use components
1. **Code reference** - details the inner workings and expectations

Whichever UI framework is used, you can add Storybook on top of it (some already do out of the box, which is great). There are times however where the default Storybook does not provide _all_ of the solutions natively. This is where addons come in!

# Addons

The Docs addon is critical for helping developers, especially those in junior roles aspiring to wet their feet in the visual side of frontend enginering.

The addons[<sup>2</sup>](https://github.com/storybookjs/storybook/#addons) this project aims to use are:

-   **a11y**: Accessibility testing and awareness (for developer ease-of-use)
-   **docs**: Higher quality documentation (for developer awareness)
-   **links**: Links between stories (for integration testing)
-   **storyshots**: Snapshot testing (for backwards compatibility testing)
-   **measure**: Inspect layouts to conform to Design Tools (e.g., Figma, Framer, Adobe XD)
-   among others from default `npx sb init`...
