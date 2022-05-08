# Serenity-lint
A modular approach to setup an easily modfiable and shareable lint ruleset linter and prettier in a few minutes.

The default ruleset is RATHER STRICT and you should not hesitate to relax rules that are too restrictive for your usage.

#Dependencies
## Vanilla
@typescript-eslint/eslint-plugin 
@typescript-eslint/parser 
eslint 
eslint-config-prettier
prettier

## With Jest
@types/jest
eslint-plugin-jest 
jest 

# Installation
Put the following files and directories in your projet root
```
- .eslint <-- ruleset directory
- .eslintignore
- .eslintrc.js <-- Lint config file entrypoint
- .prettierignore
- .prettierrc.json <-- Prettier config file entrypoint
```

# Additional jest configuration
To enable rules in .spec.ts files uncomment the jest part in .eslintrc.js, adapt file matching as needed.


# Scripts
In your package.json 
```json
"scripts": {
    ...
    "prettier": "prettier --write src",
    "lint": "eslint ./src/*",
}
```

# Usage 
Run the commands (eg with npm)  
```npm run lint```  
or  
```npm run prettier```  
