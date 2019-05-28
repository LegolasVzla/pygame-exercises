FROM python:3

# Set the working directory
WORKDIR /DefeatTheBat

COPY bat.png main.py wallpaper.jpg requirements.txt ./

RUN apt-get update && apt-get install -y \
	python3-dev -y \ 
	python3-setuptools -y \ 
	python3-numpy -y \ 
	python3-opengl -y  \ 
	libsdl-image1.2-dev -y \ 
	libsdl-mixer1.2-dev -y \ 
	libsdl-ttf2.0-dev -y \ 
	libsmpeg-dev -y \ 
	libsdl1.2-dev -y \ 
	libportmidi-dev -y \ 
	libswscale-dev -y \ 
	libavformat-dev -y \ 
	libavcodec-dev -y \ 
	libtiff5-dev -y \ 
	libx11-6 -y \ 
	libx11-dev -y \ 
	fluid-soundfont-gm -y \ 
	timgm6mb-soundfont -y \ 
	xfonts-base -y \ 
	xfonts-100dpi -y \ 
	xfonts-75dpi -y \ 
	xfonts-cyrillic -y \ 
	fontconfig -y \ 
	fonts-freefont-ttf -y \ 
	libfreetype6-dev -y

# Install any needed packages specified in requirements.txt
RUN pip install --no-cache-dir -r requirements.txt

CMD [ "python", "./main.py" ]
