# This repo is to gentle introduction about the GenAI

Some of the People/Students are worry about the paid api keys to access the LLM
This blocking them to built the application.

The indentation of this repo is to address that problem by they can do at-least POC level as an experimentation. 

The solution is so simple following the method of running the tiny model in local by using the ollama and built the application.

## Begin to LLM setup

1) As the first step we need to download the ollama cli, from their official website.

    https://ollama.com 

    ![alt text](./images/cli_page.jpeg)


> **_Data Warning:_**   This will be around 500mb.

2) Then we have to pull any of the llm models into local, by running the following command.

> **_Data Warning:_**  Data Warning:llama will consume 4.7GB and gemma 5.5GB 

Try to run any one of the command is fine to pull, both are different models,
```
    ollama pull llama3.1
```
or
```
    ollama pull gemma2
```

> **_NOTE:_**  System should have atleast 8GB of RAM available to run the models.

If its less than that try with below, very tiny model

```
    ollama pull gemma2:2b
```

> **_Data Warning:_** This one 1.6GB

3) After completion we can test using the command the model using the below command

```
    ollama run llama3.1
```

### Model setup is completed.

## Software Setup:

1) I hope you have the proper setup of python in your system and it is greater that 3.10 or 3.11

    If not follow the below link to download and install the python, 

    https://www.python.org

#### Optional softwares

2) Git for clone the repo and version control.
3) Visual Studio Code as a editor.


## Project Setup:

1) Clone this repo by using the following command, or download as the zip

    ```
    git clone https://github.com/karthickn210/GenAI.git
    ```

2) Get into the directory by run the following command,

    ```
    cd GenAI
    ```
3) lets create an virtual environment, to install dependency. 

    ```
    python -m venv .venv
    ```

4) To activate the virtual environment follow the below commands,
    For Windows,
    ```
    .\venv\Scripts\activate
    ```
    For Linux or Mac,
    ```
    source ./venv/bin/activate
    ```
5) Install the dependencies,
    ```
    pip install -r requirements.txt
    ```

### Congrats thats it with setup, lets get into the code.