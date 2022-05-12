to list all workspace commands use,
terraform workspace -h  as follows:
PS C:\Terraform\Excercises\Workspace> terraform workspace -h
Usage: terraform [global options] workspace

  new, list, show, select and delete Terraform workspaces.

Subcommands:
    delete    Delete a workspace
    list      List Workspaces
    new       Create a new workspace
    select    Select a workspace
    show      Show the name of the current workspace



    PS C:\Terraform\Excercises\Workspace> terraform workspace show
    default


    PS C:\Terraform\Excercises\Workspace> terraform workspace list
    * default

    PS C:\Terraform\Excercises\Workspace> terraform workspace new dev
    Created and switched to workspace "dev"!

    You're now on a new, empty workspace. Workspaces isolate their state,
    so if you run "terraform plan" Terraform will not see any existing state
    for this configuration.

    PS C:\Terraform\Excercises\Workspace> terraform workspace show
    dev

    PS C:\Terraform\Excercises\Workspace> terraform workspace list
      default
    * dev


    PS C:\Terraform\Excercises\Workspace> terraform workspace new staging
    Created and switched to workspace "staging"!

    You're now on a new, empty workspace. Workspaces isolate their state,
    so if you run "terraform plan" Terraform will not see any existing state
    for this configuration.

    PS C:\Terraform\Excercises\Workspace> terraform workspace new production
    Created and switched to workspace "production"!

    You're now on a new, empty workspace. Workspaces isolate their state,
    so if you run "terraform plan" Terraform will not see any existing state
    for this configuration.

    PS C:\Terraform\Excercises\Workspace> terraform workspace list
      default
      dev
    * production
      staging
