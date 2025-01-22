```
# Install dependencies and GaiaNet node
!curl -sSfL 'https://github.com/GaiaNet-AI/gaianet-node/releases/latest/download/install.sh' | bash

# Source the bash configuration (not directly applicable in Colab, but you can ensure proper path settings)
import os
os.environ['PATH'] += ':/root/.local/bin'

# Initialize GaiaNet with the specified configuration
!gaianet init --config https://raw.githubusercontent.com/GaiaNet-AI/node-configs/refs/heads/main/llama-3.2-3b-instruct/config.json

# Start GaiaNet
!gaianet start

# Check Node ID & Device ID
!gaianet info
```
