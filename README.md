Simple debian helper to append some build environment info into
the control file. This is mostly so we can tag the git
repository after the fact, once we decide a given package
is acceptable for release. TO use, add --with bbm-info to 
your dh call in debian/rules:

  %:
    dh $@ --with bbm-info
        

