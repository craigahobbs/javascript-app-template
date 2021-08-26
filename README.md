# javascript-template

**javascript-template** is a JavaScript project template for use with
[template-specialize](https://pypi.org/project/template-specialize/).
Generated projects have the following functionality:

- complete build/development experience using [javascript-build](https://github.com/craigahobbs/javascript-build#readme)

- lightweight client-rendered web application using [element-model](https://www.npmjs.com/package/element-model)
  and [schema-markdown](https://www.npmjs.com/package/schema-markdown)

- API documentation with [jsdoc](https://www.npmjs.com/package/jsdoc)

- ready to upload to [npm](https://www.npmjs.com/)

- a license file ([MIT License](https://choosealicense.com/licenses/mit/))

- 100% unit-test code coverage, enforced


## Create a New JavaScript Project

To create a new JavaScript project, clone this repository and render the template using
[template-specialize](https://pypi.org/project/template-specialize/). For example:

```
template-specialize javascript-template/template/ my-package/ \
    -k package "my-package" \
    -k name "John Doe" \
    -k email "johndoe@gmail.com" \
    -k github "johndoe"
```

The template defines the following template variables:

- **package** - the JavaScript package name (e.g., "my-package")

- **name** - the package author's full name (e.g., "John Doe")

- **email** - the package author's email address

- **github** - the package author's GitHub account name (e.g., "johndoe")

- **noapp** (optional) - if true, the web application is omitted


## Development Basics

Generated projects have a complete build/development experience using
[javascript-build](https://github.com/craigahobbs/javascript-build#readme).
It provides commands for running unit tests (with and without code coverage), running static code analysis,
building API documentation, publishing API documentation to GitHub Pages, creating and updating a changelog file,
and publishing the package to npm.

Here are a few basic commands to help you get started. For more detailed documentation, see the
[javascript-build documentation](https://github.com/craigahobbs/javascript-build#readme).

Before any commit, run the **make commit** command to run all tests:

```
make commit
```

To run unit tests, use the **make test** command:

```
make test
```

To run unit tests on a specific unit test, use the **TEST** argument:

```
make test TEST="test name"
```

To run unit tests with code coverage, use the **make cover** command:

```
make cover
```

To publish the application or API documentation to [GitHub Pages](https://pages.github.com/), use the **make gh-pages** command:

```
make gh-pages
```

To create or update a changelog file, use the **make changelog** command:

```
make changelog
```

Finally, to publish to [npm](https://www.npmjs.com/), use the **make publish** command:

```
make publish
```


## Project Structure

The project structure is as follows:

```
|-- LICENSE
|-- Makefile
|-- README.md
|-- index.js
|-- package.json
|-- src
|   |-- my-package
|   |   |-- index.js
|   |   `-- myPackage.js
|   `-- tests
|       `-- testMyPackage.js
`-- static
    `-- index.html
```
