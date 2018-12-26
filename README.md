# Screenplay Pattern with Serenity BDD

This project is a simple demonstration showing the [Screenplay pattern](https://dzone.com/articles/page-objects-refactored-solid-steps-to-the-screenp),
using the [Serenity BDD](http://serenity-bdd.info/#/) library and JUnit.

The web tests you'll find here run against the http://todomvc.com/examples/angularjs/#/ application and are organised by feature in packages under `src/test/java/net/serenitybdd/demos/todos/<pattern name>/features`.

By default the tests run on Chrome, so make sure you have the latest chromedriver instance on your system path.

## PageObjects implementation

These tests use pages and steps defined in src/main/java/net/serenitybdd/demos/todos/pageobjects.

The overall project structure is shown below:

```
+ model
    Domain model classes
+ pages
    PageObjects
+ steps
    Tasks and assertions performed by the "user"
```

## Running the project

To run the project you'll need JDK 1.8 and Maven installed.

### Page Object and JUnit

The demo covers the integration of Serenity BDD, Page Objects and JUnit.

To run it, execute:

```
mvn clean verify -Ppageobjects
```

## Reporting

The Serenity reports will be generated in the `target/site/serenity` directory.
