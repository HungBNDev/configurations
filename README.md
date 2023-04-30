# Please read the source code before run the following commands. It may different from your local config.
# Set AWS profile
  `export AWS_PROFILE=aws_profile_name`
# Install Ansible
  `brew install ansible`

# Install the required modules
  `ansible-galaxy install zzet.rbenv`

# Get the ip of host(s)
  `ansible-inventory -i inventory-tools.aws_ec2.yml --graph`
  Paste the ip to file `hosts`

# Run the playbook
  `ansible-playbook -i hosts playbooks.yml -vv`
  `-vv` is the optional.
