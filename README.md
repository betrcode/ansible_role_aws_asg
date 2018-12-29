betrcode.aws_asg
===================

*Better Code AWS AutoScalingGroup*

This role creates a AWS AutoScalingGroup and a 
ElasticLoadBalancer. The ASG will start a Docker image of 
your choice.

This role does not use CloudFormation.
See `betrcode.aws_cloudformation_asg` for another role
where CloudFormation is used. 


Requirements
------------

AWS credentials.

Packages:

* boto3


Role Variables
--------------

TODO: 


Dependencies
------------

Not dependent on any other role.


Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

---

    - hosts: localhost
      connection: local
      gather_facts: yes  # needed for ansible_date_time
      roles:
        - role: betrcode.aws_asg
          docker_image: "nginx:latest"

License
-------

MIT


Author Information
------------------

Max Wenzin, partner at Crisp

https://www.crisp.se/konsulter/max-wenzin

