# PKGBUILDs
##### Package descriptions for the Arch Linux distribution and its spins.

  This is a catalogue of package descriptions with the intent of: patching issues in packages released to the public by the distribution's maintainers, updating packages in the AUR or customizing them to better meet my own needs. One has adhered to the Arch packaging standards (https://wiki.archlinux.org/index.php/Arch_packaging_standards) as closely as possible.
  The Arch wiki article on creating packages (https://wiki.archlinux.org/index.php/creating_packages) and the PKGBUILD manual page (https://www.archlinux.org/pacman/PKGBUILD.5.html) should be used as primary references and will answer most questions.

### Table of Contents
* **binutils**: Package description for 2.26-3 from the Core repo rolled forward to a more recent commit in the 2.26 branch which includes a patch for ar which rejects arcives with a zero-size file (https://sourceware.org/bugzilla/show_bug.cgi?id=19775). Patched ar is necessary when building herloom* packages.
* **cadence-git**: Customized recipe for building cadence from the master branch at github. Optional dependencies are clearer and package versioning is more conducive to detecting updates than the AUR package which abuses the epoch variable.
* **carla-git**: Reworked PKGBUILD from the AUR that more accurately represents the software's dependencies.
* **heirloom-cvs**: Package description for the Heirloom Toolchest that has been modified to isolate the package's files in more self-contained location: (/opt/heirloom). Package licences were edited to include ALL of the licences the software ships with.
* **heirloom-devtools-cvs**: Package description for the Heirloom Development Tools that has been modified to isolate the package's files in more self-contained location: (/opt/heirloom). Dependency array was expanded to include gcc-libs. Package licences were edited to include ALL of the licences the software ships with.
* **heirloom-doctools-cvs**: Package description for the Heirloom Documentation Tools that has been modified to isolate the package's files in more self-contained location: (/opt/heirloom). Dependency array added including gcc-libs and heirloom-sh-cvs. Package licences were edited to include ALL of the licences the software ships with.
* **heirloom-sh-cvs**: Package description for the Heirloom Bourne Shell that has been modified to isolate the package's files in more self-contained location: (/opt/heirloom). Dependency array added with glibc as its first entry.