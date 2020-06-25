# terraform_public

Terraform Public Repositories and Examples

aws = Examples of deployments by Terraform into AWS
Azure = Examples of deployments by Terraform into Azure
DigitalOcean = Examples of deployments by Terraform into Digital Ocean
Local = Examples of local deployements using Terraform


Best practices - 
When adding a new module always follow with

terraform init

If that comes back clean you can test your build with

terraform plan

Or if you want to create an output file to use for your application you can do :

terraform plan -out "<outputfile.out>

If you want to just test the module your are creating and NOT your entire
terraform build, you can do a targetted plan with : 

terraform plan --target "module.<name>" -out "<outputfile.out>"

