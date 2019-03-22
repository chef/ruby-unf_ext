## Note

This is a fork of the main project, to fix AIX compilation flags.  It sets the versiont to 0.0.7.6, which may not exist on rubygems. This is consumed by the InSpec project, see https://github.com/inspec/inspec/issues/2873 and https://github.com/inspec/inspec/issues/3901


ruby-unf_ext
============

Synopsis
--------

* Unicode Normalization Form support library for CRuby

Description
-----------

* Normalizes UTF-8 strings into and from NFC, NFD, NFKC or NFKD

        # For bulk conversion
        normalizer = UNF::Normalizer.new
        a_bunch_of_strings.map! { |string|
          normalizer.normalize(string, :nfc) #=> string in NFC
        }

* Compliant with Unicode 9.0

Requirement
-----------

* Ruby 1.8.7+, 1.9.2+

* C++ compiler and libstdc++

Installation
------------

	gem install unf_ext

Or:

    ruby extconf.rb && make && make install

Development Resources
---------------------

* https://github.com/sile/unf

    For issues regarding files under the directory `unf`, please
    contact this upstream.

* https://github.com/knu/ruby-unf_ext

    The development site and the repository.

License
-------

Copyright (c) 2010-2017 Takeru Ohta
Copyright (c) 2011-2018 Akinori MUSHA

Licensed under the MIT license.
See `LICENSE` for details.
