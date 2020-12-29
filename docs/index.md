# Getting started

Simple way to develop C# with .NET5 on Linux Ubuntu 20.04.

## Installing

### Installing required system packages

```bash
sudo apt-get install apt-transport-https ca-certificates software-properties-common curl
```

### Add Microsoft GPG apt key and repos
 
```bash
curl -sSL https://packages.microsoft.com/keys/microsoft.asc | sudo apt-key add -
```

```bash
sudo add-apt-repository "deb [arch=amd64] https://packages.microsoft.com/repos/vscode stable main"
```

```bash
wget https://packages.microsoft.com/config/ubuntu/20.04/packages-microsoft-prod.deb 
```

```bash
sudo dpkg -i packages-microsoft-prod.deb 
```

```bash
sudo apt-get update
```

### Install VSCode

```bash
sudo apt install code
```

### Install .NET5

```bash
sudo apt install dotnet-sdk-5.0
```

### Install VSCode Extension

Install [.NET Extension Pack](https://marketplace.visualstudio.com/items?itemName=doggy8088.netcore-extension-pack). It contains a large number of helpful extensions for C# development.

## Smarter way for installing with ansible

```bash
sudo apt install ansible git
```

Ansible is an open-source automation tool for orchestration and general configuration and administration of computers.

For this we need the Ansible Requirements with Ansible-Galaxy.

```bash
git clone https://github.com/codegecko/NET5RoadToDevelopmentOnLinuxUbuntu
```

```bash
cd NET5RoadToDevelopmentOnLinuxUbuntu/src
```

```bash
ansible-galaxy install -r requirements.yml
```

```bash
ansible-playbook playbook.yml
```

## First CLI Project

### Create projects folder

```bash
mkdir projects
```

### Create CLI project (console project)

```bash
dotnet new console -n CLIProject
```