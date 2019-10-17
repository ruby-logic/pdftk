Pdftk
=====

**This gem is a fork of [Pdftk by WebKrak](https://github.com/webkrak/pdftk), modified to work with Ruby 2.3.**  
The original gem uses `win32/open3` if it detects `mingw` environment and Ruby newer than 1.9.  
Ruby 2.3 ships with open3, so this behaviour is no longer needed.

Pdftk is gem for merging pdf files with pdftk library for Rails.

### Installation

Configure it in an initializer:

    Pdftk.config = {
      :exe_path => '/usr/local/bin/pdftk'
    }

Add the gem to your `Gemfile`

    gem 'pdftk', github: 'ruby-logic/pdftk'

### Basic Usage

Is a example of usage:

    pdf = Pdftk.new.merge(array_with_files_path_to_merging, output_file_path)

