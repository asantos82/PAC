Instalation of PAC in Fedora25

user# wget https://netcologne.dl.sourceforge.net/project/pacmanager/pac-4.0/pac-4.5.5.7-all.deb
user# sudo dnf install glib2-devel gtk2-devel vte-devel

root# cpan Glib::MakeHelper
root# cpan Gnome2::Vte
root# wget http://search.cpan.org/CPAN/authors/id/X/XA/XAOC/Gnome2-Vte-0.11.tar.gz
root# tar xfz Gnome2-Vte-0.11.tar.gz
root# cd Gnome2-Vte-0.11/
root# perl Makefile.PL
root# make
user# sudo cp -f /root/Gnome2-Vte-0.11/blib/arch/auto/Gnome2/Vte/Vte.so /opt/pac/lib/ex/vte64/auto/Gnome2/Vte/
