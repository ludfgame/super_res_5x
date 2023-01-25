FROM pytorch/pytorch:1.9.1-cuda11.1-cudnn8-runtime

COPY requirements.txt .

RUN apt-get update && apt-get update && apt-get install -y git libgl1 libglib2.0-0

RUN pip install -r requirements.txt
RUN pip install git+https://github.com/XPixelGroup/HAT

WORKDIR /work