# Cobertura Plugin

[![Build
Status](https://jenkins.ci.cloudbees.com/buildStatus/icon?job=plugins/cobertura-plugin)](https://jenkins.ci.cloudbees.com/job/plugins/job/cobertura-plugin/)

This plugin allows you to capture code coverage report from
[Cobertura](http://cobertura.sourceforge.net/).
Jenkins will generate the trend report of coverage.
The Cobertura plugin can be [downloaded
here](http://updates.jenkins-ci.org/download/plugins/cobertura/).

# Jenkinsfile Step
Sample step to publish the coverage tests.    

    step([$class: 'CoberturaPublisher', autoUpdateHealth: false, autoUpdateStability: false, coberturaReportFile: 'coverage.xml', failNoReports: false, failUnhealthy: false, failUnstable: false, maxNumberOfBuilds: 0, onlyStable: false, sourceEncoding: 'ASCII', zoomCoverageChart: false])

For more information, see [the Wiki
page](https://wiki.jenkins-ci.org/display/JENKINS/Cobertura+Plugin).
