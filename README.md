This project reproduces a WebStorm bug when importing JS modules in a TypeScript project with `allowJs: true`.

To see the issue, open the project in WebStorm 2021.3.3 and go to `src/components/foo/Foo.js`.
The module `providers/utils` is marked as not installed, but you can still jump to it with Cmd+Click.
Visual Studio Code does not have this issue, and the project compiles and works in general.

For more info, see: https://youtrack.jetbrains.com/issue/WEB-40623
