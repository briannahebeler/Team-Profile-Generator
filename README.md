# Team Profile Generator

## Description

A Node CLI that generates profiles for each member of a software engineering team. This command line application accepts user information to generate an HTML webpage that displays a team roster of summaries for each team member in order for the user to quick;y access emails and GitHub profiles for all team members.

## Directions from class repo:

Use unit tests to help build necessary classes. 
It is recommended that you follow this workflow:
1. Run tests
2. Create or update classes to pass a single test case
3. Repeat
🎗 Remember, you can run the tests at any time with `npm run test`

It is recommended that you start with a directory structure that looks like this:
```
lib/           // classes and helper code
output/        // rendered output
templates/     // HTML template(s)
test/          // jest tests
  Employee.test.js
  Engineer.test.js
  Intern.test.js
  Manager.test.js
app.js         // Runs the application
```

### Hints

* You will want to make your methods as pure as possible. This means try to make your methods simple so that they are easier to test.

* The different employee types should all inherit some methods and properties from a base class of `Employee`.

* In your HTML template files, you may want to add a placeholder character that helps your program identify where the dynamic markup begins and ends.

### Classes
The project must have the these classes: `Employee`, `Manager`, `Engineer`,
`Intern`. The tests for these classes in the `tests` directory must all pass.

The first class is an `Employee` parent class with the following properties and
methods:
  * name
  * id
  * email
  * getName()
  * getId()
  * getEmail()
  * getRole() // Returns 'Employee'
The other three classes will extend `Employee`. 

In addition to `Employee`'s properties and methods, `Manager` will also have:
  * officeNumber
  * getRole() // Overridden to return 'Manager'

In addition to `Employee`'s properties and methods, `Engineer` will also have:
  * github  // GitHub username
  * getGithub()
  * getRole() // Overridden to return 'Engineer'

In addition to `Employee`'s properties and methods, `Intern` will also have:
  * school 
  * getSchool()
  * getRole() // Overridden to return 'Intern'

### Roster output
The project must generate a `team.html` page in the `output` directory, that displays a nicely formatted team roster. Each team member should display the following in no particular order:
  * Name
  * Role
  * ID
  * Role-specific property (School, link to GitHub profile, or office number)

## Bonus
* Use validation to ensure that the information provided is in the proper expected format.
* Add the application to your portfolio.

## Video
* A video demonstrating the entirety of the app's functionality