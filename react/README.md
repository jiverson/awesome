# React

[React](https://reactjs.org/)  

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
