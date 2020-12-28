# .NET5: Road to development on Linux Ubuntu

## Installing

### Installing required system packages

```bash
sudo apt-get install apt-transport-https ca-certificates software-properties-common
```

### Add Microsoft GPG apt key

```bash
curl -sSL https://packages.microsoft.com/keys/microsoft.asc | sudo apt-key add -
```

```bash
sudo apt-add-repository https://packages.microsoft.com/ubuntu/20.04/prod
```

### Install VSCode

```bash
sudo apt-get update
```

```bash
sudo apt install code
```

### Install .NET5

```bash
sudo apt install dotnet-sdk-5.0
```