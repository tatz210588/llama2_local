conda create -n llama2_local python=3.10.9
conda activate llama2_local

git clone https://github.com/thisserand/llama2_local.git
cd llama2_local

pip install -r requirements.txt

huggingface-cli login

provide the token (NO need to add the token ad git credentials)

python llama.py --model_name="TheBloke/Llama-2-7B-Chat-GGML" --file_name="llama-2-7b-chat.ggmlv3.q4_K_M.bin"

