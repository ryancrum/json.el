# JSON.el


This is a library for parsing and generating JSON (JavaScript Object
Notation).

Learn all about JSON here: [http://json.org/](http://json.org).

The user-serviceable entry points for the parser are the functions
`json-read` and `json-read-from-string`. The encoder has a single
entry point, `json-encode`.

Since there are several natural representations of key-value pair
mappings in elisp (alist, plist, hash-table), `json-read' allows you
to specify which you'd prefer (see `json-object-type` and
`json-array-type`).

Similarly, since `false` and `null` are distinct in JSON, you can
distinguish them by binding `json-false` and `json-null` as desired.
