# PEBKAC: a smart error database

## alternative name: REVKAS (PEBKAC pronounced as cyrillic)?

##Rough Sketch of Idea

Basically the idea is to have a database of errors which are easily searchable despite the details of those errors. Sometimes 


##Some Error Examples of Errors (need some more obscure ones)

Clojure

 * `java.lang.ClassNotFoundException: link_dataflow.models.maxwell.MaxwellEvent, compiling:(tables.clj:1:1)`
 * `RuntimeException Unmatched delimiter: )  clojure.lang.Util.runtimeException (Util.java:221)`
 * `NumberFormatException Invalid number: 1+  clojure.lang.LispReader.readNumber (LispReader.java:330)`

Python

 * `AttributeError: 'str' object has no attribute 'bar'`
 * `TypeError: can't multiply sequence by non-int of type 'float'`

JS
 * `GET http://e1.cdn.qnsr.com/cgi/b/935613,95910/95850/tx.js net::ERR_BLOCKED_BY_CLIENT`
 * `(program):1 Uncaught ReferenceError: Require is not defined`
 * `Failed to load resource: the server responded with a status of 404 (Not Found)`
 * `(index):1825 Uncaught ReferenceError: CN is not defined`
 * `s-code-contents-566dcf5….js:1647 Uncaught TypeError: Cannot read property 'split' of undefined`

##Possible Approaches to a Better Error Database?

 * [Edit-distance](https://en.wikipedia.org/wiki/Edit_distance) based search. This might alleviate some work in terms of de-specifying your errors for google's sake.
 * Parsers for classes of errors? Lots of work but it'd be pretty solid in terms of how good the answers could be. Could even auto-generate recommendations.

