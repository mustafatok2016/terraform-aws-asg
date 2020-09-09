# terraform-iaac-2020

1. Create file called module.tf
2. Copy paste the following code 
```
module "asg" {
  source  = "mustafatok2016/asg/aws"
  version = "1.0.0"
  region           = "us-east-1"
  key_name         = "asg-key-pair"                    #It will be created
  image_owner      = "amazon"                    #
  desired_capacity = 1
  max_size         = 1
  min_size         = 1
}
```

3. Run 
```
    terraform init 
```
4. Run 
```
    terraform apply
```



# Running in different region
1. Change "region" to something else


# Using different Images
### For centos use AMI_NUMBER
### For Ubuntu use  099720109477
### For AMI   use  AMI_NUMBER
