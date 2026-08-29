==> Caveats
==> ollama
To start ollama now and restart at login:
  brew services start ollama
Or, if you don't want/need a background service you can just run:
  OLLAMA_FLASH_ATTENTION="1" OLLAMA_KV_CACHE_TYPE="q8_0" /opt/homebrew/opt/ollama/bin/ollama serve
gurutejareddydevireddy@gurutejareddys-MacBook-Pro ~ % ollama serve       
Couldn't find '/Users/gurutejareddydevireddy/.ollama/id_ed25519'. Generating new private key.
Your new public key is: 

ssh-ed25519 AAAAC3NzaC1lZDI1NTE5AAAAIIx4O+IW/hao7pkzO0ZY3FiO7b8fsjZeYZkcQqELmHDZ

time=2026-08-29T19:11:33.351+05:30 level=INFO source=routes.go:1951 msg="server config" env="map[HTTPS_PROXY: HTTP_PROXY: LLAMA_ARG_FIT: LLAMA_ARG_FIT_TARGET: NO_PROXY: OLLAMA_CONTEXT_LENGTH:0 OLLAMA_DEBUG:INFO OLLAMA_DEBUG_LOG_REQUESTS:false OLLAMA_EDITOR: OLLAMA_FLASH_ATTENTION:false OLLAMA_GO_TEMPLATE:true OLLAMA_GPU_OVERHEAD:0 OLLAMA_HOST:http://127.0.0.1:11434 OLLAMA_IGPU_ENABLE: OLLAMA_KEEP_ALIVE:5m0s OLLAMA_KV_CACHE_TYPE: OLLAMA_LLM_LIBRARY: OLLAMA_LOAD_TIMEOUT:5m0s OLLAMA_MAX_LOADED_MODELS:0 OLLAMA_MAX_QUEUE:512 OLLAMA_MAX_TRANSFER_STREAMS:4 OLLAMA_MODELS:/Users/gurutejareddydevireddy/.ollama/models OLLAMA_NOHISTORY:false OLLAMA_NOPRUNE:false OLLAMA_NO_CLOUD:false OLLAMA_NUM_PARALLEL:1 OLLAMA_ORIGINS:[http://localhost https://localhost http://localhost:* https://localhost:* http://127.0.0.1 https://127.0.0.1 http://127.0.0.1:* https://127.0.0.1:* http://0.0.0.0 https://0.0.0.0 http://0.0.0.0:* https://0.0.0.0:* app://* file://* tauri://* vscode-webview://* vscode-file://*] OLLAMA_REMOTES:[ollama.com] OLLAMA_SCHED_SPREAD:false http_proxy: https_proxy: no_proxy:]"
time=2026-08-29T19:11:33.352+05:30 level=INFO source=routes.go:1953 msg="Ollama cloud disabled: false"
time=2026-08-29T19:11:33.352+05:30 level=INFO source=images.go:919 msg="total blobs: 0"
time=2026-08-29T19:11:33.352+05:30 level=INFO source=images.go:926 msg="total unused blobs removed: 0"
time=2026-08-29T19:11:33.352+05:30 level=INFO source=routes.go:2008 msg="Listening on 127.0.0.1:11434 (version 0.33.0)"
time=2026-08-29T19:11:33.353+05:30 level=INFO source=model_list_cache.go:112 msg="model list cache hydration complete" models=0 failures=0 elapsed=838.583µs
time=2026-08-29T19:11:33.353+05:30 level=INFO source=runner.go:60 msg="discovering available GPUs..."
time=2026-08-29T19:11:33.835+05:30 level=INFO source=model_recommendations.go:177 msg="model recommendations cache sleep scheduled" wait=3h44m37.287787749s consecutive_failures=0
time=2026-08-29T19:11:43.371+05:30 level=INFO source=types.go:32 msg="inference compute" id=0 filter_id=0 library=Metal compute=0.0 name=MTL0 description="Apple M2" libdirs=ollama driver=0.0 pci_id="" type=iGPU total="5.3 GiB" available="5.3 GiB"
time=2026-08-29T19:11:43.371+05:30 level=INFO source=routes.go:2058 msg="vram-based default context" total_vram="5.3 GiB" default_num_ctx=4096



ollama run qwen2.5-coder:3b

brew install anomalyco/tap/opencode

opencode
