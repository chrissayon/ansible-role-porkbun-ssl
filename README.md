# Porkbun SSL Role

Sends a request to the Porkbun Endpoint to grab the SSL Certifificate

## Installation

To install the role:

```
ansible-galaxy role install chrissayon.porkbun_ssl
```

## Role Variables

| Variable               | Description                                                                         |
| ---------------------- | ----------------------------------------------------------------------------------- |
| domain_name            | The domain you want to grab the SSL for (Will need to be with the Porkbun Provider) |
| porkbun_api_key        | Porkbun API Key                                                                     |
| porkbun_secret_api_key | Porkbun Secret API Key                                                              |
| base_path              | The base path that the keys will get written too                                    |

## Example Playbook

```
- hosts: all
  roles:
  - chrissayon.porkbun_ssl
```
