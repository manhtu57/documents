# This is checklist after implementation

## 📄 Documents/Tickets/Requirements
- [ ] Adding ticket URL in Pull Request
- [ ] Adding design file (XD, Figma, ...) in Pull Request
- [ ] Adding information of API in Pull Request


## 💻 Coding

### General Standard
- [ ] Code is not repeated or duplicated
- [ ] Avoid using negative comparison
- [ ] Avoid using magic number
- [ ] Avoid reassigning the function parameter inside function (Keeping function parameters are immutated)
- [ ] With variable won't change use CONST
- [ ] Use strict comparison === (!==) instead of weak comparison ==
- [ ] Splitting function when it is too long or more than one main functions
- [ ] Passing only those necessary params into function instead of passing the whole object
- [ ] Make sure all the environment config files are updated
- [ ] Use verb when naming a function which perform an action
- [ ] Use noun when naming a property/variable
- [ ] Use prefix `is` / `has` with boolean variable
- [ ] Avoid negatively named boolean variables
- [ ] Avoid naming variables with unclear meanings (res, check, ...)


### PHP
- [ ] Using `NOWDOC` or  `single quote` instead of `double quote`, `HEREDOC`
- [ ] Using PHP Doc for class/function/variable with [standard](https://2tbsp.com/sites/default/files/articles/phpdoc_cheatsheet.pdf)
- [ ] Using bcmath of PHP to avoid floating-point when calculate numbers
- [ ] Use SensitiveParameterValue to store sensitive data to avoid backtrace to leak sensitive data
- [ ] Ensure that data values are safely passed to JavaScript by using the 'data-' attribute approach to separate concerns and prevent potential security vulnerabilities.
- [ ] Using gizzle libary when calling API
- [ ] Include basedate if needed
- [ ] Cached response API if needed
- [ ] Using transaction when handle more query CRUD

### Symfony
- [ ] Using `Attribute` instead of `Annotation`

### Javascript
- [ ] Use let, const instead of var
- [ ] Aware floating point when cast others type to number (with JS use Number() to reserve the floating point)

### ReactJS
- [ ] Applying Slice (react-tookit) when handle state, dispact on Module files
- [ ] Avoid re-rendering with list of components by providing a key attribute
- [ ] Using typescript `.tsx`
- [ ] No state updates in loop
- [ ] Checking warning when development

### HTML/CSS
- [ ] Set width, height, color, font, image same with design
- [ ] Avoid using inline CSS
- [ ] Checking responsive in SP/APP
- [ ] Changing query version of css file (*.css?20301231)
- [ ] Add noopener noreferrer when includes external link in a tag.

### MySQL
- [ ] Use DATETIME type instead of TIMESTAMP
- [ ] Avoid using default value 0000-00-00 00:00:00, use NULL
- [ ] Use TINYINT for boolean only or for integer which only have 1,0
- [ ] Check if column is existed before adding/deleting column
- [ ] Avoid using OR in WHERE clause
- [ ] Avoid N+1 Query


## 🐞 Testing

### Unit Tests
- [ ] Write UT for common functions (services, helpers, ...)

### Intergation Tests
- [ ] Checking empty data or edge case
- [ ] Checking double click
- [ ] Checking on safari, real device if needed

## 🔐 Security
- [ ] Do not logging sensitive data (Personal Identifiable Information, keychain, password, hash, ...)
- [ ] Escape URL, raw data in template code
- [ ] Clear `console.log()`, `var_dump()` or similar function after implementation


## Others
- [ ] With 3rd library, include the copyright to avoid being sued
