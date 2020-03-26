# vscode-extension

VSCode Extension for [go-bdd](https://github.com/go-bdd/gobdd)

Used an Empty VSCode Extension with Tests sample from <https://github.com/microsoft/vscode-extension-samples/tree/master/helloworld-test-sample>.

## Running the Sample

* Run `npm install` in terminal to install dependencies
* Run the `Run Extension Tests` target in the Debug View. This will:
  * Start a task `npm: watch` to compile the code
  * Run the extension integration test in a new VS Code window

## CI/CD

We use GitHub Actions for CI/CD.

See [Publishing Extensions](https://code.visualstudio.com/api/working-with-extensions/publishing-extension) for more information.

## Technology Used

* npm
* node
* VSCode
* TypeScript
* GitHub Actions
