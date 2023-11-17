# sctp 312 cd serverless

Create new repo 
```
git clone
git add . 
git commit -m "first commit message"
git push
```

Initialize the node application. A new package.json file will be created. running npm install serverless will give us serverless as dependency for project in the package.json file and the package lock json file. 
```
npm init
npm install serverless
npm install serverless-offline --save-dev
```

Add new files
- serverless.yml
- index.js
- .gitignore

Run `serverless offline start`
to test server app on local, you can get a link from local host. 

Run `serverless package` to check if application is read to be deployed. It will create a .serverless folder and create the cloudformation templates. 

Run `serverless deploy` to run this on AWS. It will deploy based on cloud formation template. 