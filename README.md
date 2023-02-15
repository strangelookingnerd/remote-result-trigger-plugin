Remote-Build-Result-Trigger-Plugin
===================================

A plugin for Jenkins CI  that gives you the ability to monitor successful build on a **remote** Jenkins server.

## Instructions
Enable the trigger within the "Remote Build Result Trigger" section of the build's configuration page.  
When remote server build successful, plugin will trigger a local build and inject remote envs to job.

| EVN_NAME                 | description                                                                                                                                       |
|--------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------|
| REMOTE_BUILD_NUMBER      | The remote build number, such as "153".                                                                                                           |  
| REMOTE_BUILD_TIMESTAMP   | The remote build timestamp, such as "1676017363424".                                                                                              |
| REMOTE_BUILD_URL         | Full URL of this build, like [https://server:port/jenkins/job/foo/15/](https://server:port/jenkins/job/foo/15/) (<i>Jenkins URL</i> must be set). |
| REMOTE_${PARAMETER_NAME} | If remote job use buildWithParameters, use remote parameters replace ${PARAMETER_NAME}.                                                           |

![configuration screen](screenshots/2023021501.png)
## Screenshot
![configuration screen](screenshots/2023021502.png)
