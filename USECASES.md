# Use Cases

## Generate steps file

**Story**:

```
As a developer with Cucumber language knowledge
I want to quickly generate steps file from my feature file
So that I get a head-start on using GoBDD
```

Scenario 1:

```feature
Given a *.feature file is open
When I open a context menu
Then there is an option to "Generate a steps file"
```

Scenario 2:

```feature
Given an valid *.feature file is open
When I select the "Generate a steps file" in the context menu
Then a new *_steps.go file is generated in a default location
And the filename matches the feature file name
And it contains a scaffolding code with the steps corresponding to the feature file
And the code can compile without errors
```

## Navigate to step implementation

**Story**:

```
As a developer
I want to quickly go to a step implementation from my feature file
So that I have a good experience using GoBDD
```

Scenario 1:

```feature
Given a *.feature file is open
And the cursor is on any step definition
And the step's implementation exists
When I select the default action "Go to Implementations"
Then it will navigate to the step's implementation
```

NOTE: Use existing keyboard bindings.

Scenario 2:

```feature
Given a *.feature file is open
And the cursor is on any step definition
And the step's implementation does not exist
When I select the default action "Go to Implementations"
Then it will show me a warning
And the warning message will contain a scaffolding code to implement the step
And there will be a button to copy this into the clipboard
```

## Navigate to step definition

**Story**:

```
As a developer
I want to quickly go to a step definition from my step implementation file
So that I have a good experience using GoBDD
```

Scenario 1:

```feature
Given a *_test.go file is open
And the cursor is on any step implementation function
And the step's definition exists in any feature file
When I select the default action "Go to Definition"
Then it will navigate to the step's definition
```

NOTE: Use existing keyboard bindings.

Scenario 2:

```feature
Given a *_test.go file is open
And the cursor is on any step implementation function
And the step's definition does not exist in any feature file
When I select the default action "Go to Implementations"
Then it will show me a warning
```
