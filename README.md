### Overview

Red Hat® Ansible® Automation Platform advanced deployment lab

### Overall Architecture

![Architech](.images/ntier-app-topology.png)

### Outline of work flow

- provision infrastucrture include (frontend1, app1, app2, appdb1)
- setup dns using user_data
- test connection via control node with other hosts
- setup yum repos (via satellite)
- install postgres 10
- setup postgres for remote password, listing port, user, password
- setup application
- install flask application
- setup haproxy for loadbalancer application
- run smoke test application

### Projects setup

![Projects](.images/project-setup.png)

### Ansible Tower Listing all the job templates

![Jobtemplates](.images/list-all-jobs-template.png)

#### Jobs Template Detail

- 06_Cloud_Provisioner
  ![06_Cloud_Provisioner](.images/06_Cloud_Provisioner.png)
- 07_Check_Connection
  ![07_Check_Connection](.images/07_Check_Connection.png)
- 08_Clean_up
  ![08_Clean_up](.images/08_Clean_up.png)
- 09_Add_Subscription
  ![09_Add_Subscription](.images/09_Add_Subscription.png)
- 10_Database_Tier
  ![10_Database_Tier](.images/10_Database_Tier.png)
- 11_App_Tier
  ![11_App_Tier](.images/11_App_Tier.png)
- 12_Lb_Tier
  ![12_Lb_Tier](.images/12_Lb_Tier.png)
- 13_Smoke_Test
  ![13_Smoke_Test](.images/13_Smoke_Test.png)

### Ansible Tower Workflow

#### Infrastructure Provision Workflow

![Infra](.images/infra-provision-workflow.png)

#### Multi-tier Applicaton Workflow

![Apps](.images/multi-tier-app-workflow.png)

#### Nested Workflow

![Nested](.images/single-deploy.png)
