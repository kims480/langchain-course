## Preparation
git clone https://github.com/emarco177/langchain-course
cd langchain-course 
git checkout --orphan project/hello-world  
git rm -rf . 
powershell -ExecutionPolicy ByPass -c "irm https://astral.sh/uv/install.ps1 | iex" // download uv pythin package manager (Build on rust).. pip build on python
uv --help

## Initialization
uv init --no-package #Initialize the uv environment
uv add langchain
uv add langchain-openai
uv add python-dotenv black isort

# (langchain-course) PS D:\automations\codes\langchain\langchain-course> (langchain-course) means virtual env with name langchain-course

pyproject.toml have all the packages and versions required to cover this cource
black .
isort .
git status  
git add .  
git status  
git commit -m "enviroment setup"