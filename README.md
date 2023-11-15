# terraform-aws-s3

# Terraform AWS S3 Bucket Module

This is a module for creating an S3 bucket on AWS using Terraform.

## Usage

```hcl
module "s3_bucket" {
  source = "github.com/imoisharma/terraform-aws-s3"

  bucket_name = "my-bucket"
  acl    = "private"

  // Other module arguments  
}
```

## Requirements
- Terraform 0.12.x
- AWS provider >= 2.x

## Inputs
| Name         | Description               | Type   | Default | Required |
| ------------ | ------------------------- | ------ | ------- | -------- |
| bucket_name  | Name of the S3 bucket      | string | -       | yes      |
| acl          | ACL for the bucket         | string | private | no       |

## Outputs
| Name           | Description            |
| -------------- | ---------------------- |
| s3_bucket_id   | The name of the bucket |

## Contributing
Contributions are welcome! Please open an issue or PR on [GitHub](https://github.com/your-repository).
