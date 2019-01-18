# React

[React](https://reactjs.org/)  
[mobx-state-tree](https://github.com/mobxjs/mobx-state-tree)  

## Create react app  
```bash
npx create-react-app my-app --typescript
npm i --save-dev prettier rxjs-tslint-rules tslint tslint-config-prettier tslint-react
```

### Config setup  
`package.json` add the following to scripts:
```
"tslint-check": "tslint-config-prettier-check ./tslint.json"
```

### Folder structure  
```
my-app/
├── README.md
├── node_modules
├── .gitignore
├── .prettierignore
├── .prettierrc
├── package.json
├── tsconfig.json
├── tslint.json
├── public/
│   ├── favicon.ico
│   ├── index.html
│   └── manifest.json
└── src/
    └── assets/
        └── logo.svg
    └── components/
    ├── App.css
    ├── App.tsx
    ├── App.test.ts
    ├── index.css
    ├── index.tsx
    └── serviceWorker.ts
```

### Add sass
```npm i node-sass```
