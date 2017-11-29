#!/bin/sh
##### rcsid = @(#)$Id: mksbtdx,v 1.16 2010-04-12 18:04:30 rathc Exp $
#####
##
##	mksbtdx - Produce a songbook style .tdx file from a .tIdx file.
##
##      Version 4.5, 30 April, 2010
##
##      Copyright 1992--2010 Christopher Rath <christopher@rath.ca>
##
##	This package is free software; you can redistribute it and/or
##	modify it under the terms of version 2.1 of the GNU Lesser
##	General Public License as published by the Free Software
##	Foundation.
##
##	This package is distributed in the hope that it will be
##	useful, but WITHOUT ANY WARRANTY; without even the implied
##	warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR
##	PURPOSE.  See the GNU Lesser General Public License for more
##	details.
##
##	Take a .tIdx file produced by one of the songbook styles and
##	turn it into a .tdx file for final formatting into a title and
##	first line index.
##
#####
#####

###
# Check that the proper parameters were input.
###
if [ "$1" = "" ]
then
  echo USAGE: $0 jobname
fi

###
# Call makeindex to do the required munging.
##
makeindex -s songbook.ist -o $1.tdx $1.tIdx

###
# Tell the user what the new filename is.
###
echo " "
echo "The new Index file is called \`$1.tdx'."

###
# End of script.
###
