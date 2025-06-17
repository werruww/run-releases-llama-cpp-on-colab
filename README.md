# run-releases-llama-cpp-on-colab






!wget https://github.com/ggml-org/llama.cpp/releases/download/b5689/llama-b5689-bin-ubuntu-x64.zip
!unzip /content/llama-b5689-bin-ubuntu-x64.zip
!export LD_LIBRARY_PATH=$LD_LIBRARY_PATH:/content/build/bin && /content/build/bin/llama-cli -h

!export LD_LIBRARY_PATH=$LD_LIBRARY_PATH:/content/build/bin && /content/build/bin/llama-cli --model /content/Kimi-Dev-72B-UD-IQ1_S.gguf -p "what is ai?" --ctx-size 10 --batch-size 32 --color
