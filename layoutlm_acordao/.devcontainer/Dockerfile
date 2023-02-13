FROM tensorflow/tensorflow:latest-gpu-jupyter

RUN apt-get update && \
    apt-get install -y software-properties-common && \
    add-apt-repository ppa:alex-p/tesseract-ocr-devel && \
    apt-get install -y git \
    ffmpeg \
    libsm6 \
    libxext6 \
    libpoppler-dev \
    ffmpeg \
    libsm6 \
    libxext6 \
    libmagickwand-dev \
    tesseract-ocr \
    tesseract-ocr-por



RUN pip install pandas \
    scikit-learn \
    seaborn \
    scikit-image \
    pandas \
    opencv-python \
    Wand \
    Pillow \
    pdf2image \
    pytesseract \
    matplotlib \
    pdfplumber \
    pprintpp \
    Unidecode \
    torch torchvision torchaudio --extra-index-url https://download.pytorch.org/whl/cu115 \
    simpletransformers \
    && pip uninstall nvidia_cublas_cu11 -y

COPY policy.xml /etc/ImageMagick-6
