# helm-chart

## Before starting
Create a robot text to disallow some user-agents

At the root of the project, issue: `echo -e “User-Agent: *\nDisallow: /” > robots.txt`

## Create a new chart
Create a new directory called "charts" and cd into it

Issue the command: `helm create charts/test-chart`

Linting: `helm lint charts/test-chart`

Package: `helm package charts/test-chart/`

## Create a new index.yaml file

From project root, `helm repo index --url https://github.com:togoinnov/helm-chart/ .`

cat to check: `cat index.yaml`
