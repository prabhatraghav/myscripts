# GitHub Actions Collection

This repository contains multiple GitHub Actions.

## 1. Install Ansible

An action to install Ansible on a GitHub runner.

### Example Usage:

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
```

## 2. Install Docker Engine

An action to install Docker Engine on a GitHub runner.

### Example Usage:

```yaml
name: Install Docker Engine

on: [push]

jobs:
  install-docker:
    runs-on: ubuntu-latest
    
    steps:
      - name: Checkout code
        uses: actions/checkout@v2

      - name: Install Docker Engine
        uses: prabhatraghav/myscripts/.github/actions/install-docker@v1
        with:
          docker_version: 'latest'
```

## 3. Install Terraform

An action to install Terraform on a GitHub runner.

### Example Usage:

```yaml
name: Install Terraform

on: [push]

jobs:
  install-terraform:
    runs-on: ubuntu-latest
    
    steps:
      - name: Checkout code
        uses: actions/checkout@v2

      - name: Install Terraform
        uses: prabhatraghav/myscripts/.github/actions/install-terraform@v1
```

## 4. Install Aqua Trivy

An action to install Aqua Trivy on a GitHub runner.

### Example Usage:

```yaml
name: Install Aqua Trivy

on: [push]

jobs:
  install-trivy:
    runs-on: ubuntu-latest
    
    steps:
      - name: Checkout code
        uses: actions/checkout@v2

      - name: Install Aqua Trivy
        uses: prabhatraghav/myscripts/.github/actions/install-trivy@v1
```
