![Group 60](https://user-images.githubusercontent.com/44784345/209415574-f2543b13-db38-429d-9623-0da082d7b490.png)

# React + MUI + Typescript
Build your react frontend with MUI and typescript preconfigured (frontend only)

## Available Scripts

In the project directory, you can run:

### `npm start`

Runs the app in the development mode.\
Open [http://localhost:3000](http://localhost:3000) to view it in the browser.

The page will reload if you make edits.\
You will also see any lint errors in the console.

### `npm test`

Launches the test runner in the interactive watch mode.\
See the section about [running tests](https://facebook.github.io/create-react-app/docs/running-tests) for more information.

### `npm run build`

Builds the app for production to the `build` folder.\
It correctly bundles React in production mode and optimizes the build for the best performance.

The build is minified and the filenames include the hashes.\
Your app is ready to be deployed!

See the section about [deployment](https://facebook.github.io/create-react-app/docs/deployment) for more information.

### `npm run eject`

**Note: this is a one-way operation. Once you `eject`, you can’t go back!**

If you aren’t satisfied with the build tool and configuration choices, you can `eject` at any time. This command will remove the single build dependency from your project.

Instead, it will copy all the configuration files and the transitive dependencies (webpack, Babel, ESLint, etc) right into your project so you have full control over them. All of the commands except `eject` will still work, but they will point to the copied scripts so you can tweak them. At this point you’re on your own.

You don’t have to ever use `eject`. The curated feature set is suitable for small and middle deployments, and you shouldn’t feel obligated to use this feature. However we understand that this tool wouldn’t be useful if you couldn’t customize it when you are ready for it.

## Learn More

You can learn more in the [Create React App documentation](https://facebook.github.io/create-react-app/docs/getting-started).

To learn React, check out the [React documentation](https://reactjs.org/).


## Common errors
The error message "Cannot find module 'react/jsx-runtime' or its corresponding type declarations" usually occurs when your code is missing the required dependencies or there is an issue with your project's setup. Here are a few steps you can follow to resolve this error:

1. Install the required dependencies: Make sure you have the necessary dependencies installed in your project. In this case, it seems like you're missing the `react/jsx-runtime` module. You can install it by running the following command in your project's root directory (where your `package.json` file is located):
   ```bash
   npm install react-jsx-runtime
   ```
   or if you're using Yarn:
   ```bash
   yarn add react-jsx-runtime
   ```

2. Check your import statement: Ensure that your import statement for `react/jsx-runtime` is correct. It should look like this:
   ```javascript
   import { jsx } from 'react/jsx-runtime';
   ```

3. Verify your TypeScript configuration: If you're using TypeScript, make sure that your `tsconfig.json` file is properly configured. Ensure that the `compilerOptions` section includes the necessary settings for JSX, like `"jsx": "react-jsx"` or `"jsxFactory": "jsx"`, depending on your setup.

4. Clear your package cache: Sometimes, the issue can be related to the package cache. Try clearing it by running the following command:
   ```bash
   npm cache clean --force
   ```
   or with Yarn:
   ```bash
   yarn cache clean
   ```

5. Restart your development server: If you're using a development server, try restarting it to ensure that the changes take effect.

By following these steps, you should be able to resolve the "Cannot find module 'react/jsx-runtime'" error and get your project running successfully.
