### Here is a step-by-step guide to deploy WordPress using an RDS:

### Set up an RDS instance:

- Log in to your AWS Management Console.
- Choose RDS from the list of services.
- Click on "Create Database".
- Select the engine type, version, and instance size for your RDS instance.
- Choose a username and password for your database instance.
- Choose the VPC and subnet where you want to deploy your RDS instance.
- Choose the database name you want to use for your WordPress site.
- Click on "Create Database" to create your RDS instance.

### Set up a security group:

- Choose "Security Groups" from the RDS dashboard.
- Click on "Create Security Group".
- Give your security group a name and description.
- Add inbound rules to allow traffic from your WordPress EC2 instance and from your own IP address.
- Click on "Create" to create your security group.

### Launch an EC2 instance for WordPress:

- Choose EC2 from the list of services.
- Click on "Launch Instance".
- Select an Amazon Machine Image (AMI) that supports WordPress, such as Amazon Linux 2 AMI.
- Choose an instance type and configure the instance details.
- Select the VPC and subnet where you want to deploy your instance.
- Add storage and configure any additional details as needed.
- Choose the security group you created earlier to configure inbound rules.
- Launch your instance.

### Connect to your EC2 instance and install WordPress:
- Connect to your EC2 instance using SSH.
- Update the instance and install any required packages, such as Apache and PHP.
- Download the latest version of WordPress from the official website.
- Extract the WordPress files and move them to the appropriate directory on your instance.
- Configure the wp-config.php file with the database details for your RDS instance.
- Create a new virtual host file in Apache to serve your WordPress site.

### Test your WordPress installation:
- Open a web browser and navigate to the IP address or domain name of your EC2 instance.
- Follow the WordPress installation prompts to create a new site.
- Log in to your new WordPress site and configure any settings as needed.
- That's it! You have now deployed WordPress using an RDS.
