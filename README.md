# api documentation for  [htmlparser (v1.7.7)](http://github.com/tautologistics/node-htmlparser)  [![npm package](https://img.shields.io/npm/v/npmdoc-htmlparser.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-htmlparser) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-htmlparser.svg)](https://travis-ci.org/npmdoc/node-npmdoc-htmlparser)
#### Forgiving HTML/XML/RSS Parser in JS for *both* Node and Browsers

[![NPM](https://nodei.co/npm/htmlparser.png?downloads=true)](https://www.npmjs.com/package/htmlparser)

[![apidoc](https://npmdoc.github.io/node-npmdoc-htmlparser/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-htmlparser_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-htmlparser/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-htmlparser/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-htmlparser/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Chris Winberry",
        "email": "chris@winberry.net"
    },
    "bugs": {
        "url": "http://github.com/tautologistics/node-htmlparser/issues"
    },
    "contributors": [],
    "dependencies": {},
    "description": "Forgiving HTML/XML/RSS Parser in JS for *both* Node and Browsers",
    "devDependencies": {},
    "directories": {
        "lib": "./lib/"
    },
    "dist": {
        "shasum": "19e7b3997ff6fbac99ae5a7d2766489efe7e2d0e",
        "tarball": "https://registry.npmjs.org/htmlparser/-/htmlparser-1.7.7.tgz"
    },
    "engines": {
        "node": ">=0.1.33"
    },
    "homepage": "http://github.com/tautologistics/node-htmlparser",
    "keywords": [
        "html",
        "xml",
        "rss",
        "parser"
    ],
    "licenses": [
        {
            "type": "MIT",
            "url": "http://github.com/tautologistics/node-htmlparser/raw/master/LICENSE"
        }
    ],
    "main": "./lib/htmlparser",
    "maintainers": [
        {
            "name": "tautologistics",
            "email": "chris@winberry.net"
        }
    ],
    "name": "htmlparser",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+https://github.com/tautologistics/node-htmlparser.git"
    },
    "version": "1.7.7"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module htmlparser](#apidoc.module.htmlparser)
1.  [function <span class="apidocSignatureSpan">htmlparser.</span>DefaultHandler (callback, options)](#apidoc.element.htmlparser.DefaultHandler)
1.  [function <span class="apidocSignatureSpan">htmlparser.</span>Parser (handler, options)](#apidoc.element.htmlparser.Parser)
1.  [function <span class="apidocSignatureSpan">htmlparser.</span>RssHandler (callback)](#apidoc.element.htmlparser.RssHandler)
1.  object <span class="apidocSignatureSpan">htmlparser.</span>DefaultHandler.prototype
1.  object <span class="apidocSignatureSpan">htmlparser.</span>DomUtils
1.  object <span class="apidocSignatureSpan">htmlparser.</span>ElementType
1.  object <span class="apidocSignatureSpan">htmlparser.</span>Parser.prototype
1.  object <span class="apidocSignatureSpan">htmlparser.</span>RssHandler.prototype
1.  object <span class="apidocSignatureSpan">htmlparser.</span>node_htmlparser

#### [module htmlparser.DefaultHandler](#apidoc.module.htmlparser.DefaultHandler)
1.  [function <span class="apidocSignatureSpan">htmlparser.</span>DefaultHandler (callback, options)](#apidoc.element.htmlparser.DefaultHandler.DefaultHandler)
1.  object <span class="apidocSignatureSpan">htmlparser.DefaultHandler.</span>_emptyTags
1.  object <span class="apidocSignatureSpan">htmlparser.DefaultHandler.</span>reWhitespace

#### [module htmlparser.DefaultHandler.prototype](#apidoc.module.htmlparser.DefaultHandler.prototype)
1.  boolean <span class="apidocSignatureSpan">htmlparser.DefaultHandler.prototype.</span>_done
1.  [function <span class="apidocSignatureSpan">htmlparser.DefaultHandler.prototype.</span>done ()](#apidoc.element.htmlparser.DefaultHandler.prototype.done)
1.  [function <span class="apidocSignatureSpan">htmlparser.DefaultHandler.prototype.</span>error (error)](#apidoc.element.htmlparser.DefaultHandler.prototype.error)
1.  [function <span class="apidocSignatureSpan">htmlparser.DefaultHandler.prototype.</span>handleCallback (error)](#apidoc.element.htmlparser.DefaultHandler.prototype.handleCallback)
1.  [function <span class="apidocSignatureSpan">htmlparser.DefaultHandler.prototype.</span>handleElement (element)](#apidoc.element.htmlparser.DefaultHandler.prototype.handleElement)
1.  [function <span class="apidocSignatureSpan">htmlparser.DefaultHandler.prototype.</span>isEmptyTag (element)](#apidoc.element.htmlparser.DefaultHandler.prototype.isEmptyTag)
1.  [function <span class="apidocSignatureSpan">htmlparser.DefaultHandler.prototype.</span>reset ()](#apidoc.element.htmlparser.DefaultHandler.prototype.reset)
1.  [function <span class="apidocSignatureSpan">htmlparser.DefaultHandler.prototype.</span>writeComment (element)](#apidoc.element.htmlparser.DefaultHandler.prototype.writeComment)
1.  [function <span class="apidocSignatureSpan">htmlparser.DefaultHandler.prototype.</span>writeDirective (element)](#apidoc.element.htmlparser.DefaultHandler.prototype.writeDirective)
1.  [function <span class="apidocSignatureSpan">htmlparser.DefaultHandler.prototype.</span>writeTag (element)](#apidoc.element.htmlparser.DefaultHandler.prototype.writeTag)
1.  [function <span class="apidocSignatureSpan">htmlparser.DefaultHandler.prototype.</span>writeText (element)](#apidoc.element.htmlparser.DefaultHandler.prototype.writeText)
1.  object <span class="apidocSignatureSpan">htmlparser.DefaultHandler.prototype.</span>_callback
1.  object <span class="apidocSignatureSpan">htmlparser.DefaultHandler.prototype.</span>_options
1.  object <span class="apidocSignatureSpan">htmlparser.DefaultHandler.prototype.</span>_tagStack
1.  object <span class="apidocSignatureSpan">htmlparser.DefaultHandler.prototype.</span>dom

#### [module htmlparser.DomUtils](#apidoc.module.htmlparser.DomUtils)
1.  [function <span class="apidocSignatureSpan">htmlparser.DomUtils.</span>getElementById (id, currentElement, recurse)](#apidoc.element.htmlparser.DomUtils.getElementById)
1.  [function <span class="apidocSignatureSpan">htmlparser.DomUtils.</span>getElements (options, currentElement, recurse, limit)](#apidoc.element.htmlparser.DomUtils.getElements)
1.  [function <span class="apidocSignatureSpan">htmlparser.DomUtils.</span>getElementsByTagName (name, currentElement, recurse, limit)](#apidoc.element.htmlparser.DomUtils.getElementsByTagName)
1.  [function <span class="apidocSignatureSpan">htmlparser.DomUtils.</span>getElementsByTagType (type, currentElement, recurse, limit)](#apidoc.element.htmlparser.DomUtils.getElementsByTagType)
1.  [function <span class="apidocSignatureSpan">htmlparser.DomUtils.</span>testElement (options, element)](#apidoc.element.htmlparser.DomUtils.testElement)

#### [module htmlparser.Parser](#apidoc.module.htmlparser.Parser)
1.  [function <span class="apidocSignatureSpan">htmlparser.</span>Parser (handler, options)](#apidoc.element.htmlparser.Parser.Parser)
1.  object <span class="apidocSignatureSpan">htmlparser.Parser.</span>_reAttrib
1.  object <span class="apidocSignatureSpan">htmlparser.Parser.</span>_reTagName
1.  object <span class="apidocSignatureSpan">htmlparser.Parser.</span>_reTags
1.  object <span class="apidocSignatureSpan">htmlparser.Parser.</span>_reTrim
1.  object <span class="apidocSignatureSpan">htmlparser.Parser.</span>_reTrimComment
1.  object <span class="apidocSignatureSpan">htmlparser.Parser.</span>_reWhitespace

#### [module htmlparser.Parser.prototype](#apidoc.module.htmlparser.Parser.prototype)
1.  boolean <span class="apidocSignatureSpan">htmlparser.Parser.prototype.</span>_done
1.  [function <span class="apidocSignatureSpan">htmlparser.Parser.prototype.</span>done ()](#apidoc.element.htmlparser.Parser.prototype.done)
1.  [function <span class="apidocSignatureSpan">htmlparser.Parser.prototype.</span>getLocation (startTag)](#apidoc.element.htmlparser.Parser.prototype.getLocation)
1.  [function <span class="apidocSignatureSpan">htmlparser.Parser.prototype.</span>handleError (error)](#apidoc.element.htmlparser.Parser.prototype.handleError)
1.  [function <span class="apidocSignatureSpan">htmlparser.Parser.prototype.</span>parseAttribs (element)](#apidoc.element.htmlparser.Parser.prototype.parseAttribs)
1.  [function <span class="apidocSignatureSpan">htmlparser.Parser.prototype.</span>parseChunk (data)](#apidoc.element.htmlparser.Parser.prototype.parseChunk)
1.  [function <span class="apidocSignatureSpan">htmlparser.Parser.prototype.</span>parseComplete (data)](#apidoc.element.htmlparser.Parser.prototype.parseComplete)
1.  [function <span class="apidocSignatureSpan">htmlparser.Parser.prototype.</span>parseTagAttribs (elements)](#apidoc.element.htmlparser.Parser.prototype.parseTagAttribs)
1.  [function <span class="apidocSignatureSpan">htmlparser.Parser.prototype.</span>parseTagName (data)](#apidoc.element.htmlparser.Parser.prototype.parseTagName)
1.  [function <span class="apidocSignatureSpan">htmlparser.Parser.prototype.</span>parseTags ()](#apidoc.element.htmlparser.Parser.prototype.parseTags)
1.  [function <span class="apidocSignatureSpan">htmlparser.Parser.prototype.</span>reset ()](#apidoc.element.htmlparser.Parser.prototype.reset)
1.  [function <span class="apidocSignatureSpan">htmlparser.Parser.prototype.</span>validateHandler (handler)](#apidoc.element.htmlparser.Parser.prototype.validateHandler)
1.  [function <span class="apidocSignatureSpan">htmlparser.Parser.prototype.</span>writeHandler (forceFlush)](#apidoc.element.htmlparser.Parser.prototype.writeHandler)
1.  number <span class="apidocSignatureSpan">htmlparser.Parser.prototype.</span>_current
1.  number <span class="apidocSignatureSpan">htmlparser.Parser.prototype.</span>_elementsCurrent
1.  number <span class="apidocSignatureSpan">htmlparser.Parser.prototype.</span>_next
1.  object <span class="apidocSignatureSpan">htmlparser.Parser.prototype.</span>_buffer
1.  object <span class="apidocSignatureSpan">htmlparser.Parser.prototype.</span>_elements
1.  object <span class="apidocSignatureSpan">htmlparser.Parser.prototype.</span>_handler
1.  object <span class="apidocSignatureSpan">htmlparser.Parser.prototype.</span>_location
1.  object <span class="apidocSignatureSpan">htmlparser.Parser.prototype.</span>_options
1.  object <span class="apidocSignatureSpan">htmlparser.Parser.prototype.</span>_tagStack
1.  string <span class="apidocSignatureSpan">htmlparser.Parser.prototype.</span>_parseState
1.  string <span class="apidocSignatureSpan">htmlparser.Parser.prototype.</span>_prevTagSep

#### [module htmlparser.RssHandler](#apidoc.module.htmlparser.RssHandler)
1.  [function <span class="apidocSignatureSpan">htmlparser.</span>RssHandler (callback)](#apidoc.element.htmlparser.RssHandler.RssHandler)
1.  [function <span class="apidocSignatureSpan">htmlparser.RssHandler.</span>super_ (callback, options)](#apidoc.element.htmlparser.RssHandler.super_)

#### [module htmlparser.RssHandler.prototype](#apidoc.module.htmlparser.RssHandler.prototype)
1.  [function <span class="apidocSignatureSpan">htmlparser.RssHandler.prototype.</span>constructor (callback)](#apidoc.element.htmlparser.RssHandler.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">htmlparser.RssHandler.prototype.</span>done ()](#apidoc.element.htmlparser.RssHandler.prototype.done)

#### [module htmlparser.node_htmlparser](#apidoc.module.htmlparser.node_htmlparser)
1.  [function <span class="apidocSignatureSpan">htmlparser.node_htmlparser.</span>DefaultHandler (callback, options)](#apidoc.element.htmlparser.node_htmlparser.DefaultHandler)
1.  [function <span class="apidocSignatureSpan">htmlparser.node_htmlparser.</span>Parser (handler, options)](#apidoc.element.htmlparser.node_htmlparser.Parser)
1.  [function <span class="apidocSignatureSpan">htmlparser.node_htmlparser.</span>RssHandler (callback)](#apidoc.element.htmlparser.node_htmlparser.RssHandler)
1.  object <span class="apidocSignatureSpan">htmlparser.node_htmlparser.</span>DomUtils
1.  object <span class="apidocSignatureSpan">htmlparser.node_htmlparser.</span>ElementType



# <a name="apidoc.module.htmlparser"></a>[module htmlparser](#apidoc.module.htmlparser)

#### <a name="apidoc.element.htmlparser.DefaultHandler"></a>[function <span class="apidocSignatureSpan">htmlparser.</span>DefaultHandler (callback, options)](#apidoc.element.htmlparser.DefaultHandler)
- description and source-code
```javascript
function DefaultHandler(callback, options) {
	this.reset();
	this._options = options ? options : { };
	if (this._options.ignoreWhitespace == undefined)
		this._options.ignoreWhitespace = false; //Keep whitespace-only text nodes
	if (this._options.verbose == undefined)
		this._options.verbose = true; //Keep data property for tags and raw property for all
	if (this._options.enforceEmptyTags == undefined)
		this._options.enforceEmptyTags = true; //Don't allow children for HTML tags defined as empty in spec
	if ((typeof callback) == "function")
		this._callback = callback;
}
```
- example usage
```shell
...
View runtests.html in any browser

##Usage In Node

'''javascript
var htmlparser = require("htmlparser");
var rawHtml = "Xyz <script language= javascript>var foo = '<<bar>>';< /  script><!--<!-- Waah! -- -->";
var handler = new htmlparser.DefaultHandler(function (error, dom) {
	if (error)
		[...do something for errors...]
	else
		[...parsing done, do something...]
});
var parser = new htmlparser.Parser(handler);
parser.parseComplete(rawHtml);
...
```

#### <a name="apidoc.element.htmlparser.Parser"></a>[function <span class="apidocSignatureSpan">htmlparser.</span>Parser (handler, options)](#apidoc.element.htmlparser.Parser)
- description and source-code
```javascript
function Parser(handler, options) {
	this._options = options ? options : { };
	if (this._options.includeLocation == undefined) {
		this._options.includeLocation = false; //Do not track element position in document by default
	}

	this.validateHandler(handler);
	this._handler = handler;
	this.reset();
}
```
- example usage
```shell
...
var rawHtml = "Xyz <script language= javascript>var foo = '<<bar>>';< /  script><!--<!-- Waah! -- -->";
var handler = new htmlparser.DefaultHandler(function (error, dom) {
	if (error)
		[...do something for errors...]
	else
		[...parsing done, do something...]
});
var parser = new htmlparser.Parser(handler);
parser.parseComplete(rawHtml);
sys.puts(sys.inspect(handler.dom, false, null));
'''

##Usage In Browser

'''javascript
...
```

#### <a name="apidoc.element.htmlparser.RssHandler"></a>[function <span class="apidocSignatureSpan">htmlparser.</span>RssHandler (callback)](#apidoc.element.htmlparser.RssHandler)
- description and source-code
```javascript
function RssHandler(callback) {
	RssHandler.super_.call(this, callback, { ignoreWhitespace: true, verbose: false, enforceEmptyTags: false });
}
```
- example usage
```shell
...
}
parser.done();	
'''

##Parsing RSS/Atom Feeds

'''javascript
new htmlparser.RssHandler(function (error, dom) {
	...
});
'''

##DefaultHandler Options

###Usage
...
```



# <a name="apidoc.module.htmlparser.DefaultHandler"></a>[module htmlparser.DefaultHandler](#apidoc.module.htmlparser.DefaultHandler)

#### <a name="apidoc.element.htmlparser.DefaultHandler.DefaultHandler"></a>[function <span class="apidocSignatureSpan">htmlparser.</span>DefaultHandler (callback, options)](#apidoc.element.htmlparser.DefaultHandler.DefaultHandler)
- description and source-code
```javascript
function DefaultHandler(callback, options) {
	this.reset();
	this._options = options ? options : { };
	if (this._options.ignoreWhitespace == undefined)
		this._options.ignoreWhitespace = false; //Keep whitespace-only text nodes
	if (this._options.verbose == undefined)
		this._options.verbose = true; //Keep data property for tags and raw property for all
	if (this._options.enforceEmptyTags == undefined)
		this._options.enforceEmptyTags = true; //Don't allow children for HTML tags defined as empty in spec
	if ((typeof callback) == "function")
		this._callback = callback;
}
```
- example usage
```shell
...
View runtests.html in any browser

##Usage In Node

'''javascript
var htmlparser = require("htmlparser");
var rawHtml = "Xyz <script language= javascript>var foo = '<<bar>>';< /  script><!--<!-- Waah! -- -->";
var handler = new htmlparser.DefaultHandler(function (error, dom) {
	if (error)
		[...do something for errors...]
	else
		[...parsing done, do something...]
});
var parser = new htmlparser.Parser(handler);
parser.parseComplete(rawHtml);
...
```



# <a name="apidoc.module.htmlparser.DefaultHandler.prototype"></a>[module htmlparser.DefaultHandler.prototype](#apidoc.module.htmlparser.DefaultHandler.prototype)

#### <a name="apidoc.element.htmlparser.DefaultHandler.prototype.done"></a>[function <span class="apidocSignatureSpan">htmlparser.DefaultHandler.prototype.</span>done ()](#apidoc.element.htmlparser.DefaultHandler.prototype.done)
- description and source-code
```javascript
function DefaultHandler$done() {
		this._done = true;
		this.handleCallback(null);
	}
```
- example usage
```shell
...
##Streaming To Parser

'''javascript
while (...) {
	...
	parser.parseChunk(chunk);
}
parser.done();	
'''

##Parsing RSS/Atom Feeds

'''javascript
new htmlparser.RssHandler(function (error, dom) {
	...
...
```

#### <a name="apidoc.element.htmlparser.DefaultHandler.prototype.error"></a>[function <span class="apidocSignatureSpan">htmlparser.DefaultHandler.prototype.</span>error (error)](#apidoc.element.htmlparser.DefaultHandler.prototype.error)
- description and source-code
```javascript
function DefaultHandler$error(error) {
		this.handleCallback(error);
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.htmlparser.DefaultHandler.prototype.handleCallback"></a>[function <span class="apidocSignatureSpan">htmlparser.DefaultHandler.prototype.</span>handleCallback (error)](#apidoc.element.htmlparser.DefaultHandler.prototype.handleCallback)
- description and source-code
```javascript
function DefaultHandler$handleCallback(error) {
			if ((typeof this._callback) != "function")
				if (error)
					throw error;
				else
					return;
			this._callback(error, this.dom);
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.htmlparser.DefaultHandler.prototype.handleElement"></a>[function <span class="apidocSignatureSpan">htmlparser.DefaultHandler.prototype.</span>handleElement (element)](#apidoc.element.htmlparser.DefaultHandler.prototype.handleElement)
- description and source-code
```javascript
function DefaultHandler$handleElement(element) {
		if (this._done)
			this.handleCallback(new Error("Writing to the handler after done() called is not allowed without a reset()"));
		if (!this._options.verbose) {
//			element.raw = null; //FIXME: Not clean
			//FIXME: Serious performance problem using delete
			delete element.raw;
			if (element.type == "tag" || element.type == "script" || element.type == "style")
				delete element.data;
		}
		if (!this._tagStack.last()) { //There are no parent elements
			//If the element can be a container, add it to the tag stack and the top level list
			if (element.type != ElementType.Text && element.type != ElementType.Comment && element.type != ElementType.Directive) {
				if (element.name.charAt(0) != "/") { //Ignore closing tags that obviously don't have an opening tag
					this.dom.push(element);
					if (!this.isEmptyTag(element)) { //Don't add tags to the tag stack that can't have children
						this._tagStack.push(element);
					}
				}
			}
			else //Otherwise just add to the top level list
				this.dom.push(element);
		}
		else { //There are parent elements
			//If the element can be a container, add it as a child of the element
			//on top of the tag stack and then add it to the tag stack
			if (element.type != ElementType.Text && element.type != ElementType.Comment && element.type != ElementType.Directive) {
				if (element.name.charAt(0) == "/") {
					//This is a closing tag, scan the tagStack to find the matching opening tag
					//and pop the stack up to the opening tag's parent
					var baseName = element.name.substring(1);
					if (!this.isEmptyTag(element)) {
						var pos = this._tagStack.length - 1;
						while (pos > -1 && this._tagStack[pos--].name != baseName) { }
						if (pos > -1 || this._tagStack[0].name == baseName)
							while (pos < this._tagStack.length - 1)
								this._tagStack.pop();
					}
				}
				else { //This is not a closing tag
					if (!this._tagStack.last().children)
						this._tagStack.last().children = [];
					this._tagStack.last().children.push(element);
					if (!this.isEmptyTag(element)) //Don't add tags to the tag stack that can't have children
						this._tagStack.push(element);
				}
			}
			else { //This is not a container element
				if (!this._tagStack.last().children)
					this._tagStack.last().children = [];
				this._tagStack.last().children.push(element);
			}
		}
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.htmlparser.DefaultHandler.prototype.isEmptyTag"></a>[function <span class="apidocSignatureSpan">htmlparser.DefaultHandler.prototype.</span>isEmptyTag (element)](#apidoc.element.htmlparser.DefaultHandler.prototype.isEmptyTag)
- description and source-code
```javascript
isEmptyTag = function (element) {
		var name = element.name.toLowerCase();
		if (name.charAt(0) == '/') {
			name = name.substring(1);
		}
		return this._options.enforceEmptyTags && !!DefaultHandler._emptyTags[name];
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.htmlparser.DefaultHandler.prototype.reset"></a>[function <span class="apidocSignatureSpan">htmlparser.DefaultHandler.prototype.</span>reset ()](#apidoc.element.htmlparser.DefaultHandler.prototype.reset)
- description and source-code
```javascript
function DefaultHandler$reset() {
		this.dom = [];
		this._done = false;
		this._tagStack = [];
		this._tagStack.last = function DefaultHandler$_tagStack$last () {
			return(this.length ? this[this.length - 1] : null);
		}
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.htmlparser.DefaultHandler.prototype.writeComment"></a>[function <span class="apidocSignatureSpan">htmlparser.DefaultHandler.prototype.</span>writeComment (element)](#apidoc.element.htmlparser.DefaultHandler.prototype.writeComment)
- description and source-code
```javascript
function DefaultHandler$writeComment(element) {
		this.handleElement(element);
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.htmlparser.DefaultHandler.prototype.writeDirective"></a>[function <span class="apidocSignatureSpan">htmlparser.DefaultHandler.prototype.</span>writeDirective (element)](#apidoc.element.htmlparser.DefaultHandler.prototype.writeDirective)
- description and source-code
```javascript
function DefaultHandler$writeDirective(element) {
		this.handleElement(element);
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.htmlparser.DefaultHandler.prototype.writeTag"></a>[function <span class="apidocSignatureSpan">htmlparser.DefaultHandler.prototype.</span>writeTag (element)](#apidoc.element.htmlparser.DefaultHandler.prototype.writeTag)
- description and source-code
```javascript
function DefaultHandler$writeTag(element) {
		this.handleElement(element);
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.htmlparser.DefaultHandler.prototype.writeText"></a>[function <span class="apidocSignatureSpan">htmlparser.DefaultHandler.prototype.</span>writeText (element)](#apidoc.element.htmlparser.DefaultHandler.prototype.writeText)
- description and source-code
```javascript
function DefaultHandler$writeText(element) {
		if (this._options.ignoreWhitespace)
			if (DefaultHandler.reWhitespace.test(element.data))
				return;
		this.handleElement(element);
	}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.htmlparser.DomUtils"></a>[module htmlparser.DomUtils](#apidoc.module.htmlparser.DomUtils)

#### <a name="apidoc.element.htmlparser.DomUtils.getElementById"></a>[function <span class="apidocSignatureSpan">htmlparser.DomUtils.</span>getElementById (id, currentElement, recurse)](#apidoc.element.htmlparser.DomUtils.getElementById)
- description and source-code
```javascript
function DomUtils$getElementById(id, currentElement, recurse) {
			var result = DomUtils.getElements({ id: id }, currentElement, recurse, 1);
			return(result.length ? result[0] : null);
		}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.htmlparser.DomUtils.getElements"></a>[function <span class="apidocSignatureSpan">htmlparser.DomUtils.</span>getElements (options, currentElement, recurse, limit)](#apidoc.element.htmlparser.DomUtils.getElements)
- description and source-code
```javascript
function DomUtils$getElements(options, currentElement, recurse, limit) {
			recurse = (recurse === undefined || recurse === null) || !!recurse;
			limit = isNaN(parseInt(limit)) ? -1 : parseInt(limit);

			if (!currentElement) {
				return([]);
			}
	
			var found = [];
			var elementList;

			function getTest (checkVal) {
				return(function (value) { return(value == checkVal); });
			}
			for (var key in options) {
				if ((typeof options[key]) != "function") {
					options[key] = getTest(options[key]);
				}
			}
	
			if (DomUtils.testElement(options, currentElement)) {
				found.push(currentElement);
			}

			if (limit >= 0 && found.length >= limit) {
				return(found);
			}

			if (recurse && currentElement.children) {
				elementList = currentElement.children;
			} else if (currentElement instanceof Array) {
				elementList = currentElement;
			} else {
				return(found);
			}
	
			for (var i = 0; i < elementList.length; i++) {
				found = found.concat(DomUtils.getElements(options, elementList[i], recurse, limit));
				if (limit >= 0 && found.length >= limit) {
					break;
				}
			}
	
			return(found);
		}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.htmlparser.DomUtils.getElementsByTagName"></a>[function <span class="apidocSignatureSpan">htmlparser.DomUtils.</span>getElementsByTagName (name, currentElement, recurse, limit)](#apidoc.element.htmlparser.DomUtils.getElementsByTagName)
- description and source-code
```javascript
function DomUtils$getElementsByTagName(name, currentElement, recurse, limit) {
			return(DomUtils.getElements({ tag_name: name }, currentElement, recurse, limit));
		}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.htmlparser.DomUtils.getElementsByTagType"></a>[function <span class="apidocSignatureSpan">htmlparser.DomUtils.</span>getElementsByTagType (type, currentElement, recurse, limit)](#apidoc.element.htmlparser.DomUtils.getElementsByTagType)
- description and source-code
```javascript
function DomUtils$getElementsByTagType(type, currentElement, recurse, limit) {
			return(DomUtils.getElements({ tag_type: type }, currentElement, recurse, limit));
		}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.htmlparser.DomUtils.testElement"></a>[function <span class="apidocSignatureSpan">htmlparser.DomUtils.</span>testElement (options, element)](#apidoc.element.htmlparser.DomUtils.testElement)
- description and source-code
```javascript
function DomUtils$testElement(options, element) {
			if (!element) {
				return false;
			}
	
			for (var key in options) {
				if (key == "tag_name") {
					if (element.type != "tag" && element.type != "script" && element.type != "style") {
						return false;
					}
					if (!options["tag_name"](element.name)) {
						return false;
					}
				} else if (key == "tag_type") {
					if (!options["tag_type"](element.type)) {
						return false;
					}
				} else if (key == "tag_contains") {
					if (element.type != "text" && element.type != "comment" && element.type != "directive") {
						return false;
					}
					if (!options["tag_contains"](element.data)) {
						return false;
					}
				} else {
					if (!element.attribs || !options[key](element.attribs[key])) {
						return false;
					}
				}
			}
		
			return true;
		}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.htmlparser.Parser"></a>[module htmlparser.Parser](#apidoc.module.htmlparser.Parser)

#### <a name="apidoc.element.htmlparser.Parser.Parser"></a>[function <span class="apidocSignatureSpan">htmlparser.</span>Parser (handler, options)](#apidoc.element.htmlparser.Parser.Parser)
- description and source-code
```javascript
function Parser(handler, options) {
	this._options = options ? options : { };
	if (this._options.includeLocation == undefined) {
		this._options.includeLocation = false; //Do not track element position in document by default
	}

	this.validateHandler(handler);
	this._handler = handler;
	this.reset();
}
```
- example usage
```shell
...
var rawHtml = "Xyz <script language= javascript>var foo = '<<bar>>';< /  script><!--<!-- Waah! -- -->";
var handler = new htmlparser.DefaultHandler(function (error, dom) {
	if (error)
		[...do something for errors...]
	else
		[...parsing done, do something...]
});
var parser = new htmlparser.Parser(handler);
parser.parseComplete(rawHtml);
sys.puts(sys.inspect(handler.dom, false, null));
'''

##Usage In Browser

'''javascript
...
```



# <a name="apidoc.module.htmlparser.Parser.prototype"></a>[module htmlparser.Parser.prototype](#apidoc.module.htmlparser.Parser.prototype)

#### <a name="apidoc.element.htmlparser.Parser.prototype.done"></a>[function <span class="apidocSignatureSpan">htmlparser.Parser.prototype.</span>done ()](#apidoc.element.htmlparser.Parser.prototype.done)
- description and source-code
```javascript
function Parser$done() {
		if (this._done)
			return;
		this._done = true;
	
		//Push any unparsed text into a final element in the element list
		if (this._buffer.length) {
			var rawData = this._buffer;
			this._buffer = "";
			var element = {
				  raw: rawData
				, data: (this._parseState == ElementType.Text) ? rawData : rawData.replace(Parser._reTrim, "")
				, type: this._parseState
				};
			if (this._parseState == ElementType.Tag || this._parseState == ElementType.Script || this._parseState == ElementType.Style)
				element.name = this.parseTagName(element.data);
			this.parseAttribs(element);
			this._elements.push(element);
		}
	
		this.writeHandler();
		this._handler.done();
	}
```
- example usage
```shell
...
##Streaming To Parser

'''javascript
while (...) {
	...
	parser.parseChunk(chunk);
}
parser.done();	
'''

##Parsing RSS/Atom Feeds

'''javascript
new htmlparser.RssHandler(function (error, dom) {
	...
...
```

#### <a name="apidoc.element.htmlparser.Parser.prototype.getLocation"></a>[function <span class="apidocSignatureSpan">htmlparser.Parser.prototype.</span>getLocation (startTag)](#apidoc.element.htmlparser.Parser.prototype.getLocation)
- description and source-code
```javascript
function Parser$getLocation(startTag) {
		var c,
			l = this._location,
			end = this._current - (startTag ? 1 : 0),
			chunk = startTag && l.charOffset == 0 && this._current == 0;
		
		for (; l.charOffset < end; l.charOffset++) {
			c = this._buffer.charAt(l.charOffset);
			if (c == '\n') {
				l.inBuffer++;
				l.col = 0;
			} else if (c != '\r') {
				l.col++;
			}
		}
		return {
			  line: l.row + l.inBuffer + 1
			, col: l.col + (chunk ? 0: 1)
		};
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.htmlparser.Parser.prototype.handleError"></a>[function <span class="apidocSignatureSpan">htmlparser.Parser.prototype.</span>handleError (error)](#apidoc.element.htmlparser.Parser.prototype.handleError)
- description and source-code
```javascript
function Parser$handleError(error) {
		if ((typeof this._handler.error) == "function")
			this._handler.error(error);
		else
			throw error;
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.htmlparser.Parser.prototype.parseAttribs"></a>[function <span class="apidocSignatureSpan">htmlparser.Parser.prototype.</span>parseAttribs (element)](#apidoc.element.htmlparser.Parser.prototype.parseAttribs)
- description and source-code
```javascript
function Parser$parseAttribs(element) {
		//Only parse attributes for tags
		if (element.type != ElementType.Script && element.type != ElementType.Style && element.type != ElementType.Tag)
			return;
	
		var tagName = element.data.split(Parser._reWhitespace, 1)[0];
		var attribRaw = element.data.substring(tagName.length);
		if (attribRaw.length < 1)
			return;
	
		var match;
		Parser._reAttrib.lastIndex = 0;
		while (match = Parser._reAttrib.exec(attribRaw)) {
			if (element.attribs == undefined)
				element.attribs = {};
	
			if (typeof match[1] == "string" && match[1].length) {
				element.attribs[match[1]] = match[2];
			} else if (typeof match[3] == "string" && match[3].length) {
				element.attribs[match[3].toString()] = match[4].toString();
			} else if (typeof match[5] == "string" && match[5].length) {
				element.attribs[match[5]] = match[6];
			} else if (typeof match[7] == "string" && match[7].length) {
				element.attribs[match[7]] = match[7];
			}
		}
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.htmlparser.Parser.prototype.parseChunk"></a>[function <span class="apidocSignatureSpan">htmlparser.Parser.prototype.</span>parseChunk (data)](#apidoc.element.htmlparser.Parser.prototype.parseChunk)
- description and source-code
```javascript
function Parser$parseChunk(data) {
		if (this._done)
			this.handleError(new Error("Attempted to parse chunk after parsing already done"));
		this._buffer += data; //FIXME: this can be a bottleneck
		this.parseTags();
	}
```
- example usage
```shell
...
'''

##Streaming To Parser

'''javascript
while (...) {
	...
	parser.parseChunk(chunk);
}
parser.done();	
'''

##Parsing RSS/Atom Feeds

'''javascript
...
```

#### <a name="apidoc.element.htmlparser.Parser.prototype.parseComplete"></a>[function <span class="apidocSignatureSpan">htmlparser.Parser.prototype.</span>parseComplete (data)](#apidoc.element.htmlparser.Parser.prototype.parseComplete)
- description and source-code
```javascript
function Parser$parseComplete(data) {
		this.reset();
		this.parseChunk(data);
		this.done();
	}
```
- example usage
```shell
...
var handler = new htmlparser.DefaultHandler(function (error, dom) {
	if (error)
		[...do something for errors...]
	else
		[...parsing done, do something...]
});
var parser = new htmlparser.Parser(handler);
parser.parseComplete(rawHtml);
sys.puts(sys.inspect(handler.dom, false, null));
'''

##Usage In Browser

'''javascript
var handler = new Tautologistics.NodeHtmlParser.DefaultHandler(function (error, dom) {
...
```

#### <a name="apidoc.element.htmlparser.Parser.prototype.parseTagAttribs"></a>[function <span class="apidocSignatureSpan">htmlparser.Parser.prototype.</span>parseTagAttribs (elements)](#apidoc.element.htmlparser.Parser.prototype.parseTagAttribs)
- description and source-code
```javascript
function Parser$parseTagAttribs(elements) {
		var idxEnd = elements.length;
		var idx = 0;
	
		while (idx < idxEnd) {
			var element = elements[idx++];
			if (element.type == ElementType.Tag || element.type == ElementType.Script || element.type == ElementType.style)
				this.parseAttribs(element);
		}
	
		return(elements);
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.htmlparser.Parser.prototype.parseTagName"></a>[function <span class="apidocSignatureSpan">htmlparser.Parser.prototype.</span>parseTagName (data)](#apidoc.element.htmlparser.Parser.prototype.parseTagName)
- description and source-code
```javascript
function Parser$parseTagName(data) {
		if (data == null || data == "")
			return("");
		var match = Parser._reTagName.exec(data);
		if (!match)
			return("");
		return((match[1] ? "/" : "") + match[2]);
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.htmlparser.Parser.prototype.parseTags"></a>[function <span class="apidocSignatureSpan">htmlparser.Parser.prototype.</span>parseTags ()](#apidoc.element.htmlparser.Parser.prototype.parseTags)
- description and source-code
```javascript
function Parser$parseTags() {
		var bufferEnd = this._buffer.length - 1;
		while (Parser._reTags.test(this._buffer)) {
			this._next = Parser._reTags.lastIndex - 1;
			var tagSep = this._buffer.charAt(this._next); //The currently found tag marker
			var rawData = this._buffer.substring(this._current, this._next); //The next chunk of data to parse
	
			//A new element to eventually be appended to the element list
			var element = {
				  raw: rawData
				, data: (this._parseState == ElementType.Text) ? rawData : rawData.replace(Parser._reTrim, "")
				, type: this._parseState
			};
	
			var elementName = this.parseTagName(element.data);
	
			//This section inspects the current tag stack and modifies the current
			//element if we're actually parsing a special area (script/comment/style tag)
			if (this._tagStack.length) { //We're parsing inside a script/comment/style tag
				if (this._tagStack[this._tagStack.length - 1] == ElementType.Script) { //We're currently in a script tag
					if (elementName.toLowerCase() == "/script") //Actually, we're no longer in a script tag, so pop it off the stack
						this._tagStack.pop();
					else { //Not a closing script tag
						if (element.raw.indexOf("!--") != 0) { //Make sure we're not in a comment
							//All data from here to script close is now a text element
							element.type = ElementType.Text;
							//If the previous element is text, append the current text to it
							if (this._elements.length && this._elements[this._elements.length - 1].type == ElementType.Text) {
								var prevElement = this._elements[this._elements.length - 1];
								prevElement.raw = prevElement.data = prevElement.raw + this._prevTagSep + element.raw;
								element.raw = element.data = ""; //This causes the current element to not be added to the element list
							}
						}
					}
				}
				else if (this._tagStack[this._tagStack.length - 1] == ElementType.Style) { //We're currently in a style tag
					if (elementName.toLowerCase() == "/style") //Actually, we're no longer in a style tag, so pop it off the stack
						this._tagStack.pop();
					else {
						if (element.raw.indexOf("!--") != 0) { //Make sure we're not in a comment
							//All data from here to style close is now a text element
							element.type = ElementType.Text;
							//If the previous element is text, append the current text to it
							if (this._elements.length && this._elements[this._elements.length - 1].type == ElementType.Text) {
								var prevElement = this._elements[this._elements.length - 1];
								if (element.raw != "") {
									prevElement.raw = prevElement.data = prevElement.raw + this._prevTagSep + element.raw;
									element.raw = element.data = ""; //This causes the current element to not be added to the element list
								} else { //Element is empty, so just append the last tag marker found
									prevElement.raw = prevElement.data = prevElement.raw + this._prevTagSep;
								}
							} else { //The previous element was not text
								if (element.raw != "") {
									element.raw = element.data = element.raw;
								}
							}
						}
					}
				}
				else if (this._tagStack[this._tagStack.length - 1] == ElementType.Comment) { //We're currently in a comment tag
					var rawLen = element.raw.length;
					if (element.raw.charAt(rawLen - 2) == "-" && element.raw.charAt(rawLen - 1) == "-" && tagSep == ">") {
						//Actually, we're no longer in a style tag, so pop it off the stack
						this._tagStack.pop();
						//If the previous element is a comment, append the current text to it
						if (this._elements.length && this._elements[this._elements.length - 1].type == ElementType.Comment) {
							var prevElement = this._elements[this._elements.length - 1];
							prevElement.raw = prevElement.data = (prevElement.raw + element.raw).replace(Parser._reTrimComment, "");
							element.raw = element.data = ""; //This causes the current element to not be added to the element list
							element.type = ElementType.Text;
						}
						else //Previous element not a comment
							element.type = ElementType ...
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.htmlparser.Parser.prototype.reset"></a>[function <span class="apidocSignatureSpan">htmlparser.Parser.prototype.</span>reset ()](#apidoc.element.htmlparser.Parser.prototype.reset)
- description and source-code
```javascript
function Parser$reset() {
		this._buffer = "";
		this._done = false;
		this._elements = [];
		this._elementsCurrent = 0;
		this._current = 0;
		this._next = 0;
		this._location = {
			  row: 0
			, col: 0
			, charOffset: 0
			, inBuffer: 0
		};
		this._parseState = ElementType.Text;
		this._prevTagSep = '';
		this._tagStack = [];
		this._handler.reset();
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.htmlparser.Parser.prototype.validateHandler"></a>[function <span class="apidocSignatureSpan">htmlparser.Parser.prototype.</span>validateHandler (handler)](#apidoc.element.htmlparser.Parser.prototype.validateHandler)
- description and source-code
```javascript
function Parser$validateHandler(handler) {
		if ((typeof handler) != "object")
			throw new Error("Handler is not an object");
		if ((typeof handler.reset) != "function")
			throw new Error("Handler method 'reset' is invalid");
		if ((typeof handler.done) != "function")
			throw new Error("Handler method 'done' is invalid");
		if ((typeof handler.writeTag) != "function")
			throw new Error("Handler method 'writeTag' is invalid");
		if ((typeof handler.writeText) != "function")
			throw new Error("Handler method 'writeText' is invalid");
		if ((typeof handler.writeComment) != "function")
			throw new Error("Handler method 'writeComment' is invalid");
		if ((typeof handler.writeDirective) != "function")
			throw new Error("Handler method 'writeDirective' is invalid");
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.htmlparser.Parser.prototype.writeHandler"></a>[function <span class="apidocSignatureSpan">htmlparser.Parser.prototype.</span>writeHandler (forceFlush)](#apidoc.element.htmlparser.Parser.prototype.writeHandler)
- description and source-code
```javascript
function Parser$writeHandler(forceFlush) {
		forceFlush = !!forceFlush;
		if (this._tagStack.length && !forceFlush)
			return;
		while (this._elements.length) {
			var element = this._elements.shift();
			switch (element.type) {
				case ElementType.Comment:
					this._handler.writeComment(element);
					break;
				case ElementType.Directive:
					this._handler.writeDirective(element);
					break;
				case ElementType.Text:
					this._handler.writeText(element);
					break;
				default:
					this._handler.writeTag(element);
					break;
			}
		}
	}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.htmlparser.RssHandler"></a>[module htmlparser.RssHandler](#apidoc.module.htmlparser.RssHandler)

#### <a name="apidoc.element.htmlparser.RssHandler.RssHandler"></a>[function <span class="apidocSignatureSpan">htmlparser.</span>RssHandler (callback)](#apidoc.element.htmlparser.RssHandler.RssHandler)
- description and source-code
```javascript
function RssHandler(callback) {
	RssHandler.super_.call(this, callback, { ignoreWhitespace: true, verbose: false, enforceEmptyTags: false });
}
```
- example usage
```shell
...
}
parser.done();	
'''

##Parsing RSS/Atom Feeds

'''javascript
new htmlparser.RssHandler(function (error, dom) {
	...
});
'''

##DefaultHandler Options

###Usage
...
```

#### <a name="apidoc.element.htmlparser.RssHandler.super_"></a>[function <span class="apidocSignatureSpan">htmlparser.RssHandler.</span>super_ (callback, options)](#apidoc.element.htmlparser.RssHandler.super_)
- description and source-code
```javascript
function DefaultHandler(callback, options) {
	this.reset();
	this._options = options ? options : { };
	if (this._options.ignoreWhitespace == undefined)
		this._options.ignoreWhitespace = false; //Keep whitespace-only text nodes
	if (this._options.verbose == undefined)
		this._options.verbose = true; //Keep data property for tags and raw property for all
	if (this._options.enforceEmptyTags == undefined)
		this._options.enforceEmptyTags = true; //Don't allow children for HTML tags defined as empty in spec
	if ((typeof callback) == "function")
		this._callback = callback;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.htmlparser.RssHandler.prototype"></a>[module htmlparser.RssHandler.prototype](#apidoc.module.htmlparser.RssHandler.prototype)

#### <a name="apidoc.element.htmlparser.RssHandler.prototype.constructor"></a>[function <span class="apidocSignatureSpan">htmlparser.RssHandler.prototype.</span>constructor (callback)](#apidoc.element.htmlparser.RssHandler.prototype.constructor)
- description and source-code
```javascript
function RssHandler(callback) {
	RssHandler.super_.call(this, callback, { ignoreWhitespace: true, verbose: false, enforceEmptyTags: false });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.htmlparser.RssHandler.prototype.done"></a>[function <span class="apidocSignatureSpan">htmlparser.RssHandler.prototype.</span>done ()](#apidoc.element.htmlparser.RssHandler.prototype.done)
- description and source-code
```javascript
function RssHandler$done() {
		var feed = { };
		var feedRoot;

		var found = DomUtils.getElementsByTagName(function (value) { return(value == "rss" || value == "feed"); }, this.dom, false);
		if (found.length) {
			feedRoot = found[0];
		}
		if (feedRoot) {
			if (feedRoot.name == "rss") {
				feed.type = "rss";
				feedRoot = feedRoot.children[0]; //<channel/>
				feed.id = "";
				try {
					feed.title = DomUtils.getElementsByTagName("title", feedRoot.children, false)[0].children[0].data;
				} catch (ex) { }
				try {
					feed.link = DomUtils.getElementsByTagName("link", feedRoot.children, false)[0].children[0].data;
				} catch (ex) { }
				try {
					feed.description = DomUtils.getElementsByTagName("description", feedRoot.children, false)[0].children[0].data;
				} catch (ex) { }
				try {
					feed.updated = new Date(DomUtils.getElementsByTagName("lastBuildDate", feedRoot.children, false)[0].children[0].data);
				} catch (ex) { }
				try {
					feed.author = DomUtils.getElementsByTagName("managingEditor", feedRoot.children, false)[0].children[0].data;
				} catch (ex) { }
				feed.items = [];
				DomUtils.getElementsByTagName("item", feedRoot.children).forEach(function (item, index, list) {
					var entry = {};
					try {
						entry.id = DomUtils.getElementsByTagName("guid", item.children, false)[0].children[0].data;
					} catch (ex) { }
					try {
						entry.title = DomUtils.getElementsByTagName("title", item.children, false)[0].children[0].data;
					} catch (ex) { }
					try {
						entry.link = DomUtils.getElementsByTagName("link", item.children, false)[0].children[0].data;
					} catch (ex) { }
					try {
						entry.description = DomUtils.getElementsByTagName("description", item.children, false)[0].children[0].data;
					} catch (ex) { }
					try {
						entry.pubDate = new Date(DomUtils.getElementsByTagName("pubDate", item.children, false)[0].children[0].data);
					} catch (ex) { }
					feed.items.push(entry);
				});
			} else {
				feed.type = "atom";
				try {
					feed.id = DomUtils.getElementsByTagName("id", feedRoot.children, false)[0].children[0].data;
				} catch (ex) { }
				try {
					feed.title = DomUtils.getElementsByTagName("title", feedRoot.children, false)[0].children[0].data;
				} catch (ex) { }
				try {
					feed.link = DomUtils.getElementsByTagName("link", feedRoot.children, false)[0].attribs.href;
				} catch (ex) { }
				try {
					feed.description = DomUtils.getElementsByTagName("subtitle", feedRoot.children, false)[0].children[0].data;
				} catch (ex) { }
				try {
					feed.updated = new Date(DomUtils.getElementsByTagName("updated", feedRoot.children, false)[0].children[0].data);
				} catch (ex) { }
				try {
					feed.author = DomUtils.getElementsByTagName("email", feedRoot.children, true)[0].children[0].data;
				} catch (ex) { }
				feed.items = [];
				DomUtils.getElementsByTagName("entry", feedRoot.children).forEach(function (item, index, list) {
					var entry = {};
					try {
						entry.id = DomUtils.getElementsByTagName("id", item.children, false)[0].children[0].data;
					} catch (ex) { }
					try {
						entry.title = DomUtils.getElementsByTagName("title", item.children, false)[0].children[0].data;
					} catch (ex) { }
					try {
						entry.link = DomUtils.getElementsByTagName("link", item.children, false)[0].attribs.href;
					} catch (ex) { }
					try {
						entry.description = DomUtils.getElementsByTagName("summary", item.children, false)[0].children[0].data;
					} catch (ex) { }
					try {
						entry.pubDate = new Date(DomUtils.getElementsByTagName("updated", item.children, false)[0].children[0].data);
					} catch (ex) { }
					feed.items.push(entry);
				});
			}

			this.dom = feed;
		}
		RssHandler.super_.prototype.done.call(this);
	}
```
- example usage
```shell
...
##Streaming To Parser

'''javascript
while (...) {
	...
	parser.parseChunk(chunk);
}
parser.done();	
'''

##Parsing RSS/Atom Feeds

'''javascript
new htmlparser.RssHandler(function (error, dom) {
	...
...
```



# <a name="apidoc.module.htmlparser.node_htmlparser"></a>[module htmlparser.node_htmlparser](#apidoc.module.htmlparser.node_htmlparser)

#### <a name="apidoc.element.htmlparser.node_htmlparser.DefaultHandler"></a>[function <span class="apidocSignatureSpan">htmlparser.node_htmlparser.</span>DefaultHandler (callback, options)](#apidoc.element.htmlparser.node_htmlparser.DefaultHandler)
- description and source-code
```javascript
function DefaultHandler(callback, options) {
	this.reset();
	this._options = options ? options : { };
	if (this._options.ignoreWhitespace == undefined)
		this._options.ignoreWhitespace = false; //Keep whitespace-only text nodes
	if (this._options.verbose == undefined)
		this._options.verbose = true; //Keep data property for tags and raw property for all
	if (this._options.enforceEmptyTags == undefined)
		this._options.enforceEmptyTags = true; //Don't allow children for HTML tags defined as empty in spec
	if ((typeof callback) == "function")
		this._callback = callback;
}
```
- example usage
```shell
...
View runtests.html in any browser

##Usage In Node

'''javascript
var htmlparser = require("htmlparser");
var rawHtml = "Xyz <script language= javascript>var foo = '<<bar>>';< /  script><!--<!-- Waah! -- -->";
var handler = new htmlparser.DefaultHandler(function (error, dom) {
	if (error)
		[...do something for errors...]
	else
		[...parsing done, do something...]
});
var parser = new htmlparser.Parser(handler);
parser.parseComplete(rawHtml);
...
```

#### <a name="apidoc.element.htmlparser.node_htmlparser.Parser"></a>[function <span class="apidocSignatureSpan">htmlparser.node_htmlparser.</span>Parser (handler, options)](#apidoc.element.htmlparser.node_htmlparser.Parser)
- description and source-code
```javascript
function Parser(handler, options) {
	this._options = options ? options : { };
	if (this._options.includeLocation == undefined) {
		this._options.includeLocation = false; //Do not track element position in document by default
	}

	this.validateHandler(handler);
	this._handler = handler;
	this.reset();
}
```
- example usage
```shell
...
var rawHtml = "Xyz <script language= javascript>var foo = '<<bar>>';< /  script><!--<!-- Waah! -- -->";
var handler = new htmlparser.DefaultHandler(function (error, dom) {
	if (error)
		[...do something for errors...]
	else
		[...parsing done, do something...]
});
var parser = new htmlparser.Parser(handler);
parser.parseComplete(rawHtml);
sys.puts(sys.inspect(handler.dom, false, null));
'''

##Usage In Browser

'''javascript
...
```

#### <a name="apidoc.element.htmlparser.node_htmlparser.RssHandler"></a>[function <span class="apidocSignatureSpan">htmlparser.node_htmlparser.</span>RssHandler (callback)](#apidoc.element.htmlparser.node_htmlparser.RssHandler)
- description and source-code
```javascript
function RssHandler(callback) {
	RssHandler.super_.call(this, callback, { ignoreWhitespace: true, verbose: false, enforceEmptyTags: false });
}
```
- example usage
```shell
...
}
parser.done();	
'''

##Parsing RSS/Atom Feeds

'''javascript
new htmlparser.RssHandler(function (error, dom) {
	...
});
'''

##DefaultHandler Options

###Usage
...
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
