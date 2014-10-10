## Setup

In order to run this project you need JDK 6 or 7 with $JAVA_HOME defined in your environment. You will also need to have marketplace running (the test expects a base URL of https://localhost:8443/marketplace).


## Run All Tests

```
./gradlew test
```

The task will stop on the first test failure. To run all test tasks without stopping on failures, use:

```
./gradlew test --continue
```

## Run a Single Test

The tests are organized by REST Resource (Agency, Category, Listing, etc). To run a test for a single resource prefix the resource name with test. For example to run the test for Category use the following command:

```
./gradlew testCategory
```

## Open a Test in the Editor

To edit/run the test from the GUI prefix the resouce name with edit. For example to edit the test for Category use:

```
./gradlew editCategory
```

## List All Resources

```
./gradlew list
```