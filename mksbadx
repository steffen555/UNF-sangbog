#!/bin/sh
##### rcsid = @(#)$Id: mksbkdx,v 1.10 2003/08/19 23:30:36 christopher Exp $
#####
##
##	mksbadx - Produce a songbook style .adx file from a .aIdx file.
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
##	Take a .aIdx file produced by one of the songbook styles and
##	turn it into a .adx file for final formatting into an index 
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
makeindex -s songbook.ist -o $1.adx $1.aIdx

###
# Tell the user what the new filename is.
###
echo " "
echo "The new Index file is called \`$1.adx'."

###
# End of script.
###
