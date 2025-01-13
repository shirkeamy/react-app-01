# Getting Started with Create React App

This project was bootstrapped with [Create React App](https://github.com/facebook/create-react-app).

# Issues and its resolution

Once we create an application usign `create-react-app` using template of `typescript` it gives us error as below 

![alt text](./imgs/image.png)

To resolve this issue we have to do some steps like
1. Add `tsconfig.json` file with below code
    ```
    {
        "compilerOptions": {
            "target": "es5",
            "lib": [
                "dom",
                "dom.iterable",
                "esnext"
            ],
            "allowJs": true,
            "skipLibCheck": true,
            "esModuleInterop": true,
            "allowSyntheticDefaultImports": true,
            "strict": true,
            "forceConsistentCasingInFileNames": true,
            "noFallthroughCasesInSwitch": true,
            "module": "commonjs",
            "moduleResolution": "node",
            "resolveJsonModule": true,
            "isolatedModules": true,
            "noEmit": true,
            "jsx": "react-jsx"
        },
        "include": ["./src/**/*"],
        "exclude": [
            "node_modules"
        ],
        "typeAcquisition": {
            "include": ["jest"]
        }
    }
2. Install `web-vitals` with version `^3.4.0`
    ```
    npm install web-vitals@3.4.0
3. Need to install some dependancies
    ```
    npm install --save-dev @types/react
    npm install --save-dev @types/react-dom
4. Remove test file for now


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

## Learn More

You can learn more in the [Create React App documentation](https://facebook.github.io/create-react-app/docs/getting-started).

To learn React, check out the [React documentation](https://reactjs.org/).
