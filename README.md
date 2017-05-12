Brilliant Fantastic Business
============================

A repository of all the important business papers running Brilliant Fantastic as a consultantcy. For the world to see.

## BUSINESS PAPERS

* [Support Contract](contracts/support_contract.md)

## INSTALLATION

These important business papers are written in markdown, also known as god's format. To convert these to a sendable format, we can take advantage of [Pandoc](http://pandoc.org/).

You need Ruby and a clone of this repo locally to convert the documents.

### Prerequisites

* [Ruby](http://ruby-lang.org)
* [Git](https://git-scm.com/)
* [Pandoc](http://pandoc.org) - You can run `brew install pandoc` in order to install it.
* [BasicTeX](http://www.tug.org/mactex/morepackages.html)
* [Bundler](http://bundler.io/) - You can run `gem install bundler` in order to install it.

## CONVERTING TO PDF

* Clone the repo

```
git clone https://github.com/brilliantfantastic/business.git
```

* Install the gems

```
bundle install
```

* Run the rake task

```
rake "convert[contracts/support_contract.md]"
```

The output is placed in the `/output` directory as the name of the document.
