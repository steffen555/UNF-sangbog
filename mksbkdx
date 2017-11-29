#!/bin/sh
##### rcsid = @(#)$Id: mksbkdx,v 1.14 2010-04-12 18:04:30 rathc Exp $
#####
##
##	mksbkdx - Produce a songbook style .kdx file from a .kIdx file.
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
##	Take a .kIdx file produced by one of the songbook styles and
##	turn it into a .kdx file for final formatting into an index 
##	of songs by key.
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
makeindex -s songbook.ist -o $1.kdx $1.kIdx

###
# Tell the user what the new filename is.
###
echo " "
echo "The new Index file is called \`$1.kdx'."

###
# End of script.
###
