## gen-terraform-env-vars

Python script parses an existing .tfvars file and generates a .sh version you can stat in your session to generate your global TF_VARS

Works around Warnings message and issue discussed here https://github.com/hashicorp/terraform/issues/22004

### Usage
Pass the script the location of your .tfvars file and script will generate a .tfvars.sh version you can export

```
python gen_terraform_env_vars.py /ops/utils/terraform.tfvars
```

### Limitations

* Requires Python3
* Linux only
* Only handles simple key/value pairs (so if you have lists etc you will need to extend script)
