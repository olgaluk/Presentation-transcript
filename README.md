# Presentation-transcript
Hello! Today I want to tell you about the Sass preprocessor.

Before starting to use technologies, it would be good to understand what they are and why they can be useful at all. In the beginning I will talk about what a preprocessor and a CSS preprocessor are. Let's start with the definition. 

A preprocessor is a tool that converts code from one syntax to another. Usually, the input to the preprocessor is code written using syntactic structures that are understandable to this preprocessor. It should be said that the preprocessor can completely replace the syntactic constructions of the language or partially extend them that is add new constructions. As a result, at the output we get the code that the program understands, which will use it after the preprocessor.

If we consider the preprocessors with CSS, the picture is more understandable. CSS preprocessor is an add-on to CSS that adds previously inaccessible features to CSS using new syntaxes. The main task of the preprocessor is to provide convenient syntactic constructions for the developer to simplify and thereby speed up the development and support of styles in projects. CSS preprocessors translate code written using a preprocessor language into pure and valid CSS code.

What are CSS preprocessors?

There are three popular preprocessors:

- Less
- Sass (SCSS)
- Stylus

Next, I will discuss in more detail only about one of them.

I have formed a Google trend chart requests for preprocessors. As you can see, Sass has been in first place for five years. I chose Sass because of its flexibility and breadth of possibilities. So, the Sass preprocessor is the most powerful of the CSS preprocessors. It has a large developer community. Founded in 2007 as a module for HAML and written in Ruby. The possibilities of the preprocessor itself are expanded by the multi-functional library Compass.

What is the use of preprocessors?

With the help of preprocessors, you can write code:

- Readability for humans
- Structured and logical
- Productivity
- Ease of use

The syntax without nesting in CSS is complex, for visual perception. In addition, you need to remember the name of the parent when nesting.

The most popular functionality of any CSS preprocessor is the ability to nest selectors into each other. When using preprocessors, you can put one selector in another, and another in a third, getting something similar to the table of contents of the book.

Speaking quite briefly, using Mixins, you can make the code reusable. This helps to avoid helper classes in markup or duplication of properties from selector to selector.

Using preprocessors has become easier than before. You just need to install a program that will monitor for preprocessor files, and if they change, they will compile the contents of these files into pure CSS code.

It has two syntaxes:

- Sass - simplified CSS syntax. Considered obsolete. Provides a more short way to work with CSS. Files used by this syntax have the extension .sass.

- SCSS (Sassy CSS) - based on standard CSS syntax. This is an extended CSS syntax. This means, that every valid CSS style sheet is a valid SCSS file. This syntax is improved by the Sass functionality described later. Files using this syntax have the extension .scss.

Further I will give examples and consider only the syntax of SCSS.

Nesting

Sass will let you nest your CSS selectors as in the visual HTML hierarchy.
This is a great way to make your CSS file more readable. When you generate a CSS file, you will get something like this at the output.

Partials

You can create partial Sass files that contain small pieces of CSS, which can be used in other Sass files. A partial is simply a Sass file named with a leading underscore. Sass partials are used with the @import directive.

Import

You can import modules using the @import directive, as shown in the example. The directive must write a file name, hyperlink, or any other path.
Ways to divide the code into modules in CSS and Sass are different. When you break the CSS code into smaller style sheets, you need to run a separate HTTP request to load each table. In Sass, the @import directive loads the module code immediately, so the result is always a single CSS file.
When the CSS is generated you will get.

Variables

Variables are important functionality that is not present in CSS. Style sheets use a lot of repetitions, so it's very useful to be able to set a variable once and then reference it.
To create a variable in CSS, you need to use the $symbol.
From the example, we see that after creating variables, we can insert them instead of values. And now you can change the color and font of all the elements where our variables are inserted in one place.
When the CSS is generated you will get.

Mixins

Mixins give you the ability to create groups of CSS declarations that you will have to reuse. It is good to use mixins for vendor prefixes as shown in the example.

Extend

This is one of the most useful features of Sass. Using the @extend directive, you can inherit CSS property sets from one selector to another. A placeholder class - a special type of classes that is displayed only, when using the extension, this will keep your compiled CSS clean. The example shows how to use it.
Each of these classes gets CSS properties of the first placeholder class. This will help you avoid writing many classes in HTML elements.

So, we looked at the basics of working with Sass. Thank you for your attention.
