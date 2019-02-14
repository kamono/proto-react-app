
* ````$ cd $REPO````
* ````$ git clone https://github.com/kamono/proto-react-app.git````
* ````$ cd proto-react-app````

* The Amplify CLI is a tool that allows you create and configure AWS services for your application. Its purpose is to simplify mobile and web application development for you. The CLI uses AWS CloudFormation and nested stacks, which allows you to add or modify configurations locally before you push them for execution in the cloud.
* ````$ npm install -g @aws-amplify/cli````

* If DO NOT have aws configures on your local (~/.aws/config, ~/.aws/credentials), the you can set that up by running the command below.
* ````$ amplify configure````

* ````$ amplify init```` <br>Select the default for Project, then use 'aws' for environment. Choose your editor, select 'javascript' and 'react'. Finally, select the defaults for Path, Build, Start commands. Finally, select the profile you want to use. In my case, I choose 'default', becuase that's what I named it in ~/.aws/config (config deets below)

    ````[default]```` <br>
    ````output = json```` <br>
    ````region = us-east-1````




* ````npm install```` To download the react* dependencies in your package.jsoncl

* AWS Amplify is a library that provides you with tools to build serverless applications. With it, integrating various AWS services with your app can be done in few lines of code
* ````$ npm install --save aws-amplify````
* ````$ npm install --save aws-amplify-react````

* RUN LOCALLY
* ````$ npm start````

* BUILD PROJECT FOR DEPLOYMENT
* ````$ npm build```` or ````$ npm run-script build````

* DEPLOY APP TO THE CLOUD
* ````$ amplify add hosting```` This adds web hosting. Select 'DEV' for this example as selecting PROD will take > 10 minutes. 
    * Create a unique bucket name.
    * Hit Enter to select the default for index doc.
    * Hit Enter to select the default for error doc.

* Use the ````amplify status```` command to view the resources that we will push to aws.

* ````$ amplify publish```` This will deploy our application to the ☁️