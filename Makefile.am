##
## Description  : vk_renderer - Makefile.am
## Author       : DRE 2024
## Purpose      : main Makefile
## Revision     : $Id: Makefile.am,v 1.12 2008/12/02 20:49:08 cvsuser Exp $
##

# DRE 2022 : the subdirectories alert for automake 
# NOTE: Every line ends in a Carriage Return
SUBDIRS = nuklear-glfw-vulkan/ demo/ example/ 


# DRE2022 - a generic aclocal flag set for m4 files
ACLOCAL_AMFLAGS = -I m4


AM_CFLAGS 		= 
AM_LDFLAGS		= 

# the executable program vk-oit vulkan order independent transparecy 
bin_PROGRAMS =
# DRE 2022 this command tells libtool to build a library called 
lib_LTLIBRARIES = libvk_render.la

# library's source files - added one per line but no headers
libvk_render_la_SOURCES =   
						
# ENDS WITH CARRIAGE RETURN LAST LINE

# DRE 2022 - Libraries LIBADD (Libraries ADD) while programs LDADD which means linker daemon (ld) ADD
libvk_render_la_LDFLAGS =  
 
libvk_render_la_LIBADD = 



# DRE 2022 - target recipe makes doxygen outputs, after updating config format file
dox:
	doxygen
#
create-dox:
	doxygen -g 



