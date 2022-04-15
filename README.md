# Why work with Terraform via JSON?
Right now I'm on a mission at work to codify user and group management for Okta 
and Google. This will allow us to manage users and groups via a pull request and
reduce user error that is common in click-ops. We also found that there were a
number of Google groups that were improperly configured, which we discovered while
performing the imports into Terraform state. 

Our end goal, and something I'm working on right now, is to create a self-service 
dashboard that our employees can use to handle these requests on their own and
all my team has to do is approve the PR. 

We chose working with JSON files over the normal Terraform .tf files because of
the flexibility that JSON provides given that we write our dashboards in Python.