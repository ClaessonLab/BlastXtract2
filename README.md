# BlastXtract2

--INTRODUCTION--

Searches of translated un-annotated genomic DNA sequences against protein
databases is a useful early-stage method for discovering protein homologues
encoded by the sequence, but generates huge amounts of output data that
quickly becomes impregnable. BlastXtract is a web-based tool for managing
and visualizing results from large translated BLAST, FastA, Blat and Pauda searches.
It combines the speed and storage benefits of Relational Database Management
Systems with an easy-to-use graphical navigation map, and greatly facilitates
the early exploration of genomic sequence.
 
More information can be obtained at
http://bioinfo.ucc.ie/cgi-bin/blastXtract2/
 
--INSTALLATION--
 
BlastXtract2 is developed using Perl 5.8.0 on the Linux Ubuntu 12.0 operating
system. 
 
To install BlastXtract, make sure you have permission to write to the cgi-
enabled directory to create databases in MySQL/PostgreSQL, which should be
up and running. Then run the installation program
 
blastXtract2_install.pl
 
This script checks that all the perl modules are installed, sets a few installation
parameters, creates the MySQL/PostgreSQL database and copies the modified program
to the appropriate webserver destination.
 
--IMPORTANT NOTES--
 
In the Apache configuration file, set TimeOut to at least 600, since large
output files can take long time to upload.
 
If installing the DBD::mysql module make sure to also have mysql-server,
mysql-devel, zlib and zlib-devel installed. Also do 'unset LANG' or 'LANG="c"'
before compiling the module.
 
--COPYRIGHT--
 
Copyright (C) 2015 Genome Research Limited
 
This program is free software; you can redistribute it and/or
modify it under the terms of the GNU General Public License
as published by the Free Software Foundation; either version 2
of the License, or (at your option) any later version.
 
This program is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
GNU General Public License for more details.
 
You should have received a copy of the GNU General Public License
along with this program; if not, write to the Free Software
Foundation, Inc., 59 Temple Place - Suite 330, Boston, MA  02111-1307, USA.
 
--CONTACT INFORMATION--
 
If you have any questions, complaints, or suggestions, please email them to
 
Marcus Claesson
E-mail: mclaesson@bioinfo.ucc.ie
 
Department of Microbiology,
National University of Ireland,
Cork, Ireland
 
Last Revised February 15, 2015
