# .NET5: Road to development on Linux Ubuntu

*Ubuntu 20.04*

## Installing

### Installing required system packages

```bash
sudo apt-get install apt-transport-https ca-certificates software-properties-common curl
```

### Add Microsoft GPG apt key

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

Install [C# Extension](https://marketplace.visualstudio.com/items?itemName=ms-dotnettools.csharp) powered by OmniSharp.