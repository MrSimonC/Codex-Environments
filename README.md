# Codex-Environments

This very small repo has one purpose: a good set up script for use in OpenAI Codex Environments.

This repo was created 25 June 25 when .net was not natively supported, nor docker.

I'm a software engineer and OpenAI's Codex is the first real low-cost (i.e. with flat monthly fee) high-value way we have of iterating until a solution is correctly (at least built) and maybe unit tested (if you have such things).

I usually make stuff like this private, so if this was useful to you, then give this repo a star ⭐ thanks! -- Simon C.

```bash
# Install .Net 9

echo "🔄 Updating package lists..."
sudo apt update

echo "➕ Adding the Ubuntu .NET backports PPA..."
sudo add-apt-repository -y ppa:dotnet/backports

echo "🔄 Updating package lists after adding PPA..."
sudo apt update

echo "⬇️ Installing .NET 9 SDK..."
sudo apt install -y dotnet-sdk-9.0

echo "restore dotnet nuget"
cd /workspace/YOUR_REPO_NAME && dotnet restore

# Install Docker (using convenience script)
curl -fsSL https://get.docker.com -o get-docker.sh && sh get-docker.sh && rm get-docker.sh
```