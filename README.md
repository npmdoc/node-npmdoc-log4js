# api documentation for  [log4js (v1.1.1)](https://github.com/nomiddlename/log4js-node#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-log4js.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-log4js) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-log4js.svg)](https://travis-ci.org/npmdoc/node-npmdoc-log4js)
#### Port of Log4js to work with node.

[![NPM](https://nodei.co/npm/log4js.png?downloads=true)](https://www.npmjs.com/package/log4js)

[![apidoc](https://npmdoc.github.io/node-npmdoc-log4js/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-log4js_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-log4js/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-log4js/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-log4js/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Gareth Jones",
        "email": "gareth.nomiddlename@gmail.com"
    },
    "browser": {
        "os": false
    },
    "bugs": {
        "url": "http://github.com/nomiddlename/log4js-node/issues"
    },
    "dependencies": {
        "debug": "^2.2.0",
        "semver": "^5.3.0",
        "streamroller": "^0.4.0"
    },
    "description": "Port of Log4js to work with node.",
    "devDependencies": {
        "jshint": "^2.9.2",
        "sandboxed-module": "0.1.3",
        "tape": "^4.6.2",
        "vows": "0.7.0"
    },
    "directories": {
        "test": "test",
        "lib": "lib"
    },
    "dist": {
        "shasum": "c21d29c7604089e4f255833e7f94b3461de1ff43",
        "tarball": "https://registry.npmjs.org/log4js/-/log4js-1.1.1.tgz"
    },
    "engines": {
        "node": ">=0.12"
    },
    "gitHead": "1fb4f2f8723e6837dc3269970841184684238f74",
    "homepage": "https://github.com/nomiddlename/log4js-node#readme",
    "keywords": [
        "logging",
        "log",
        "log4j",
        "node"
    ],
    "license": "Apache-2.0",
    "main": "./lib/log4js",
    "maintainers": [
        {
            "name": "csausdev",
            "email": "gareth.jones@sensis.com.au"
        }
    ],
    "name": "log4js",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+https://github.com/nomiddlename/log4js-node.git"
    },
    "scripts": {
        "pretest": "jshint lib/ test/",
        "test": "tape 'test/tape/**/*.js' && vows test/vows/*.js"
    },
    "version": "1.1.1"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module log4js](#apidoc.module.log4js)
1.  [function <span class="apidocSignatureSpan">log4js.</span>addAppender ()](#apidoc.element.log4js.addAppender)
1.  [function <span class="apidocSignatureSpan">log4js.</span>clearAppenders ()](#apidoc.element.log4js.clearAppenders)
1.  [function <span class="apidocSignatureSpan">log4js.</span>configure (configurationFileOrObject, options)](#apidoc.element.log4js.configure)
1.  [function <span class="apidocSignatureSpan">log4js.</span>connectLogger (logger4js, options)](#apidoc.element.log4js.connectLogger)
1.  [function <span class="apidocSignatureSpan">log4js.</span>getBufferedLogger (categoryName)](#apidoc.element.log4js.getBufferedLogger)
1.  [function <span class="apidocSignatureSpan">log4js.</span>getDefaultLogger ()](#apidoc.element.log4js.getDefaultLogger)
1.  [function <span class="apidocSignatureSpan">log4js.</span>getLogger (loggerCategoryName)](#apidoc.element.log4js.getLogger)
1.  [function <span class="apidocSignatureSpan">log4js.</span>hasLogger (logger)](#apidoc.element.log4js.hasLogger)
1.  [function <span class="apidocSignatureSpan">log4js.</span>levels.Level (level, levelStr)](#apidoc.element.log4js.levels.Level)
1.  [function <span class="apidocSignatureSpan">log4js.</span>loadAppender (appender, appenderModule)](#apidoc.element.log4js.loadAppender)
1.  [function <span class="apidocSignatureSpan">log4js.</span>replaceConsole (logger)](#apidoc.element.log4js.replaceConsole)
1.  [function <span class="apidocSignatureSpan">log4js.</span>restoreConsole ()](#apidoc.element.log4js.restoreConsole)
1.  [function <span class="apidocSignatureSpan">log4js.</span>setGlobalLogLevel (level)](#apidoc.element.log4js.setGlobalLogLevel)
1.  [function <span class="apidocSignatureSpan">log4js.</span>shutdown (cb)](#apidoc.element.log4js.shutdown)
1.  object <span class="apidocSignatureSpan">log4js.</span>appenderMakers
1.  object <span class="apidocSignatureSpan">log4js.</span>appenders
1.  object <span class="apidocSignatureSpan">log4js.</span>connect_logger
1.  object <span class="apidocSignatureSpan">log4js.</span>date_format
1.  object <span class="apidocSignatureSpan">log4js.</span>layouts
1.  object <span class="apidocSignatureSpan">log4js.</span>levels
1.  object <span class="apidocSignatureSpan">log4js.</span>levels.Level.prototype
1.  object <span class="apidocSignatureSpan">log4js.</span>logger

#### [module log4js.appenderMakers](#apidoc.module.log4js.appenderMakers)
1.  [function <span class="apidocSignatureSpan">log4js.appenderMakers.</span>stdout ()](#apidoc.element.log4js.appenderMakers.stdout)

#### [module log4js.appenders](#apidoc.module.log4js.appenders)
1.  [function <span class="apidocSignatureSpan">log4js.appenders.</span>stdout ()](#apidoc.element.log4js.appenders.stdout)

#### [module log4js.connect_logger](#apidoc.module.log4js.connect_logger)
1.  [function <span class="apidocSignatureSpan">log4js.connect_logger.</span>connectLogger (logger4js, options)](#apidoc.element.log4js.connect_logger.connectLogger)

#### [module log4js.date_format](#apidoc.module.log4js.date_format)
1.  [function <span class="apidocSignatureSpan">log4js.date_format.</span>asString (date, timezoneOffset)](#apidoc.element.log4js.date_format.asString)
1.  string <span class="apidocSignatureSpan">log4js.date_format.</span>ABSOLUTETIME_FORMAT
1.  string <span class="apidocSignatureSpan">log4js.date_format.</span>DATETIME_FORMAT
1.  string <span class="apidocSignatureSpan">log4js.date_format.</span>ISO8601_FORMAT
1.  string <span class="apidocSignatureSpan">log4js.date_format.</span>ISO8601_WITH_TZ_OFFSET_FORMAT

#### [module log4js.layouts](#apidoc.module.log4js.layouts)
1.  [function <span class="apidocSignatureSpan">log4js.layouts.</span>addLayout (name, serializerGenerator)](#apidoc.element.log4js.layouts.addLayout)
1.  [function <span class="apidocSignatureSpan">log4js.layouts.</span>basicLayout (loggingEvent, timezoneOffset)](#apidoc.element.log4js.layouts.basicLayout)
1.  [function <span class="apidocSignatureSpan">log4js.layouts.</span>coloredLayout (loggingEvent, timezoneOffset)](#apidoc.element.log4js.layouts.coloredLayout)
1.  [function <span class="apidocSignatureSpan">log4js.layouts.</span>colouredLayout (loggingEvent, timezoneOffset)](#apidoc.element.log4js.layouts.colouredLayout)
1.  [function <span class="apidocSignatureSpan">log4js.layouts.</span>dummyLayout (loggingEvent)](#apidoc.element.log4js.layouts.dummyLayout)
1.  [function <span class="apidocSignatureSpan">log4js.layouts.</span>layout (name, config)](#apidoc.element.log4js.layouts.layout)
1.  [function <span class="apidocSignatureSpan">log4js.layouts.</span>messagePassThroughLayout (loggingEvent)](#apidoc.element.log4js.layouts.messagePassThroughLayout)
1.  [function <span class="apidocSignatureSpan">log4js.layouts.</span>patternLayout (pattern, tokens, timezoneOffset)](#apidoc.element.log4js.layouts.patternLayout)

#### [module log4js.levels](#apidoc.module.log4js.levels)
1.  [function <span class="apidocSignatureSpan">log4js.levels.</span>Level (level, levelStr)](#apidoc.element.log4js.levels.Level)
1.  [function <span class="apidocSignatureSpan">log4js.levels.</span>forName (levelStr, levelVal)](#apidoc.element.log4js.levels.forName)
1.  [function <span class="apidocSignatureSpan">log4js.levels.</span>getLevel (levelStr)](#apidoc.element.log4js.levels.getLevel)
1.  [function <span class="apidocSignatureSpan">log4js.levels.</span>toLevel (sArg, defaultLevel)](#apidoc.element.log4js.levels.toLevel)
1.  object <span class="apidocSignatureSpan">log4js.levels.</span>ALL
1.  object <span class="apidocSignatureSpan">log4js.levels.</span>DEBUG
1.  object <span class="apidocSignatureSpan">log4js.levels.</span>ERROR
1.  object <span class="apidocSignatureSpan">log4js.levels.</span>FATAL
1.  object <span class="apidocSignatureSpan">log4js.levels.</span>INFO
1.  object <span class="apidocSignatureSpan">log4js.levels.</span>MARK
1.  object <span class="apidocSignatureSpan">log4js.levels.</span>OFF
1.  object <span class="apidocSignatureSpan">log4js.levels.</span>TRACE
1.  object <span class="apidocSignatureSpan">log4js.levels.</span>WARN

#### [module log4js.levels.Level](#apidoc.module.log4js.levels.Level)
1.  [function <span class="apidocSignatureSpan">log4js.levels.</span>Level (level, levelStr)](#apidoc.element.log4js.levels.Level.Level)

#### [module log4js.levels.Level.prototype](#apidoc.module.log4js.levels.Level.prototype)
1.  [function <span class="apidocSignatureSpan">log4js.levels.Level.prototype.</span>isEqualTo (otherLevel)](#apidoc.element.log4js.levels.Level.prototype.isEqualTo)
1.  [function <span class="apidocSignatureSpan">log4js.levels.Level.prototype.</span>isGreaterThanOrEqualTo (otherLevel)](#apidoc.element.log4js.levels.Level.prototype.isGreaterThanOrEqualTo)
1.  [function <span class="apidocSignatureSpan">log4js.levels.Level.prototype.</span>isLessThanOrEqualTo (otherLevel)](#apidoc.element.log4js.levels.Level.prototype.isLessThanOrEqualTo)
1.  [function <span class="apidocSignatureSpan">log4js.levels.Level.prototype.</span>toString ()](#apidoc.element.log4js.levels.Level.prototype.toString)

#### [module log4js.logger](#apidoc.module.log4js.logger)
1.  [function <span class="apidocSignatureSpan">log4js.logger.</span>Logger (name, level)](#apidoc.element.log4js.logger.Logger)
1.  [function <span class="apidocSignatureSpan">log4js.logger.</span>LoggingEvent (categoryName, level, data, logger)](#apidoc.element.log4js.logger.LoggingEvent)
1.  [function <span class="apidocSignatureSpan">log4js.logger.</span>addLevelMethods (level)](#apidoc.element.log4js.logger.addLevelMethods)
1.  [function <span class="apidocSignatureSpan">log4js.logger.</span>disableAllLogWrites ()](#apidoc.element.log4js.logger.disableAllLogWrites)
1.  [function <span class="apidocSignatureSpan">log4js.logger.</span>enableAllLogWrites ()](#apidoc.element.log4js.logger.enableAllLogWrites)



# <a name="apidoc.module.log4js"></a>[module log4js](#apidoc.module.log4js)

#### <a name="apidoc.element.log4js.addAppender"></a>[function <span class="apidocSignatureSpan">log4js.</span>addAppender ()](#apidoc.element.log4js.addAppender)
- description and source-code
```javascript
function addAppender() {
  var args = Array.prototype.slice.call(arguments);
  var appender = args.shift();
  //check for a shutdown fn
  if (args.length > 0 && typeof args[0] === 'function') {
    appenderShutdowns[appender] = args.shift();
  }

  if (args.length === 0 || args[0] === undefined) {
    args = [ ALL_CATEGORIES ];
  }
  //argument may already be an array
  if (Array.isArray(args[0])) {
    args = args[0];
  }

  args.forEach(function(appenderCategory) {
    addAppenderToCategory(appender, appenderCategory);

    if (appenderCategory === ALL_CATEGORIES) {
      addAppenderToAllLoggers(appender);
    } else {

      for(var loggerCategory in loggers) {
        if (doesAppenderContainsLogger(appenderCategory,loggerCategory)) {
          loggers[loggerCategory].addListener("log", appender);
        }
      }

    }
  });
}
```
- example usage
```shell
...
'''
See example.js for a full example, but here's a snippet (also in fromreadme.js):
'''javascript
var log4js = require('log4js');
//console log is loaded by default, so you won't normally need to do this
//log4js.loadAppender('console');
log4js.loadAppender('file');
//log4js.addAppender(log4js.appenders.console());
log4js.addAppender(log4js.appenders.file('logs/cheese.log'), 'cheese');

var logger = log4js.getLogger('cheese');
logger.setLevel('ERROR');

logger.trace('Entering cheese testing');
logger.debug('Got cheese.');
...
```

#### <a name="apidoc.element.log4js.clearAppenders"></a>[function <span class="apidocSignatureSpan">log4js.</span>clearAppenders ()](#apidoc.element.log4js.clearAppenders)
- description and source-code
```javascript
function clearAppenders() {
  //if we're calling clearAppenders, we're probably getting ready to write
  //so turn log writes back on, just in case this is after a shutdown
  loggerModule.enableAllLogWrites();
  appenders = {};
  for (var logger in loggers) {
    if (hasLogger(logger)) {
      loggers[logger].removeAllListeners("log");
    }
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.log4js.configure"></a>[function <span class="apidocSignatureSpan">log4js.</span>configure (configurationFileOrObject, options)](#apidoc.element.log4js.configure)
- description and source-code
```javascript
function configure(configurationFileOrObject, options) {
  var config = configurationFileOrObject;
  config = config || process.env.LOG4JS_CONFIG;
  options = options || {};

  if (config === undefined || config === null || typeof(config) === 'string') {
    if (options.reloadSecs) {
      initReloadConfiguration(config, options);
    }
    config = loadConfigurationFile(config) || defaultConfig;
  } else {
    if (options.reloadSecs) {
      getLogger('log4js').warn(
        'Ignoring configuration reload parameter for "object" configuration.'
      );
    }
  }
  configureOnceOff(config, options);
}
```
- example usage
```shell
...
'''bash
[2010-01-17 11:43:37.987] [ERROR] cheese - Cheese is too ripe!
[2010-01-17 11:43:37.990] [FATAL] cheese - Cheese was breeding ground for listeria.
'''
The first 5 lines of the code above could also be written as:
'''javascript
var log4js = require('log4js');
log4js.configure({
  appenders: [
    { type: 'console' },
    { type: 'file', filename: 'logs/cheese.log', category: 'cheese' }
  ]
});
'''
...
```

#### <a name="apidoc.element.log4js.connectLogger"></a>[function <span class="apidocSignatureSpan">log4js.</span>connectLogger (logger4js, options)](#apidoc.element.log4js.connectLogger)
- description and source-code
```javascript
function getLogger(logger4js, options) {
	if ('object' == typeof options) {
		options = options || {};
	} else if (options) {
		options = { format: options };
	} else {
		options = {};
	}

	var thislogger = logger4js
  , level = levels.toLevel(options.level, levels.INFO)
  , fmt = options.format || DEFAULT_FORMAT
  , nolog = options.nolog ? createNoLogCondition(options.nolog) : null;

  return function (req, res, next) {
    // mount safety
    if (req._logging) return next();

		// nologs
		if (nolog && nolog.test(req.originalUrl)) return next();
		if (thislogger.isLevelEnabled(level) || options.level === 'auto') {

			var start = new Date()
			, statusCode
			, writeHead = res.writeHead
			, url = req.originalUrl;

			// flag as logging
			req._logging = true;

			// proxy for statusCode.
			res.writeHead = function(code, headers){
				res.writeHead = writeHead;
				res.writeHead(code, headers);
				res.__statusCode = statusCode = code;
				res.__headers = headers || {};

				//status code response level handling
				if(options.level === 'auto'){
					level = levels.INFO;
					if(code >= 300) level = levels.WARN;
					if(code >= 400) level = levels.ERROR;
				} else {
					level = levels.toLevel(options.level, levels.INFO);
				}
			};

			//hook on end request to emit the log entry of the HTTP request.
			res.on('finish', function() {
				res.responseTime = new Date() - start;
				//status code response level handling
				if(res.statusCode && options.level === 'auto'){
					level = levels.INFO;
					if(res.statusCode >= 300) level = levels.WARN;
					if(res.statusCode >= 400) level = levels.ERROR;
				}
				if (thislogger.isLevelEnabled(level)) {
          var combined_tokens = assemble_tokens(req, res, options.tokens || []);
					if (typeof fmt === 'function') {
						var line = fmt(req, res, function(str){ return format(str, combined_tokens); });
						if (line) thislogger.log(level, line);
					} else {
						thislogger.log(level, format(fmt, combined_tokens));
					}
				}
			});
		}

    //ensure next gets always called
    next();
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.log4js.getBufferedLogger"></a>[function <span class="apidocSignatureSpan">log4js.</span>getBufferedLogger (categoryName)](#apidoc.element.log4js.getBufferedLogger)
- description and source-code
```javascript
function getBufferedLogger(categoryName) {
    var base_logger = getLogger(categoryName);
    var logger = {};
    logger.temp = [];
    logger.target = base_logger;
    logger.flush = function () {
        for (var i = 0; i < logger.temp.length; i++) {
            var log = logger.temp[i];
            logger.target[log.level](log.message);
            delete logger.temp[i];
        }
    };
    logger.trace = function (message) { logger.temp.push({level: 'trace', message: message}); };
    logger.debug = function (message) { logger.temp.push({level: 'debug', message: message}); };
    logger.info = function (message) { logger.temp.push({level: 'info', message: message}); };
    logger.warn = function (message) { logger.temp.push({level: 'warn', message: message}); };
    logger.error = function (message) { logger.temp.push({level: 'error', message: message}); };
    logger.fatal = function (message) { logger.temp.push({level: 'fatal', message: message}); };

    return logger;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.log4js.getDefaultLogger"></a>[function <span class="apidocSignatureSpan">log4js.</span>getDefaultLogger ()](#apidoc.element.log4js.getDefaultLogger)
- description and source-code
```javascript
function getDefaultLogger() {
  return getLogger(Logger.DEFAULT_CATEGORY);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.log4js.getLogger"></a>[function <span class="apidocSignatureSpan">log4js.</span>getLogger (loggerCategoryName)](#apidoc.element.log4js.getLogger)
- description and source-code
```javascript
function getLogger(loggerCategoryName) {

  // Use default logger if categoryName is not specified or invalid
  if (typeof loggerCategoryName !== "string") {
    loggerCategoryName = Logger.DEFAULT_CATEGORY;
  }

  if (!hasLogger(loggerCategoryName)) {

    var level;

<span class="apidocCodeCommentSpan">    /* jshint -W073 */
</span>    // If there's a "levels" entry in the configuration
    if (levels.config) {
      // Goes through the categories in the levels configuration entry,
      // starting with the "higher" ones.
      var keys = Object.keys(levels.config).sort();
      for (var idx = 0; idx < keys.length; idx++) {
        var levelCategory = keys[idx];
        if (doesLevelEntryContainsLogger(levelCategory, loggerCategoryName)) {
          // level for the logger
          level = levels.config[levelCategory];
        }
      }
    }
    /* jshint +W073 */

    // Create the logger for this name if it doesn't already exist
    loggers[loggerCategoryName] = new Logger(loggerCategoryName, level);

    /* jshint -W083 */
    var appenderList;
    for(var appenderCategory in appenders) {
      if (doesAppenderContainsLogger(appenderCategory, loggerCategoryName)) {
        appenderList = appenders[appenderCategory];
        appenderList.forEach(function(appender) {
          loggers[loggerCategoryName].addListener("log", appender);
        });
      }
    }
    /* jshint +W083 */

    if (appenders[ALL_CATEGORIES]) {
      appenderList = appenders[ALL_CATEGORIES];
      appenderList.forEach(function(appender) {
        loggers[loggerCategoryName].addListener("log", appender);
      });
    }
  }

  return loggers[loggerCategoryName];
}
```
- example usage
```shell
...


## usage

Minimalist version:
'''javascript
var log4js = require('log4js');
var logger = log4js.getLogger();
logger.debug("Some debug messages");
'''
By default, log4js outputs to stdout with the coloured layout (thanks to [masylum](http://github.com/masylum)), so for the above
 you would see:
'''bash
[2010-01-17 11:43:37.987] [DEBUG] [default] - Some debug messages
'''
See example.js for a full example, but here's a snippet (also in fromreadme.js):
...
```

#### <a name="apidoc.element.log4js.hasLogger"></a>[function <span class="apidocSignatureSpan">log4js.</span>hasLogger (logger)](#apidoc.element.log4js.hasLogger)
- description and source-code
```javascript
function hasLogger(logger) {
  return loggers.hasOwnProperty(logger);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.log4js.levels.Level"></a>[function <span class="apidocSignatureSpan">log4js.</span>levels.Level (level, levelStr)](#apidoc.element.log4js.levels.Level)
- description and source-code
```javascript
function Level(level, levelStr) {
  this.level = level;
  this.levelStr = levelStr;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.log4js.loadAppender"></a>[function <span class="apidocSignatureSpan">log4js.</span>loadAppender (appender, appenderModule)](#apidoc.element.log4js.loadAppender)
- description and source-code
```javascript
function loadAppender(appender, appenderModule) {
  appenderModule = appenderModule || requireAppender(appender);

  if (!appenderModule) {
    throw new Error("Invalid log4js appender: " + util.inspect(appender));
  }

  module.exports.appenders[appender] = appenderModule.appender.bind(appenderModule);
  if (appenderModule.shutdown) {
    appenderShutdowns[appender] = appenderModule.shutdown.bind(appenderModule);
  }
  appenderMakers[appender] = appenderModule.configure.bind(appenderModule);
}
```
- example usage
```shell
...
'''bash
[2010-01-17 11:43:37.987] [DEBUG] [default] - Some debug messages
'''
See example.js for a full example, but here's a snippet (also in fromreadme.js):
'''javascript
var log4js = require('log4js');
//console log is loaded by default, so you won't normally need to do this
//log4js.loadAppender('console');
log4js.loadAppender('file');
//log4js.addAppender(log4js.appenders.console());
log4js.addAppender(log4js.appenders.file('logs/cheese.log'), 'cheese');

var logger = log4js.getLogger('cheese');
logger.setLevel('ERROR');
...
```

#### <a name="apidoc.element.log4js.replaceConsole"></a>[function <span class="apidocSignatureSpan">log4js.</span>replaceConsole (logger)](#apidoc.element.log4js.replaceConsole)
- description and source-code
```javascript
function replaceConsole(logger) {
  function replaceWith(fn) {
    return function() {
      fn.apply(logger, arguments);
    };
  }
  logger = logger || getLogger("console");
  ['log','debug','info','warn','error'].forEach(function (item) {
    console[item] = replaceWith(item === 'log' ? logger.info : logger[item]);
  });
}
```
- example usage
```shell
...

The default appender has been changed from 'console' to 'stdout' - this alleviates a memory problem that happens when logging using
 console. If you're using log4js in a browser (via browserify), then you'll probably need to explicitly configure log4js to use
the console appender now (unless browserify handles process.stdout).

I'm also trying to move away from 'vows' for the tests, and use 'tape' instead. New tests should be added to 'test/tape', not the
 vows ones.

log4js also no longer supports node versions below 0.12.x.

NOTE: from log4js 0.5 onwards you'll need to explicitly enable replacement of node's console.log functions. Do this either by calling
 'log4js.replaceConsole()' or configuring with an object or json file like this:

'''javascript
{
appenders: [
  { type: "console" }
],
replaceConsole: true
...
```

#### <a name="apidoc.element.log4js.restoreConsole"></a>[function <span class="apidocSignatureSpan">log4js.</span>restoreConsole ()](#apidoc.element.log4js.restoreConsole)
- description and source-code
```javascript
function restoreConsole() {
  ['log', 'debug', 'info', 'warn', 'error'].forEach(function (item) {
    console[item] = originalConsoleFunctions[item];
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.log4js.setGlobalLogLevel"></a>[function <span class="apidocSignatureSpan">log4js.</span>setGlobalLogLevel (level)](#apidoc.element.log4js.setGlobalLogLevel)
- description and source-code
```javascript
function setGlobalLogLevel(level) {
  Logger.prototype.level = levels.toLevel(level, levels.TRACE);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.log4js.shutdown"></a>[function <span class="apidocSignatureSpan">log4js.</span>shutdown (cb)](#apidoc.element.log4js.shutdown)
- description and source-code
```javascript
function shutdown(cb) {
  // First, disable all writing to appenders. This prevents appenders from
  // not being able to be drained because of run-away log writes.
  loggerModule.disableAllLogWrites();

  //turn off config reloading
  if (configState.timerId) {
    clearInterval(configState.timerId);
  }

  // Call each of the shutdown functions in parallel
  var completed = 0;
  var error;
  var shutdownFcts = [];
  var complete = function(err) {
    error = error || err;
    completed++;
    if (completed >= shutdownFcts.length) {
      cb(error);
    }
  };
  for (var category in appenderShutdowns) {
    if (appenderShutdowns.hasOwnProperty(category)) {
      shutdownFcts.push(appenderShutdowns[category]);
    }
  }
  if (!shutdownFcts.length) {
    return cb();
  }
  shutdownFcts.forEach(function(shutdownFct) { shutdownFct(complete); });
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.log4js.appenderMakers"></a>[module log4js.appenderMakers](#apidoc.module.log4js.appenderMakers)

#### <a name="apidoc.element.log4js.appenderMakers.stdout"></a>[function <span class="apidocSignatureSpan">log4js.appenderMakers.</span>stdout ()](#apidoc.element.log4js.appenderMakers.stdout)
- description and source-code
```javascript
stdout = function () { [native code] }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.log4js.appenders"></a>[module log4js.appenders](#apidoc.module.log4js.appenders)

#### <a name="apidoc.element.log4js.appenders.stdout"></a>[function <span class="apidocSignatureSpan">log4js.appenders.</span>stdout ()](#apidoc.element.log4js.appenders.stdout)
- description and source-code
```javascript
stdout = function () { [native code] }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.log4js.connect_logger"></a>[module log4js.connect_logger](#apidoc.module.log4js.connect_logger)

#### <a name="apidoc.element.log4js.connect_logger.connectLogger"></a>[function <span class="apidocSignatureSpan">log4js.connect_logger.</span>connectLogger (logger4js, options)](#apidoc.element.log4js.connect_logger.connectLogger)
- description and source-code
```javascript
function getLogger(logger4js, options) {
	if ('object' == typeof options) {
		options = options || {};
	} else if (options) {
		options = { format: options };
	} else {
		options = {};
	}

	var thislogger = logger4js
  , level = levels.toLevel(options.level, levels.INFO)
  , fmt = options.format || DEFAULT_FORMAT
  , nolog = options.nolog ? createNoLogCondition(options.nolog) : null;

  return function (req, res, next) {
    // mount safety
    if (req._logging) return next();

		// nologs
		if (nolog && nolog.test(req.originalUrl)) return next();
		if (thislogger.isLevelEnabled(level) || options.level === 'auto') {

			var start = new Date()
			, statusCode
			, writeHead = res.writeHead
			, url = req.originalUrl;

			// flag as logging
			req._logging = true;

			// proxy for statusCode.
			res.writeHead = function(code, headers){
				res.writeHead = writeHead;
				res.writeHead(code, headers);
				res.__statusCode = statusCode = code;
				res.__headers = headers || {};

				//status code response level handling
				if(options.level === 'auto'){
					level = levels.INFO;
					if(code >= 300) level = levels.WARN;
					if(code >= 400) level = levels.ERROR;
				} else {
					level = levels.toLevel(options.level, levels.INFO);
				}
			};

			//hook on end request to emit the log entry of the HTTP request.
			res.on('finish', function() {
				res.responseTime = new Date() - start;
				//status code response level handling
				if(res.statusCode && options.level === 'auto'){
					level = levels.INFO;
					if(res.statusCode >= 300) level = levels.WARN;
					if(res.statusCode >= 400) level = levels.ERROR;
				}
				if (thislogger.isLevelEnabled(level)) {
          var combined_tokens = assemble_tokens(req, res, options.tokens || []);
					if (typeof fmt === 'function') {
						var line = fmt(req, res, function(str){ return format(str, combined_tokens); });
						if (line) thislogger.log(level, line);
					} else {
						thislogger.log(level, format(fmt, combined_tokens));
					}
				}
			});
		}

    //ensure next gets always called
    next();
  };
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.log4js.date_format"></a>[module log4js.date_format](#apidoc.module.log4js.date_format)

#### <a name="apidoc.element.log4js.date_format.asString"></a>[function <span class="apidocSignatureSpan">log4js.date_format.</span>asString (date, timezoneOffset)](#apidoc.element.log4js.date_format.asString)
- description and source-code
```javascript
asString = function (date, timezoneOffset) {
<span class="apidocCodeCommentSpan">  /*jshint -W071 */
</span>  var format = exports.ISO8601_FORMAT;
  if (typeof(date) === "string") {
    format = arguments[0];
    date = arguments[1];
    timezoneOffset = arguments[2];
  }
  // make the date independent of the system timezone by working with UTC
  if (timezoneOffset === undefined) {
    timezoneOffset = date.getTimezoneOffset();
  }
  date.setUTCMinutes(date.getUTCMinutes() - timezoneOffset);
  var vDay = addZero(date.getUTCDate());
  var vMonth = addZero(date.getUTCMonth()+1);
  var vYearLong = addZero(date.getUTCFullYear());
  var vYearShort = addZero(date.getUTCFullYear().toString().substring(2,4));
  var vYear = (format.indexOf("yyyy") > -1 ? vYearLong : vYearShort);
  var vHour  = addZero(date.getUTCHours());
  var vMinute = addZero(date.getUTCMinutes());
  var vSecond = addZero(date.getUTCSeconds());
  var vMillisecond = padWithZeros(date.getUTCMilliseconds(), 3);
  var vTimeZone = offset(timezoneOffset);
  date.setUTCMinutes(date.getUTCMinutes() + timezoneOffset);
  var formatted = format
    .replace(/dd/g, vDay)
    .replace(/MM/g, vMonth)
    .replace(/y{1,4}/g, vYear)
    .replace(/hh/g, vHour)
    .replace(/mm/g, vMinute)
    .replace(/ss/g, vSecond)
    .replace(/SSS/g, vMillisecond)
    .replace(/O/g, vTimeZone);
  return formatted;

}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.log4js.layouts"></a>[module log4js.layouts](#apidoc.module.log4js.layouts)

#### <a name="apidoc.element.log4js.layouts.addLayout"></a>[function <span class="apidocSignatureSpan">log4js.layouts.</span>addLayout (name, serializerGenerator)](#apidoc.element.log4js.layouts.addLayout)
- description and source-code
```javascript
addLayout = function (name, serializerGenerator) {
  layoutMakers[name] = serializerGenerator;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.log4js.layouts.basicLayout"></a>[function <span class="apidocSignatureSpan">log4js.layouts.</span>basicLayout (loggingEvent, timezoneOffset)](#apidoc.element.log4js.layouts.basicLayout)
- description and source-code
```javascript
function basicLayout(loggingEvent, timezoneOffset) {
  return timestampLevelAndCategory(
    loggingEvent,
    undefined,
    timezoneOffset
  ) + formatLogData(loggingEvent.data);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.log4js.layouts.coloredLayout"></a>[function <span class="apidocSignatureSpan">log4js.layouts.</span>coloredLayout (loggingEvent, timezoneOffset)](#apidoc.element.log4js.layouts.coloredLayout)
- description and source-code
```javascript
function colouredLayout(loggingEvent, timezoneOffset) {
  return timestampLevelAndCategory(
    loggingEvent,
    colours[loggingEvent.level.toString()],
    timezoneOffset
  ) + formatLogData(loggingEvent.data);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.log4js.layouts.colouredLayout"></a>[function <span class="apidocSignatureSpan">log4js.layouts.</span>colouredLayout (loggingEvent, timezoneOffset)](#apidoc.element.log4js.layouts.colouredLayout)
- description and source-code
```javascript
function colouredLayout(loggingEvent, timezoneOffset) {
  return timestampLevelAndCategory(
    loggingEvent,
    colours[loggingEvent.level.toString()],
    timezoneOffset
  ) + formatLogData(loggingEvent.data);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.log4js.layouts.dummyLayout"></a>[function <span class="apidocSignatureSpan">log4js.layouts.</span>dummyLayout (loggingEvent)](#apidoc.element.log4js.layouts.dummyLayout)
- description and source-code
```javascript
function dummyLayout(loggingEvent) {
  return loggingEvent.data[0];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.log4js.layouts.layout"></a>[function <span class="apidocSignatureSpan">log4js.layouts.</span>layout (name, config)](#apidoc.element.log4js.layouts.layout)
- description and source-code
```javascript
layout = function (name, config) {
  return layoutMakers[name] && layoutMakers[name](config);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.log4js.layouts.messagePassThroughLayout"></a>[function <span class="apidocSignatureSpan">log4js.layouts.</span>messagePassThroughLayout (loggingEvent)](#apidoc.element.log4js.layouts.messagePassThroughLayout)
- description and source-code
```javascript
function messagePassThroughLayout(loggingEvent) {
  return formatLogData(loggingEvent.data);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.log4js.layouts.patternLayout"></a>[function <span class="apidocSignatureSpan">log4js.layouts.</span>patternLayout (pattern, tokens, timezoneOffset)](#apidoc.element.log4js.layouts.patternLayout)
- description and source-code
```javascript
function patternLayout(pattern, tokens, timezoneOffset) {
  // jshint maxstatements:22
  var TTCC_CONVERSION_PATTERN  = "%r %p %c - %m%n";
  var regex = /%(-?[0-9]+)?(\.?[0-9]+)?([\[\]cdhmnprzxy%])(\{([^\}]+)\})?|([^%]+)/;

  pattern = pattern || TTCC_CONVERSION_PATTERN;

  function categoryName(loggingEvent, specifier) {
    var loggerName = loggingEvent.categoryName;
    if (specifier) {
      var precision = parseInt(specifier, 10);
      var loggerNameBits = loggerName.split(".");
      if (precision < loggerNameBits.length) {
        loggerName = loggerNameBits.slice(loggerNameBits.length - precision).join(".");
      }
    }
    return loggerName;
  }

  function formatAsDate(loggingEvent, specifier) {
    var format = dateFormat.ISO8601_FORMAT;
    if (specifier) {
      format = specifier;
      // Pick up special cases
      if (format == "ISO8601") {
        format = dateFormat.ISO8601_FORMAT;
      } else if (format == "ISO8601_WITH_TZ_OFFSET") {
        format = dateFormat.ISO8601_WITH_TZ_OFFSET_FORMAT;
      } else if (format == "ABSOLUTE") {
        format = dateFormat.ABSOLUTETIME_FORMAT;
      } else if (format == "DATE") {
        format = dateFormat.DATETIME_FORMAT;
      }
    }
    // Format the date
    return dateFormat.asString(format, loggingEvent.startTime, timezoneOffset);
  }

  function hostname() {
    return os.hostname().toString();
  }

  function formatMessage(loggingEvent) {
    return formatLogData(loggingEvent.data);
  }

  function endOfLine() {
    return eol;
  }

  function logLevel(loggingEvent) {
    return loggingEvent.level.toString();
  }

  function startTime(loggingEvent) {
    return dateFormat.asString('hh:mm:ss', loggingEvent.startTime, timezoneOffset);
  }

  function startColour(loggingEvent) {
    return colorizeStart(colours[loggingEvent.level.toString()]);
  }

  function endColour(loggingEvent) {
    return colorizeEnd(colours[loggingEvent.level.toString()]);
  }

  function percent() {
    return '%';
  }

  function pid(loggingEvent) {
    if (loggingEvent && loggingEvent.pid) {
      return loggingEvent.pid;
    } else {
      return process.pid;
    }
  }

  function clusterInfo(loggingEvent, specifier) {
    if (loggingEvent.cluster && specifier) {
      return specifier
        .replace('%m', loggingEvent.cluster.master)
        .replace('%w', loggingEvent.cluster.worker)
        .replace('%i', loggingEvent.cluster.workerId);
    } else if (loggingEvent.cluster) {
      return loggingEvent.cluster.worker+'@'+loggingEvent.cluster.master;
    } else {
      return pid();
    }
  }

  function userDefined(loggingEvent, specifier) {
    if (typeof(tokens[specifier]) !== 'undefined') {
      if (typeof(tokens[specifier]) === 'function') {
        return tokens[specifier](loggingEvent);
      } else {
        return tokens[specifier];
      }
    }
    return null;
  }

  var replacers = {
    'c': categoryName,
    'd': formatAsDate,
    'h': hostname,
    'm': formatMessage,
    'n': endOfLine,
    'p': logLevel,
    'r': startTime,
    '[': startColour,
    ']': endColour,
    'y': clusterInfo,
    'z': pid,
    '%': percent,
    'x': userDefined
  };

  function replaceToken(conversionCharacter, loggingEvent, specifier) {
    return replacers[conversionCharacter](loggingEvent, specifier);
  }

  function truncate(truncation, toTruncate) {
    var len;
    if (truncation) {
      len = parseInt(truncation.substr(1), 10);
      return toTruncate.substring(0, len);
    }

    return toTruncate;
  }

  function pad(padding, toPad) {
    var len;
    if (padding) {
      if (padding.charAt(0) == "-") {
        len = parseInt(padding.substr(1), 10);
        // Right pad with spaces
        while (toPad.length < len) {
          toPad += " ";
        }
      } else {
        len = parseInt(padding, 10);
        // Left pad with spaces
        while (toPad.length < len) {
          toPad = " " + toPad;
        }
      }
    }
    return toPad;
  }

  function truncateAndPad(toTruncAndPad, truncation, padding) {
    var replacement = toTruncAndPad;
    replacement = trun ...
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.log4js.levels"></a>[module log4js.levels](#apidoc.module.log4js.levels)

#### <a name="apidoc.element.log4js.levels.Level"></a>[function <span class="apidocSignatureSpan">log4js.levels.</span>Level (level, levelStr)](#apidoc.element.log4js.levels.Level)
- description and source-code
```javascript
function Level(level, levelStr) {
  this.level = level;
  this.levelStr = levelStr;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.log4js.levels.forName"></a>[function <span class="apidocSignatureSpan">log4js.levels.</span>forName (levelStr, levelVal)](#apidoc.element.log4js.levels.forName)
- description and source-code
```javascript
forName = function (levelStr, levelVal) {
  var level;
  if (typeof levelStr === "string" && typeof levelVal === "number") {
    var levelUpper = levelStr.toUpperCase();
    level = new levels.Level(levelVal, levelUpper);
    loggerModule.addLevelMethods(level);
  }
  return level;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.log4js.levels.getLevel"></a>[function <span class="apidocSignatureSpan">log4js.levels.</span>getLevel (levelStr)](#apidoc.element.log4js.levels.getLevel)
- description and source-code
```javascript
getLevel = function (levelStr) {
  var level;
  if (typeof levelStr === "string") {
    var levelUpper = levelStr.toUpperCase();
    level = levels.toLevel(levelStr);
  }
  return level;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.log4js.levels.toLevel"></a>[function <span class="apidocSignatureSpan">log4js.levels.</span>toLevel (sArg, defaultLevel)](#apidoc.element.log4js.levels.toLevel)
- description and source-code
```javascript
function toLevel(sArg, defaultLevel) {
  if (!sArg) {
    return defaultLevel;
  }
  if (sArg instanceof Level) {
    module.exports[sArg.toString()] = sArg;
    return sArg;
  }
  if (typeof sArg === "string") {
    return module.exports[sArg.toUpperCase()] || defaultLevel;
  }
  return toLevel(sArg.toString());
}
```
- example usage
```shell
...
	} else if (options) {
		options = { format: options };
	} else {
		options = {};
	}

	var thislogger = logger4js
, level = levels.toLevel(options.level, levels.INFO)
, fmt = options.format || DEFAULT_FORMAT
, nolog = options.nolog ? createNoLogCondition(options.nolog) : null;

return function (req, res, next) {
  // mount safety
  if (req._logging) return next();
...
```



# <a name="apidoc.module.log4js.levels.Level"></a>[module log4js.levels.Level](#apidoc.module.log4js.levels.Level)

#### <a name="apidoc.element.log4js.levels.Level.Level"></a>[function <span class="apidocSignatureSpan">log4js.levels.</span>Level (level, levelStr)](#apidoc.element.log4js.levels.Level.Level)
- description and source-code
```javascript
function Level(level, levelStr) {
  this.level = level;
  this.levelStr = levelStr;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.log4js.levels.Level.prototype"></a>[module log4js.levels.Level.prototype](#apidoc.module.log4js.levels.Level.prototype)

#### <a name="apidoc.element.log4js.levels.Level.prototype.isEqualTo"></a>[function <span class="apidocSignatureSpan">log4js.levels.Level.prototype.</span>isEqualTo (otherLevel)](#apidoc.element.log4js.levels.Level.prototype.isEqualTo)
- description and source-code
```javascript
isEqualTo = function (otherLevel) {
  if (typeof otherLevel === "string") {
    otherLevel = toLevel(otherLevel);
  }
  return this.level === otherLevel.level;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.log4js.levels.Level.prototype.isGreaterThanOrEqualTo"></a>[function <span class="apidocSignatureSpan">log4js.levels.Level.prototype.</span>isGreaterThanOrEqualTo (otherLevel)](#apidoc.element.log4js.levels.Level.prototype.isGreaterThanOrEqualTo)
- description and source-code
```javascript
isGreaterThanOrEqualTo = function (otherLevel) {
  if (typeof otherLevel === "string") {
    otherLevel = toLevel(otherLevel);
  }
  return this.level >= otherLevel.level;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.log4js.levels.Level.prototype.isLessThanOrEqualTo"></a>[function <span class="apidocSignatureSpan">log4js.levels.Level.prototype.</span>isLessThanOrEqualTo (otherLevel)](#apidoc.element.log4js.levels.Level.prototype.isLessThanOrEqualTo)
- description and source-code
```javascript
isLessThanOrEqualTo = function (otherLevel) {
  if (typeof otherLevel === "string") {
    otherLevel = toLevel(otherLevel);
  }
  return this.level <= otherLevel.level;
}
```
- example usage
```shell
...
for (var i = 0; i < numArgs; i++) {
  args[i] = arguments[i + 1];
}
this._log(logLevel, args);
};

Logger.prototype.isLevelEnabled = function(otherLevel) {
return this.level.isLessThanOrEqualTo(otherLevel);
};

['Trace','Debug','Info','Warn','Error','Fatal', 'Mark'].forEach(addLevelMethods);

function addLevelMethods(level) {
level = levels.toLevel(level);
...
```

#### <a name="apidoc.element.log4js.levels.Level.prototype.toString"></a>[function <span class="apidocSignatureSpan">log4js.levels.Level.prototype.</span>toString ()](#apidoc.element.log4js.levels.Level.prototype.toString)
- description and source-code
```javascript
toString = function () {
  return this.levelStr;
}
```
- example usage
```shell
...
if (timezoneOffset === undefined) {
  timezoneOffset = date.getTimezoneOffset();
}
date.setUTCMinutes(date.getUTCMinutes() - timezoneOffset);
var vDay = addZero(date.getUTCDate());
var vMonth = addZero(date.getUTCMonth()+1);
var vYearLong = addZero(date.getUTCFullYear());
var vYearShort = addZero(date.getUTCFullYear().toString().substring(2,4));
var vYear = (format.indexOf("yyyy") > -1 ? vYearLong : vYearShort);
var vHour  = addZero(date.getUTCHours());
var vMinute = addZero(date.getUTCMinutes());
var vSecond = addZero(date.getUTCSeconds());
var vMillisecond = padWithZeros(date.getUTCMilliseconds(), 3);
var vTimeZone = offset(timezoneOffset);
date.setUTCMinutes(date.getUTCMinutes() + timezoneOffset);
...
```



# <a name="apidoc.module.log4js.logger"></a>[module log4js.logger](#apidoc.module.log4js.logger)

#### <a name="apidoc.element.log4js.logger.Logger"></a>[function <span class="apidocSignatureSpan">log4js.logger.</span>Logger (name, level)](#apidoc.element.log4js.logger.Logger)
- description and source-code
```javascript
function Logger(name, level) {
  this.category = name || DEFAULT_CATEGORY;

  if (level) {
    this.setLevel(level);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.log4js.logger.LoggingEvent"></a>[function <span class="apidocSignatureSpan">log4js.logger.</span>LoggingEvent (categoryName, level, data, logger)](#apidoc.element.log4js.logger.LoggingEvent)
- description and source-code
```javascript
function LoggingEvent(categoryName, level, data, logger) {
  this.startTime = new Date();
  this.categoryName = categoryName;
  this.data = data;
  this.level = level;
  this.logger = logger;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.log4js.logger.addLevelMethods"></a>[function <span class="apidocSignatureSpan">log4js.logger.</span>addLevelMethods (level)](#apidoc.element.log4js.logger.addLevelMethods)
- description and source-code
```javascript
function addLevelMethods(level) {
  level = levels.toLevel(level);

  var levelStrLower = level.toString().toLowerCase();
  var levelMethod = levelStrLower.replace(/_([a-z])/g, function(g) { return g[1].toUpperCase(); } );
  var isLevelMethod = levelMethod[0].toUpperCase() + levelMethod.slice(1);

  Logger.prototype['is'+isLevelMethod+'Enabled'] = function() {
    return this.isLevelEnabled(level);
  };

  Logger.prototype[levelMethod] = function () {
    if (logWritesEnabled && this.isLevelEnabled(level)) {
      var numArgs = arguments.length;
      var args = new Array(numArgs);
      for (var i = 0; i < numArgs; i++) {
        args[i] = arguments[i];
      }
      this._log(level, args);
    }
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.log4js.logger.disableAllLogWrites"></a>[function <span class="apidocSignatureSpan">log4js.logger.</span>disableAllLogWrites ()](#apidoc.element.log4js.logger.disableAllLogWrites)
- description and source-code
```javascript
function disableAllLogWrites() {
  logWritesEnabled = false;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.log4js.logger.enableAllLogWrites"></a>[function <span class="apidocSignatureSpan">log4js.logger.</span>enableAllLogWrites ()](#apidoc.element.log4js.logger.enableAllLogWrites)
- description and source-code
```javascript
function enableAllLogWrites() {
  logWritesEnabled = true;
}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
