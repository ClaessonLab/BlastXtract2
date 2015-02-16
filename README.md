# BlastXtract2

--INTRODUCTION--

BlastXtract2 facilitates early exploration of un-annotated genomic and metagenomic sequences. Various formats of translated searches of multiple sequences against multiple protein databases can be uploaded to a MySQL server accessed by a locally installed BlastXtract2 web-server. There, an intuitive GUI allows straightforward data-mining and enables quick detection of potential frameshifts and poorly sequenced/assembled regions.

Before installing feel free to test a demo version at
http://bioinfo.ucc.ie/cgi-bin/blastXtract2/blastXtract2.pl

--INSTALLATION--

BlastXtract2 is developed using Perl 5.8.0 on the Linux Ubuntu 12.0 operating system. 
To install BlastXtract, make sure you have permission to write to the cgi-enabled directory to create databases in MySQL/PostgreSQL, which should be up and running. Then run the installation program blastXtract2_install.pl 
This script checks that all the perl modules are installed, sets a few installation parameters, creates the MySQL/PostgreSQL database and copies the modified program to the appropriate webserver destination.
 
--IMPORTANT NOTES--

In the Apache configuration file, set TimeOut to at least 600, since large output files can take long time to upload. If installing the DBD::mysql module make sure to also have mysql-server,
mysql-devel, zlib and zlib-devel installed. Also do 'unset LANG' or 'LANG="c"' before compiling the module.

--MODIFICATION OF COG DATABASE--

The original COG database at ftp://ftp.ncbi.nih.gov/pub/COG/COG can be modified so that COG categories are visible in BLASTx output results and can be colour-coded and summarised in BlastXtract2. To do this, follow instructions in 'how_COGdb_was_created'.

--COPYRIGHT--

Copyright (C) 2015 Genome Research Limited
 
This program is free software; you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation; either version 2 of the License, or (at your option) any later version. 
This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU General Public License for more details. You should have received a copy of the GNU General Public License along with this program; if not, write to the Free Software Foundation, Inc., 59 Temple Place - Suite 330, Boston, MA  02111-1307, USA.

--CONTACT INFORMATION—

If you have any questions, complaints, or suggestions, please email them to
Marcus Claesson
E-mail: m.claesson@ucc.ie
School of Microbiology,
University College Cork,
Cork, Ireland
Last Revised February 16, 2015
