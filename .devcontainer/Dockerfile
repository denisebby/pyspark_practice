FROM jupyter/pyspark-notebook:31b807ec9e83

USER root

RUN apt-get clean && apt-get update && apt-get -y install --no-install-recommends \
    python3-pip

# this didnt work but adding user root seems to have worked anyways
# RUN useradd -m vscode && echo "docker:docker" | chpasswd && adduser vscode sudo

RUN pip3 install ipykernel

# USER vscode
CMD /bin/bash



