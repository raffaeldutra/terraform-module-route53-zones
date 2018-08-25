# Terraform module for AWS Route 53

Terraform module to create one Route53 DNS record for a new zone.

## Usage

```hcl
module "route53-zone-example-solutions" {
  source = "git@github.com:raffaeldutra/terraform-module-route53-zones"
  zone   = "example.solutions"
}
```

```hcl
module "route53-zone-example-cloud" {
  source = "git@github.com:raffaeldutra/terraform-module-route53-zones"
  zone   = "example.cloud"
}

```


## Outputs

```hcl
${aws_route53_zone.zone.zone_id}
```

```hcl
${aws_route53_zone.zone.zone_name}
```
