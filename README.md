# Web-Cloner

# Install Homebrew
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"  # Fetch and execute the Homebrew installation script

# Add Homebrew to your PATH (for bash users, adapt for other shells if necessary)
echo 'eval "$(/home/linuxbrew/.linuxbrew/bin/brew shellenv)"' >> ~/.bashrc  # Add Homebrew environment setup to bashrc
eval "$(/home/linuxbrew/.linuxbrew/bin/brew shellenv)"  # Evaluate the Homebrew environment setup

# Reload your shell configuration
source ~/.bashrc  # Reload bash configuration

# Verify Homebrew installation
brew --version  # Check the installed version of Homebrew to confirm installation

# Install Go using Homebrew
brew install go  # Install the Go programming language

# Set up your Go environment variables
export GOPATH=$HOME/go  # Set GOPATH to the Go workspace
export PATH=$PATH:$GOPATH/bin  # Add GOPATH/bin to your PATH

# (Optional) Add Go environment variables to your shell configuration for persistence
echo 'export GOPATH=$HOME/go' >> ~/.bashrc  # Add GOPATH to bashrc
echo 'export PATH=$PATH:$GOPATH/bin' >> ~/.bashrc  # Add GOPATH/bin to PATH in bashrc

# Reload your shell configuration again
source ~/.bashrc  # Reload bash configuration to apply changes

# Navigate to your Go project directory
cd path/to/your/project  # Change directory to your Go project

# Run your Go file
go run yourfile.go  # Execute your Go file

# (Optional) Build and run your Go project
go build -o yourbinary  # Compile your Go project into a binary named 'yourbinary'
./yourbinary  # Run the compiled binary
