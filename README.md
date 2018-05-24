-------------------------------------------------------------------------------
What organization or people are asking to have this signed:
-------------------------------------------------------------------------------
Oracle

-------------------------------------------------------------------------------
What product or service is this for:
-------------------------------------------------------------------------------
Solaris 

-------------------------------------------------------------------------------
What's the justification that this really does need to be signed for the whole world to be able to boot it:
-------------------------------------------------------------------------------
This is for secure booting Solaris OS.

-------------------------------------------------------------------------------
Who is the primary contact for security updates, etc.
-------------------------------------------------------------------------------
- Name: Ann Lai	
- Position: Senior Software Engineer
- Email address: ann.lai@oracle.com
- PGP key, signed by the other security contacts, and preferably also with signatures that are reasonably well known in the linux community:
ssh-rsa AAAAB3NzaC1yc2EAAAABIwAAAQEA0KhxFTQr13GAKu7WxcVfccgtUop9hm54kW5gs4d02Z8GlS2gb0/5NDafHrOwf7PTOv6YZUxJqyzlUlkm6uZbtKdPDVKs4o6TmxGlDJsgyVyHqYo9LY4+2cD+i4H5wdgL5nQEd+Uo0ubS34r6Bw1zpiOmPpMZpPRdZpjxWihzULXjMltL/hPy6oG131lSVjby7RFC4HolchO2lKYbP1PqKu2CSIEKCGyoq8VWQK5c3xlOZcX2AwWO3sueRi/641HHhDhWIy/ERIvuErDr6DXBz7xoyCDjHA1zn6ovVJ80ZAAluPi0kRhOoKTJ+rebdjUcejGjeK4iPsjlALF+vjbxsQ== adlai@sanpen-csx12-0

-------------------------------------------------------------------------------
Who is the secondary contact for security updates, etc.
-------------------------------------------------------------------------------
- Name: David Marx
- Position: Principal Software Engineer
- Email address: david.m.marx@oracle.com
- PGP key, signed by the other security contacts, and preferably also with signatures that are reasonably well known in the linux community:

-------------------------------------------------------------------------------
What upstream shim tag is this starting from:
-------------------------------------------------------------------------------
shim 0.9

-------------------------------------------------------------------------------
URL for a repo that contains the exact code which was built to get this binary:
-------------------------------------------------------------------------------
We didn't build the exact code from upstream.  We had to make modification to upstream shim for it to work in Solaris.

-------------------------------------------------------------------------------
What patches are being applied and why:
-------------------------------------------------------------------------------
Multiple patches were applied so the shim can work in Solaris.  We #ifdef all the changes we made.

-------------------------------------------------------------------------------
What OS and toolchain must we use to reproduce this build?  Include where to find it, etc.  We're going to try to reproduce your build as close as possible to verify that it's really a build of the source tree you tell us it is, so these need to be fairly thorough. At the very least include the specific versions of gcc, binutils, and gnu-efi which were used, and where to find those binaries.
-------------------------------------------------------------------------------
Solaris 11.4
gcc 5.5.0 http://ftp.gnu.org/gnu/gcc/gcc-5.4.0/gcc-5.4.0.tar.gz
E)
gnu-efi 3.0 http://sourceforge.net/projects/gnu-efi/files/gnu-efi_3.0u.orig.tar.gz/download
binutils 2.29 http://ftp.gnu.org/gnu/binutils/binutils-2.29.tar.bz2

-------------------------------------------------------------------------------
Which files in this repo are the logs for your build?   This should include logs for creating the buildroots, applying patches, doing the build, creating the archives, etc.
-------------------------------------------------------------------------------
build.log

-------------------------------------------------------------------------------
Put info about what bootloader you're using, including which patches it includes to enforce Secure Boot here:
-------------------------------------------------------------------------------
Our bootloader is GRUB 2. 

-------------------------------------------------------------------------------
Put info about what kernel you're using, including which patches it includes to enforce Secure Boot here:
-------------------------------------------------------------------------------
Solaris kernel.

