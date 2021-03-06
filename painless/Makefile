all:
	##################################################
	###               MapleCOMSPS                  ###
	##################################################
	cd mapleCOMSPS && tar zxvf m4ri-20140914.tar.gz
	cd mapleCOMSPS/m4ri-20140914 && ./configure
	+ $(MAKE) -C mapleCOMSPS/m4ri-20140914
	+ $(MAKE) -C mapleCOMSPS

	##################################################
	###                 PaInleSS                   ###
	##################################################
	+ $(MAKE) -C painless-src
	mv painless-src/painless painless-mcomsps

clean:
	##################################################
	###               MapleCOMSPS                  ###
	##################################################
	rm -rf mapleCOMSPS/m4ri-20140914
	+ $(MAKE) -C mapleCOMSPS clean

	##################################################
	###                 PaInleSS                   ###
	##################################################
	+ $(MAKE) clean -C painless-src
	rm -f painless-mcomsps
