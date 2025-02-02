> nano run-locally.sh

```bash
...
# host local webserver
python3 -m http.server --bind 0.0.0.0 "$PORT"
```
 
> nano /etc/systemd/system/ollama.service
 
```bash
...
Environment="OLLAMA_HOST=0.0.0.0"
Environment="OLLAMA_HOST=http://192.___.1.121:8000"
...
```
 
in browser line on another local web PC: http://192.___.1.121:8000

![](https://raw.githubusercontent.com/unton3ton/ollama-ui/refs/heads/main/ollama-modeltree-dark.gif)

# ollama-ui

Just a simple HTML UI for Ollama

Now available as a chrome extension!
https://chrome.google.com/webstore/detail/ollama-ui/cmgdpmlhgjhoadnonobjeekmfcehffco

## Usage

```
git clone https://github.com/ollama-ui/ollama-ui
cd ollama-ui
make

open http://localhost:8000 # in browser
```

![screenshot1](/screenshot1.jpg?raw=true)

![screenshot2](/screenshot2.jpg?raw=true)
