# gpt_quick_start

chat_gpt_quickstart

#0) Make a new python virtual environment

pip install venv (in case you dont have venv installed)

python -m venv /path/to/new/virtual/environment

#So something like:
cd go/to/some/directory
python -m venv gpt_env
source gpt_env/bin/activate

#At this point forward, you will be in that environment and all your libraries will be installed in isolation

# https://docs.python.org/3/library/venv.html

# https://stackoverflow.com/questions/70242667/how-to-create-venv

# Windows-specific instructions here:
# https://mothergeo-py.readthedocs.io/en/latest/development/how-to/venv-win.html



# 1) Install OpenAI and other necessary libraries

# To install the OpenAI Python library:

pip install openai
#(pip3 install openai if path settings arent set)


#2) Set API key
#The library needs to be configured with your account's API key, which you obtain from your OpenAI account.

#You can either set it as the OPENAI_API_KEY environment variable before using the library:

export OPENAI_API_KEY='sk-...'

#Or, within your python script, set openai.api_key to its value:

import openai
openai.api_key = "sk-..."

