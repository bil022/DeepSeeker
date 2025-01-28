# DeepSeeker
How to run DeepSeek on local machine

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
