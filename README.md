Brilliant Fantastic Business
============================

A repository of all the important business papers running Brilliant Fantastic as a consultantcy. For the world to see.

## BUSINESS PAPERS

* [Support Contract](contracts/support_contract.md)

## CONVERTING TO PDF

These important business papers are written in markdown, also known as god's format. To convert these to a sendable format, we can take advantage of [Pandoc](http://pandoc.org/).

You need Ruby and a clone of this repo locally to convert the documents. You will also need to install the `rake` gem to make this happen.

There is a Rake task that allows us to convert any of these documents one at a time. In order to convert these documents to PDF, try running the following:

```
rake "convert[pdf, contracts/support_contract.md]"
```
