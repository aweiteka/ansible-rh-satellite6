Ansible playbook to install standalone Red Hat Satellite Server v6.

## Usage ##
1. Clone this repo

        https://github.com/aweiteka/ansible-rh-satellite6.git

2. Update inventory hosts file if not running locally
3. Copy custom_vars.template to custom_vars.yaml file and update. Also review vars in site.yaml

        cp custom_vars.template custom_vars.yaml

4. Run the playbook:

        ansible-playbook site.yaml -i inventory [ansible-opts]

## Requires ##
 * Ansible 1.2+ running on local control machine
 * RHEL 6
 * A Red Hat subscription. The system will be registered and subscribed.

## Issues ##
 * Red Hat subscription not working. You must first register machine to RH CDN and attach Satellite 6 subscription.
