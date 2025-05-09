## Runs entirely on github no need to download 
#### (only thing u need to do is add email and password)
#### (Remove this file and rename Instructions.md to README.md)
### Table of contents:
- [Setup](https://github.com/dibope/mcserverstarter/blob/main/README.md#to-use-it-for-ur-seedloaf-server)
- [Prevent friends from changing code](https://github.com/dibope/mcserverstarter/blob/main/README.md#to-prevent-them-from-changing-the-code) (Make sure u do this too!)
- [Common problems](https://github.com/dibope/mcserverstarter/blob/main/README.md#common-problems)

### To use it for ur seedloaf server: (Setup)

1)Fork this and create 2 repository secrets named USERNAME, PASSWORD.(ur email and seddloaf password)

  To add repository secret:(Settings > Secrets and variables > Actions > repository secrets)

( No one, even u can't see them after u set so it's really a secret)
![repo_secrets1](https://github.com/dibope/mcserverstarter/blob/main/.github/workflows/Images/repo_secrets1.jpg)

2)Click Run selenium script(yeah not the one in pic) then Run workflow. Refresh page to view the run.
![start_mc](https://github.com/dibope/mcserverstarter/blob/main/.github/workflows/Images/startmc.jpg)

3) Create a finegrain token (If using this for the [bot](https://discord.com/oauth2/authorize?client_id=1365006964001738993))
Go to settings in profile > developer settings > personal access token > fine grain (there a image below if don't know what to set in it)

Permissions for Personal access token

Expiration : no expiration

Repository access : all repositories (or the repo u want)

Permissions : Actions (read and write); Workflow(read and write)


4)Add your friends as collaborators(you know it's not required for the [bot](https://discord.com/oauth2/authorize?client_id=1365006964001738993))
![collaboraters](https://github.com/dibope/mcserverstarter/blob/main/.github/workflows/Images/collaboraters.jpg)

### To prevent them from changing the code:

1)Go to settings>branchs>branch protection rule>Require status check>select "fail-job" or type if not appearred.
![fail_job1](https://github.com/dibope/mcserverstarter/blob/main/.github/workflows/Images/fail_job1.jpg)
![fail_job2](https://github.com/dibope/mcserverstarter/blob/main/.github/workflows/Images/fail_job2.jpg)

2)Set ur friends with read only access

### Common problems:
1. rewrite secrets

2. check if u have enabled workflows in Action tab

3. try **renaming selenium_new.txt to selenium.yml** after renaming current selenium.yml to selenium.txt or something
