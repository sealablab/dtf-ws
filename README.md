# DTF Workspace

This repository contains the development environment for DTF (DUT Testing Framework) projects. 

## Quick Start

1. Clone this repository:
   ```bash
   git clone git@github.com:sealablab/dtf-ws.git ./DTF
   cd ./DTF
   ```

2. Run uv `uv-go.sh`  
   ```bash
	user@box ~/DTF: bash ./uv-go.sh                                                                                                   (base)
	Cloning into 'dtf-framework'...
	Cloning into 'dtf-tools'...
	Resolved 6 packages in 116ms
    Built dtf-framework @ file:///Users/johnycsh/dtf-ws/dtf-framework
	Resolved 23 packages in 240ms
	Built dtf-tools @ file:///Users/johnycsh/dtf-ws/dtf-tools
   ```
3. Run uv venv
   ``` bash
	uv venv
	Creating virtual environment at: .venv
	Activate with: source .venv/bin/activate.fish
	```

4. Don't forget to source the appropriate activate from your current shell:
   ``` bash
	source .venv/bin/activate.___
	Creating virtual environment at: .venv
	user@box: ~/dtf-ws: source .venv/bin/activate.fish
	(dtf-ws) user@box ~/DTF (main)>
	```


## Project Structure

```
dtf-workspace/
├── pyproject.toml         # `dtf-workspace` Contains references to `dtf-framework` and `dtf-tools` 
├── dtf-framework/         # `dtf-framework` source
└── dtf-tools/             # `dtf-tools` source
```

## Contributing

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Submit a pull request

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
