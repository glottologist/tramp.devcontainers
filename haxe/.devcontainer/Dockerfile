FROM glottologist/development-ubuntu:19.12.3
ADD README.md .
RUN apt-get install -y software-properties-common
RUN add-apt-repository ppa:haxe/releases -y 
RUN apt-get update
RUN apt-get install haxe -y 
RUN mkdir ~/haxelib && haxelib setup ~/haxelib

