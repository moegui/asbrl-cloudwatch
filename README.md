ASBRL-CLOUDWATCH
=========

Deploy Cloudwatch Agent as a Docker container.

Requirements
------------

Need to be Docker engine installed.

Role Variables
--------------

- default_user: 'ubuntu'
- METRICS_NAMESPACE: "cw-agent"
- METRICS_INTERVAL: 300
- LOGS_GROUP_NAME: "cw-agent"
- LOGS_SERVERLOG_FILE: "syslog"
- DOCKER_LOG_DRIVER: "json-file"
- DOCKER_LOG_OPTIONS: "{}"
- CONTAINER_NAME: "cw-agent"
- DOCKER_CPU_PERIOD: 0
- DOCKER_MEMORY: 0
- DOCKER_LABELS:
    tag1: test
- ADVANCED_METRICS: false

Dependencies
------------

None

Example Playbook
----------------

      - name: Deploy CloudWatch
        include_role:
          name: asbrl-cloudwatch

License
-------

BSD

Author Information
------------------

Moegui.com