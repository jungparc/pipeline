## Dev Tools > Pipeline > Release Notes

### February 28, 2023
* Added an artifact feature that allows you to use external repository resources as start or end condtions for pipeline stages. You can find how to use in [Pipeline User Guide](/Dev%20Tools/Pipeline/ko/console-guide/#_1)

### January 31, 2023
* Added a feature to assign dynamically created tags by using the image tag format in the build stage.
* Added a feature to deploy with the most recent tag among tags dynamically created using the image tag format in the deployment stage.
* Changes to how image autorun is executed as follows.
    * Tag value is excluded from required values from autorun settings.
    * Changed to automatically run the entered tag and a matched tag with regular expression are pushed.
    * Changed to automatically run a tag when it is pushed with tags excluding latest as long as the tag is not entered.

### December 27, 2022
* Fixed an issue where, when creating a pipeline, you have to select a source repository in the Source Settings step to go to the previous stage.

### October 25, 2022
* Modified to display a guide message when the kubernetes integration test in deployment target times out.

### August 23, 2022
* Made modifications so that, when running a pipeline without stages through the [API](https://docs.nhncloud.com/en/Dev%20Tools/Pipeline/en/api-guide/#pipeline), a failure response is returned.

### July 26, 2022
* Added a webhook stage.
* Changed the API endpoint domain from api-pipeline.cloud.toast.com to kr1-pipeline.api.nhncloudservice.com.

### May 24, 2022
* Added the connection check feature for the source repository, image registry, build tool, and deployment target. You can see how to use it in the [Pipeline User Guide](/Dev%20Tools/Pipeline/en/console-guide). 
* Added details to CloudTrail.
    * Added details for deletion of settings
    * Added details about pipeline execution

### February 22, 2022
* Added GitLab to the source repository. You can find how to use it in the [Pipeline User Guide](/Dev%20Tools/Pipeline/en/console-guide/#set-up-an-environment).

### January 25, 2022
* Added an API to run Pipeline. You can find how to use it in the [Pipeline API Guide](/Dev%20Tools/Pipeline/en/api-guide/#pipeline).
* Known issues (to be improved after analyzing the cause)
    * When creating a development environment, if you specify a value for the development environment constraints, the development environment creation fails.

### May 25, 2021
* Added integration with CloudTrail. You can check the events that occurred in Pipeline in CloudTrail.

### April 27, 2021

#### Release of a New Service
* A continuous deployment service that lets you manage the application deployment flow, such as building source code, creating container images, and deploying container images.
