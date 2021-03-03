FROM ubuntu:latest

ENV DEBIAN_FRONTEND noninteractive

# RUN apt install --no-install-recommends -y \
#       python3 python3-pip texlive texlive-extra-utils texlive-base git \
#       latexmk texlive-xetex texlive-pstricks texlive-science texlive-publishers && \
#     pip3 install pygments

RUN apt-get update -q && \
    apt-get install -qy texlive-full && \
    apt-get purge -y *-doc && \
    apt-get clean -y && \
    rm -rf /var/lib/apt/lists/*
