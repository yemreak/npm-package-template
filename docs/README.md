# npm-package-template

## Getting Started

To get started with this npm package template, follow these steps:

1. Clone the repository to your local machine.
2. Navigate to the project directory.
3. In your `package.json`, use VSCode Find and Replace feature to change all instances of 
	- `mypackage` to your own package name
	- `yemreak` to your own author name
	- ![alt text](assets/SCR-20240427-qoxk.png)
4. Install the dependencies by running the following command:
	```zsh
	npm install
	```
5. To add a new user to npm registry, run:
	```zsh
	npm adduser
	```
6. To publish the package to the **public** npm registry, run:
	```zsh
	npm publish --access public
	```
## `tsconfig.json`

- **Target**: Specifies the version of ECMAScript to use. Set to `ESNext`, which means the latest draft version
- **Module**: Determines the module system, using `ESNext` for the latest
- **OutDir**: The output directory for compiled files is `./out`
- **RootDir**: The root directory containing TypeScript files is `./src`
- **ModuleResolution**: Configured to `Bundler`, indicating that a module bundler handles module resolution
- **esModuleInterop**: Set to `true` to enable interoperability for non-ECMAScript module (ESM) packages
- **ForceConsistentCasingInFileNames**: Ensures that references to filenames maintain consistent casing
- **Strict**: Enables all strict type-checking options
- **SkipLibCheck**: Skips type checking for default library files (`*.d.ts`)
- **ResolveJsonModule**: Allows importing `.json` files
- **SourceMap**: Generates corresponding `.map` files for debugging
- **Declaration**: Emits `.d.ts` files for each corresponding `.ts` file
- **Incremental**: Enables incremental compilation by caching certain file contents
- **StrictNullChecks**: Ensures strict null checking where `null` and `undefined` are handled explicitly
- **Include**: Includes all TypeScript files within `src`, matching the pattern `src/**/*.ts`
- **Exclude**: Excludes files in `node_modules` and all `.spec.ts` files to prevent them from being compiled
