#!/bin/bash

if [ _$1 == _ ]
then
	echo "Usage: ./vpn.sh [<login> [all]|info|kill]"
fi

if [[ _$1 =~ _[a-z] ]]
then
	if [ _$2 == '_all' ]
	then
		f5fpc -s -t vpn.univie.ac.at:8443 -u $1
	elif [ _$1 == '_kill' ]
	then
		f5fpc -o
	elif [ _$1 == '_info' ]
	then
		f5fpc --info
	else
		f5fpc -s -t vpn.univie.ac.at -u $1
	fi
fi

