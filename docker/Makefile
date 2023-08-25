all: help

help:
	@echo ""
	@echo "-- Help Menu"
	@echo ""
	@echo "   1. make build              - build all images"
	# @echo "   1. make pull             - pull all images"
	@echo "   1. make clean              - remove all images"
	@echo ""

build:
	@docker build --tag ros:vins-mono -f ./Dockerfile ..

clean:
	@docker rmi -f ros:vins-mono	
# docker build --tag ros:vins-mono -f ./Dockerfile .
# docker run -it --net=host -v /home/snow_dwq/warehouse_ws:/root/warehouse/ \
				-v /tmp/.X11-unix:/tmp/.X11-unix \
                -v /mnt/wslg:/mnt/wslg \
                -e DISPLAY \
                -e WAYLAND_DISPLAY \
                -e XDG_RUNTIME_DIR \
                -e PULSE_SERVER \
				ros:vins-mono  /bin/bash