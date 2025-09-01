# Codex-Environments

Setup and Maintance script for a dotnet project in Codex (web) from OpenAI _(docker still not supported September 2025)._

## Setup Script

```bash
# Install .Net 9

echo "➕ Adding the Ubuntu .NET backports PPA..."
sudo add-apt-repository -y ppa:dotnet/backports

echo "🔄 Updating package lists after adding PPA..."
sudo apt update

echo "⬇️ Installing .NET 9 SDK..."
sudo apt install -y dotnet-sdk-9.0

echo "📦 restore dotnet nuget"
dotnet restore /workspace/YOUR_REPO_NAME
```

## Maintenance Script
```bash
echo "📦 restore dotnet nuget"
dotnet restore /workspace/YOUR_REPO_NAME
```
