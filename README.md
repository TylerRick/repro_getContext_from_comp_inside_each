This is a minimal reproduction of a "Function called outside component initialization" error that I
ran into in a real app, and my various attempts to figure out the cause and resolution of the error.

More information can be found in this question:
<https://stackoverflow.com/questions/64152594/should-svelte-libraries-include-external-svelte-in-rollup-config-js-func>

To build this app:

1. `npm i`

1. Build its dependency:

    ```
    cd packages/my-new-component/
    npx rollup -c -w
    ```

1. Build the app:

    ```
    npx rollup -c -w
    ```
