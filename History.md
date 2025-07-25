# 0.3.0 / 05.07.2025

* Use simple_xlsx_reader insted of RubyXL to speed up comparision
* Use standardrb to format the code
* Added minimal ruby-version and license to gemspec
* Removed testing and code for Swissmedic-Packages older than 2019
* Remove obsolete file setup.rb
* Replaced pry by debug

# 0.2.9 / 07.01.2025

* Eliminated warning because of frozen string under Ruby 3.4
* Added devenv environment for Ruby 3.4 (see https://devenv.sh/)

# 0.2.8 / 04.10.2023

* Fix problem when expiration_date is a string 'Unbegrenzt'
* Updated tests
* Added Ruby 3.2 for running github/workflow tests

# 0.2.7 / 13.03.2019

* Set date to nil when expiration_date is a string 'Unbegrenzt'

# 0.2.6 / 13.02.2019

* Adapt to swissmedic new XLSX files

# 0.2.5 / 05.02.2018

* Adapte to swissmedic fixing a typo for betäubunsmittel
* Run travis tests for ruby 2.5, too

# 0.2.3 / 25.09.2017

* Fix comparing Date cells
* Run travis tests for ruby 2.3 and 2.4

# 0.2.2 / 11.01.2016

* Don't fail if date cells are nil
* Show version of gem with -h
* Use /usr/bin/env ruby to get actual ruby. Was fixed to outdated /usr/bin/ruby18
* Run travis tests for ruby 2.2.3, too.

# 0.2.1 / 06.07.2015

* Fix problems comparing dates (using to_date.start)
* Assume nothing has changed when comparing nil with an emtpy string
* Revert nr of paramenters of diff method to previous version, to make oddb.org happy again

# 0.2.0 / 03.07.2015

* Abort if Swissmedic introduces incompatible header lines
* Support new format of SwissMedic July 2015
* Reworked compating xlsx-files
* Remove support for old .xls-format (used before 2013)

# 0.1.9 / 08.06.2015

* Swissmedic has different header lines

# 0.1.8 / 07.07.2014

* Support parsing xlsx of Swissmedic July

# 0.1.7 / 15.01.2014

* Support comparing xls and xslx files
* Must use rubyzip 0.9.9 to support all ruby versions
* Added debugger to Gemfile

# 0.1.6 / 14.01.2014

* Added test/data/Packungen-2014.xlsx
* Added missing dependencies for rubyXL
* Moved VERSION to separate file
* Use rubyXL for xslx files

# 0.1.5 / 11.12.2013

* Updated tests as we no longer raise an error
* Update to spreadsheet 0.9.6
* Just display unhandled line instead of raising an exception
* daily_travis_ci.rb on 20131124
* updated Manifest.txt

# 0.1.4 / 22.10.2010

* Add utility proc rows_to_skip
* Forced version in gemspec to 0.1.4
* Refactored. Added utility each_valid_row

# 0.1.3 / 16.8.2010

* Swissmedic_Packungen without 'Gruppe'

* Version 0.1.3 is capable of the Packungen.xls without column 'Gruppe',
  column E in the previous format. If you want to use Packunge.xls
  including the column 'Gruppe', you should use version 0.1.2. After
  you get the source code via Git command, type in the swissmedic-diff
  directory as follows:

* git checkout 4c8c9323297453c3cb3380a9d41457d534ed8861
  Then you can get the version 0.1.2.
