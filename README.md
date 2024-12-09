# Ansible Validated Content Setup

## Prerequisites

Before proceeding, ensure you have the following:

- Ansible Automation Platform (AAP) installed and configured.
- An appropriate user with the necessary permissions to create projects and job templates in AAP.

## Create the Project

| Input | Value
| ---: | ---
| Name | JTalton / Setup Projects and Job Templates
| Description | Playbooks for setting up projects and job templates to run the validated content.
| SCM Type | git
| SCM URL | https://github.com/jamestalton/playbooks.git

## Create the Job Template

| Input | Value
| ---: | ---
| Name | JTalton / Setup Projects and Job Templates
| Description | This job template adds projects and job templates to run the validated content.
| Project | Setup Validated Content
| Playbook | setup.yml

### Extra Var

Check the `prompt on launch` for extra vars.

Enter the required variables:

```yaml
aap_url: YOUR_AAP_URL
aap_username: PROMPT_USERNAME
aap_password: PROMPT_PASSWORD
```
