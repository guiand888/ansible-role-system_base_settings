guiand888.system_base_settings
===

# Purpose
Baseline system configuration with:  
- Hostname Configuration  
- Locale Settings  
- Timezone Management  
- NTP Configuration with Chrony  

# Instructions

## Required Variables
- `system_base_settings_timezone`: System timezone (default: Asia/Singapore)  
- `system_base_settings_ntp_servers`: List of NTP servers  
- `system_base_settings_system_locale`: System locale settings  

## Example Configuration
```yaml
system_base_settings_timezone: Asia/Singapore
system_base_settings_ntp_servers:
  - 0.sg.pool.ntp.org
  - 1.sg.pool.ntp.org
system_base_settings_system_locale: en_US.UTF-8
```

## Example Playbook
```yaml
- hosts: all
  roles:
    - guiand888.system_base_settings
  vars:
    system_base_settings_timezone: Europe/London
```

# Maintainers
Guillaume A.
  - Contact: [mail@guillaumea.fr](mailto:mail@guillaumea.fr)
  - Blog: https://blog.guillaumea.fr
