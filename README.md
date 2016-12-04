# DockerPOC
I'm a repo to do docker poc

## Features
* I'll setup a jenkins server that will have the initial setup turned off.
* The jenkins setup will have an admin user already in place.
* The jenkins setup comes with a pre-installed plugins such as git, maven, job-dsl.. you can install more plugins by adding an entry in plugins.txt.
* The jenkins setup comes with 5 pre-bundled jenkins jobs
  * SeedJob: This is a a seed job that creates the rest of the 4 jobs, if you want to add more pre-bundled jobs you just need the put the dsl of those jenkins jobs in jobdsl folder.
  * RepoCICreator: This jenkins job can do the CI setup of a project, right now it can setup the code stability and code coverage jenkins jobs of a maven based java project, but we can add more capabilities as and when needed.
  * ProjectStatsPluginGenerator: This jenkins job creates the artifact(hpi) for Project stats plugin.
  * BuildsTrackerPluginGenerator: This jenkins job creates the artifact(hpi) for Builds Tracker plugin.
  * JenkinsImageGenerator: This jenkins job creates the image of current jenkins setup, with the above 2 custom plugins installed and uploads it to a private docker repository(ECR).
* 
