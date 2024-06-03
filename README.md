# GitHub Actions Collection

This repository contains multiple GitHub Actions.

## 1. Install Ansible

An action to install Ansible on a GitHub runner.

### Example Usage

```yaml
name: Install Ansible

on: [push]

jobs:
  install-ansible:
    runs-on: ubuntu-latest
    
    steps:
      - name: Checkout code
        uses: actions/checkout@v2

      - name: Install Ansible
        uses: prabhatraghav/myscripts/.github/actions/install-ansible@v1
