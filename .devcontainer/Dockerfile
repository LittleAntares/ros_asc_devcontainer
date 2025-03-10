# Start from the ROS Noetic Desktop container you mentioned
FROM devrt/ros-devcontainer-vscode:noetic-desktop

# Install additional tools or packages
USER root
RUN apt-get update && apt-get install -y --no-install-recommends \
    vim \
    git \
    mosh \
    libi2c-dev \
    i2c-tools  \
    gpiod \
    libgpiod-dev \
    libgpiod-doc \ 
    v4l-utils \
    libv4l-dev \
    qv4l2 \
    uvcdynctrl \
    libcanberra-gtk0 \
    libcanberra-gtk-module \
    && rm -rf /var/lib/apt/lists/*

RUN pip3 install --upgrade pip && pip3 install --upgrade setuptools wheel
RUN pip3 install --upgrade numpy && pip3 install opencv-contrib-python



