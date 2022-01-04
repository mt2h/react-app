# GitHub Actions

This project is the continuation of https://github.com/mt2h/github-actions-test of course Github Actions

## Local testing react app

```bash
#create react app
cd project/
sudo snap install node --classic
npx create-react-app react-app --use-npm

#local test
cd react-app/
npm run start

npm run test
CI=true #the npm run test doesn't heard changes
npm run test -- --coverage

npm run build

#deploy app on surge
sudo npm install --global surge
surge
#trite-grandmother.surge.sh

#verify
npm install --save-dev --save-exact prettier
npx prettier --check "**/*.js"
npx prettier --write "**/*.js"
npx prettier --check "**/*.js"

npx prettier --write "**/*.{js,jsx.yml,yaml,.json.css,scss,md}"
npm run format:check
```

## Surge

![Surge](./img/surge.png)
