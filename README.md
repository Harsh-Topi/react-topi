# react-topi - boilerplate code for react projects.

Special thanks to @Dallas-Ng for coming up with the folder structure. I really liked how he structured his React projects, so I decided to make a boilerplate for myself.

## How to run the project

```sh
npm install
npm run dev
```

## Folder structure

```sh
client/
    ├── .github                 # Github actions YAML files
    ├── .next                   # Next generation files
    ├── components              # All components
    ├── node_modules
    ├── pages                   # All pages (routes) in the application
    ├── public                  # Any static content that needs to be served
    ├── styles                  # Top level stylesheets
    ├── .babelrc                # Babel Settings
    ├── .eslintignore
    ├── .eslintrc.json
    ├── .gitignore
    ├── .prettierignore
    ├── .prettierrc.json
    ├── .next.config.js         # Next.js settings
    ├── package-lock.json       # Packaged dependencies managed by NPM
    ├── package.json            # Project settings
```

## Naming / Directory Conventions

```sh
# For components, files are to follow this structure
components/
    ├── [FolderNameInCaps]
    |       ├──[component-name.jsx]     # Component (Component name must be in lowercase kebab case.)
    |       ├──[index.js]               # Import/Export for the components
    |       └──[styles.js]              # Styled components assets for the specific component
    |   # Example
    ├── Login
    |       ├──Sign-Up
    |       |   ├──index.js
    |       |   ├──sign-up.jsx
    |       |   └──styles.js
    |       └──Sign-In
    |           ├──index.js
    |           ├──sign-in.jsx
    |           └──styles.js
    |
    └── [OtherComponents]
```

#### Naming

1. Components parent folders are always to be in `Pascal-Kebab` format
2. The components itself, will be in `lowercase-kebab` format
3. The "styles.js" file must only be named as exactly that.

## Linter

I have a main linter (eslint) and a code formatter (prettier). The configuration for both are included into the development files already. If you are using VScode, it should piroritize those files over your existing settings. If you are using a different editor, please check if it is linting properly.

#### How to run the linters

```sh
# eslint
npx eslint ./

# prettier (this can be done via format on save option in your editor)
npx prettier ./components
npx prettier ./pages
```
