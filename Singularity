Bootstrap: docker
From: alpine

%post
	apk update
	apk add wget
	wget http://github.com/bbuchfink/diamond/releases/download/v0.9.22/diamond-linux64.tar.gz
	tar xzf diamond-linux64.tar.gz
	wget https://raw.githubusercontent.com/upendrak/diamond_blast_docker/master/mouse.1.protein.faa
	wget https://raw.githubusercontent.com/upendrak/diamond_blast_docker/master/zebrafish.1.protein.faa

%environment
	export PATH=/:$PATH

%runscript
	diamond


## Sample Singularity file created during NSF Cyber Carpentry 2018. Parts taken from the original Diamond dockerfile and lecture notes.
