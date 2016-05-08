Ansible Role: chibineko
=========

Install [chibineko](https://chibineko.jp/) on Ubuntu 14.04 LTS.

Requirements
------------

None

Role Variables
--------------

Available variables are listed below, along with default values (see `defaults/main.yml`):

- chibineko_source_directory: "/home/{{ ansible_user_id }}/src/chibineko"
- chibineko_ruby_version: "2.3.0"
- chibineko_mailer_development_default_url_options_host: "localhost"
- chibineko_mailer_development_default_url_options_port: 3000
- chibineko_mailer_test_default_url_options_host: "localhost"
- chibineko_mailer_test_default_url_options_port: 3000
- chibineko_mailer_production_default_url_options_host: "example.com"
- chibineko_mailer_production_delivery_method: :smtp
-  chibineko_mailer_production_smtp_settings_enable_starttls_auto: true
- chibineko_mailer_production_smtp_settings_address: "smtp.gmail.com"
- chibineko_mailer_production_smtp_settings_port: 587
- chibineko_mailer_production_smtp_settings_domain: "example.com"
- chibineko_mailer_production_smtp_settings_authentication: "plain"
- chibineko_mailer_production_smtp_settings_user_name: "<yourname>@gmail.com"
- chibineko_mailer_production_smtp_settings_password: "<yourpassword>"

Dependencies
------------

None

Example Playbook
----------------

    - hosts: servers
      roles:
         - { role: kobanyan.chibineko }

License
-------

MIT / BSD

Author Information
------------------

kobanyan
