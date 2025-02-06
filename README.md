# DeepSeeker

https://huggingface.co/collections/unsloth/deepseek-r1-all-versions-678e1c48f5d2fce87892ace5

Run DeepSeek on local machine

```
git clone https://github.com/ggerganov/llama.cpp.git
cd llama.cpp
cmake .
make
wget https://huggingface.co/unsloth/DeepSeek-R1-Distill-Llama-8B-GGUF/resolve/main/DeepSeek-R1-Distill-Llama-8B-Q8_0.gguf
bin/llama-run DeepSeek-R1-Distill-Llama-8B-Q8_0.gguf 
```

Output
```
> hello                                                                                                     

Hello! How can I assist you today? 😊
> what is 2 ^ 7?

2 raised to the power of 7 is equal to 128.
```

ollama deep_seek 671b on mediator (memory =~ 3T, required >~600G?)

```
export OLLAMA_MODELS=/mnt/tscc2/share/ollama
# systemctl restart ollama?
CUDA_VISIBLE_DEVICES="" ollama serve &
CUDA_VISIBLE_DEVICES="" ollama run deepseek-r1:671b
```
