

Next step is to create a YAML file, which will set the foundation of the CI/CD server. 


Create the YAML file with the following command `touch .gitlab-ci.yml`{{execute}} in your project repository. Using `nano .gitlab-ci.yml`{{execute}}, add following code to the
YAML file:


    build-job:
      stage: build
      script:
        - echo "Hello, $GITLAB_USER_LOGIN!"

    test-job1:
      stage: test
      script:
        - echo "This job tests something"

    test-job2:
      stage: test
      script:
        - echo "This job tests something, but takes more time than test-job1."
        - echo "After the echo commands complete, it runs the sleep command for 20 seconds"
        - echo "which simulates a test that runs 20 seconds longer than test-job1"
        - sleep 20

    deploy-prod:
      stage: deploy
      script:
        - echo "This job deploys something from the $CI_COMMIT_BRANCH branch."

This sample code will only execute echo commands, but it gives an overview of how you can specify the stages for your project.