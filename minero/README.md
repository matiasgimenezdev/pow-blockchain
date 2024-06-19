# PoW miners

These nodes will be in charge of processing the tasks generated by the coordinator node applying brute force to solve the challenge of mining new blocks of the blockchain. To calculate the hash that solves the challenge it uses the host CPU or the NVIDIA GPU (using CUDA) in case it detects its presence.

## Instructions

1. Install dependencies

```sh
python3 -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
```

2. Run the application

```sh
flask --app src/server.py run --host 0.0.0.0
```