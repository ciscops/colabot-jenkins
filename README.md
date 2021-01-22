# COLABot-Jenkins
Deployment:
1.  Build image
    - docker build -t jenkins:jcasc .
2. Tag image
    - docker tag $IMAGE $REPO/$IMAGE_NAME
3. Push image to repo
    - docker push $REPO/$IMAGE_NAME
4. Deploy with the following environment vars:
- GITHUB_ADMIN_ID
- GITHUB_TOKEN
- DOCKERHUB_ID
- DOCKERHUB_PASSWORD
- JENKINS_ADMIN_ID
- JENKINS_ADMIN_PASSWORD
- JENKINS_LOCATION_URL
