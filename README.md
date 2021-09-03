# Supply Chain Goat

## Introduction

The purpose of this repository is to share information and learn about software supply chain security issues. 

Follow these steps to learn about threats and countermeasures related to software supply chain. If you would like to see a different threat being addressed, or have other feedback, please create an issue. 

## Get started

1. Create a fork of the repo.
2. Go to the Actions tab in the fork. Click the "Enable Actions" button. 

## Tutorial #1

1. Create a new issue in the forked repo. Then label the issue as an enhancement. Once you do this, an action will get triggered. 
2. Go to the Actions tab, and have a look at the permissions assigned to the `GITHUB_TOKEN`. 
3. By default, the `GITHUB_TOKEN` has a lot of permissions assigned. 
4. You can now manually secure the workflow by adding the `permissions` key, but it is hard to know what the permissions should be. In this tutorial, let us fix the permissions automatically. 
5. Visit [Step Security GitHub App](https://github.com/apps/step-security) and click on Install. Install it on your forked repo.
6. You should see a pull request with the minimum permissions assigned for the workflow. 
7. Create another issue and label it as an enhancement. Another workflow will get triggered. 
8. Go to the Actions tab, and have a look at the permissions assigned to the `GITHUB_TOKEN` in the new workflow run. 
9. Now it has the minimum permissions assigned. 
10. Congratulations on completing the tutorial!

## Threats and Countermeasures

This table lists threats and countermeasures related to software supply chain security. More will be added soon. 

Number | Threats  | Countermeasures  | Related incident
-------|--------- |------------------|----------------
1      |Exfiltration of secrets from the pipeline | Use credentials that are minimally scoped | Codecov breach, where credentials were exfiltrated from pipelines
