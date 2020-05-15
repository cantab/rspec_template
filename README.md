# RSpec Template

## About the RSpec Template

A template to start Test Driven Development with the RSpec testing framework

## How to Use the Template

Clone this git repository

  	git clone git@github.com:cantab/rspec_template.git

go into the new app directory

  	cd rspec_template

install the RSpec gem

  	bundle install

you may also need to install the rspec binary

	bundle binstubs rspec-core

### Installing Gems

Add any gems the project requires in the Gemfile, then run

  	bundle install

### Writing Examples

Write your tests in separate example files in the spec/ directory. The name of each example file must end with _spec.rb for RSpec to pick it up.

I've put a sample example file in spec/changeme_spec.rb to start you off, and you can put your examples there to start with.

You can rename this file to whatever you like, but remember the filename must end with _spec.rb.

As you continue developing your project, you may find it more sensible to split your examples into separate files in the /spec directory.

### Writing Code

Write your code in separate code files in the lib/ directory. The name of each code file must have an .rb extension for your tests and code to work.

I've put a sample code file in lib/changeme.rb to start you off, and you can put your code there to start with.

You can rename this file to whatever you like, but remember the filename must end with .rb.

As you continue developing your project, you may find it more sensible to split your code into separate files in the lib/ directory; just make sure each of these files is required in the spec_helper file (see below), so that your tests can run properly.

### Spec Helper File

If you open the example file, you will see a line "require 'spec\_helper'" at the top of each file. This loads the spec/spec\_helper.rb file. At the top of the spec_helper.rb file, each of the code files is required. This allows the correct environment to be set up for the examples to run.

If you add further code files (see above), make sure you add the corresponding "require" line in the spec_helper.rb file

You can also add any other setup you need to run that is relevant for all examples in the spec_helper.rb file.

### Running Your Examples

  	bundle exec rspec spec

or

	rake spec

## Contact

Comments, patches, Git pull requests and bug reports are welcome.

## License

Copyright (c) 2014 Chong-Yee Khoo. All rights reserved.

MIT License

Permission is hereby granted, free of charge, to any person obtaining
a copy of this software and associated documentation files (the
"Software"), to deal in the Software without restriction, including
without limitation the rights to use, copy, modify, merge, publish,
distribute, sublicense, and/or sell copies of the Software, and to
permit persons to whom the Software is furnished to do so, subject to
the following conditions:

The above copyright notice and this permission notice shall be
included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE
LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION
WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
