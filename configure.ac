#
# Input file for autoconf
#
# Copyright (C) 2011 Francesco Salvestrini
#
# This program is free software; you can redistribute it and/or modify
# it under the terms of the GNU General Public License as published by
# the Free Software Foundation; either version 2 of the License, or
# (at your option) any later version.
#
# This program is distributed in the hope that it will be useful,
# but WITHOUT ANY WARRANTY; without even the implied warranty of
# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
# GNU General Public License for more details.
#
# You should have received a copy of the GNU General Public License along
# with this program; if not, write to the Free Software Foundation, Inc.,
# 51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA.
#

AC_INIT([sumr],[m4_esyscmd(build-aux/git-version-gen .tarball-version)],[salvestrini@gmail.com],[sumr])

AC_PREREQ([2.65])

AC_CONFIG_HEADERS([src/config.h])
AC_CONFIG_SRCDIR([src/sumr.c])
AC_CONFIG_AUX_DIR([build-aux])
AC_CONFIG_MACRO_DIR([m4])

AC_CANONICAL_BUILD
AC_CANONICAL_HOST
AC_CANONICAL_TARGET

AM_INIT_AUTOMAKE([1.11 foreign no-installman no-installinfo -Wall])

AC_PROG_SED
AC_PROG_GREP

AC_PATH_PROG([SORT], [sort])
AC_PATH_PROG([UNIQ], [uniq])
AC_PATH_PROG([GIT],  [git])

AC_PROG_CPP
AC_PROG_CC
AM_PROG_CC_C_O

AC_CONFIG_FILES([
  Makefile
  src/Makefile
])

AC_OUTPUT
