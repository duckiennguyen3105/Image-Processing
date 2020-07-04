# Image-Processing
Chào mừng đến với hướng dẫn chạy code xử lí ảnh 
Để chạy được code thì cần phải cài đặt những thư viện sau trong Python 

!! Lưu ý: chỉ chạy được trên hệ điều hành Linux

        1, Phải cài đặt Python 3, link cài đặt: https://www.python.org/download

        2, Chạy câu lệnh dưới đây trong terminal để cài đặt thư viện: 
                apt-get install -y --fix-missing \
                    build-essential \
                    cmake \
                    gfortran \
                    git \
                    wget \
                    curl \
                    graphicsmagick \
                    libgraphicsmagick1-dev \
                    libatlas-base-dev \
                    libavcodec-dev \
                    libavformat-dev \
                    libgtk2.0-dev \
                    libjpeg-dev \
                    liblapack-dev \
                    libswscale-dev \
                    pkg-config \
                    python3-dev \
                    python3-numpy \
                    software-properties-common \
                    zip \
                    && apt-get clean && rm -rf /tmp/* /var/tmp/*
    
           3, Chạy câu lệnh dưới đây để git clone code về:
                cd ~ && \
                mkdir -p image_processing && \
                git clone -b 'v19.9' --single-branch https://github.com/davisking/dlib.git image_processing/ && \
                cd  dlib/ && \
                python3 setup.py install --yes USE_AVX_INSTRUCTIONS
