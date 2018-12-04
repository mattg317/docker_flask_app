# Deploying your app on AWS Elastic Beanstalk (EB)

1. Assure your app works locally.

2. Push your image up to Docker Hub `docker push <username>/<imagename>`

3. **OPTIONAL** you may need to login if this is the first time you are logging into Docker Hub via the CLI.

4. **OPTIONAL** create an AWS account if you don't have one.

5. Edit the **Name** in the [Dockerrun.aws.json](Dockerrun.aws.json) file to the your `<username>/<imagename>`

6. Login to AWS and navigate to the Elastic Beanstalk console.

7. Click **Create New Application**

8. Give your application a unique name and provide a description then click **Create**.

9. Under Environments click **Create one now** and select **Web server environment**.

10. Enter a domain.

11. Select `Docker` under **Proconfigured platform**.

12. Select `Upload your code` and upload your `Dockerrun.aws.json` file.

13. Click **Create** and wait a for minutes for setup to complete.

14. Visit your site at `<domainname>.<availability zone>.elasticbeanstalk.com`