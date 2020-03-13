# GitHub resources

Configuration of all Github resources is placed here.

## Usage

To run this example you need to execute:

```bash
$ terraform init
$ terraform plan
$ terraform apply
```

<!-- BEGINNING OF PRE-COMMIT-TERRAFORM DOCS HOOK -->
## Providers

| Name | Version |
|------|---------|
| github | ~> 2.4 |

## Inputs

| Name | Description | Type | Default | Required |
|------|-------------|------|---------|:-----:|
| admins | List of admin usernames | `list(string)` | `[]` | no |
| branch\_protections | Map of team memberships to manage | `map(map(any))` | `{}` | no |
| github\_organization | Github organization to manage | `string` | n/a | yes |
| members | List of member usernames | `list(string)` | `[]` | no |
| repositories | Map of repositories to manage | `map(any)` | `{}` | no |
| team\_memberships | Map of team memberships to manage | `map(map(string))` | `{}` | no |
| team\_repositories | Map of team repositories to manage | `map(string)` | `{}` | no |
| teams | Map of teams to manage | `any` | `{}` | no |

## Outputs

No output.

<!-- END OF PRE-COMMIT-TERRAFORM DOCS HOOK -->