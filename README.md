# default-credentials-scanner

Small helper to run **THC-Hydra** with SecLists **`*betterdefaultpasslist*`** combo files (under `Passwords/Default-Credentials`) against a host list.

## Requirements

- Kali (or similar) with `hydra` and SecLists at `/usr/share/seclists/...`

## Usage

```bash
chmod +x hydra-betterdefaults.sh
./hydra-betterdefaults.sh [options] targets.txt
```

`targets.txt`: one IP or hostname per line (optional `host:port`). See `./hydra-betterdefaults.sh --help` for `-d` (dry-run), `-o` (output dir), `-e` (extra hydra args), and env vars.

Use only on systems you are authorized to test.
