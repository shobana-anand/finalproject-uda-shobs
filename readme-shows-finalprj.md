Hello,

I have created 4 workflows -
Frontend Continuous integration which gets triggered both manually and on pull request and runs successfully with all 3 steps - lint, test, build running sucessfully with the lint output and test output as specified in project instruction notes and the image build is done successfully.
Backend Continuous Integration which gets triggered both manually and on pull request and runs successfully with all 3 steps - lint, test, build running sucessfully with the lint output and test output as specified in project instruction notes and the image build is done successfully.
Frontend Continuous deployment which gets triggered on push to main branch and also can get triggered manually. This completes successfuly with all the steps - lint, test and build and  deploy to k8s completes successfully with frontend pods running successfully in the cluster.
Backend Continuous deployment which gets triggered either manually and / or push to main branch. All the steps - lint, test, build and deploy gets completed successfully with backend application running in the container after the successful completion. 


For setting up the resources, I followed the project instructions to apply terraform and spin up the resources. Github-actions-user was used to integrate Github actions with AWS. I also had set up a IAM user shobs-github-user which I used for CLI to interact with AWS. 
