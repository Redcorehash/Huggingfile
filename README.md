# Huggingfile
!pip install huggingface_hub

from huggingface_hub import hf_hub_download

# Download the file from Hugging Face
file_path = hf_hub_download(repo_id="Doubleupai/huggingfile", filename="your_file_name")

# Convert the file to txt
with open(file_path, 'r') as file:
    content = file.read()

with open('output.txt', 'w') as output_file:
    output_file.write(content)
