# api documentation for  [fis (v1.10.5)](http://fis.baidu.com/)  [![npm package](https://img.shields.io/npm/v/npmdoc-fis.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-fis) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-fis.svg)](https://travis-ci.org/npmdoc/node-npmdoc-fis)
#### front-end integrated solution.

[![NPM](https://nodei.co/npm/fis.png?downloads=true)](https://www.npmjs.com/package/fis)

[![apidoc](https://npmdoc.github.io/node-npmdoc-fis/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-fis_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-fis/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-fis/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-fis/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "FIS Team",
        "email": "fis@baidu.com"
    },
    "bin": {
        "fis": "bin/fis"
    },
    "bugs": {
        "url": "https://github.com/fis-dev/fis/issues"
    },
    "dependencies": {
        "colors": "0.6.2",
        "commander": "1.3.2",
        "fis-command-install": "0.2.15",
        "fis-command-release": "0.13.0",
        "fis-command-server": "0.7.9",
        "fis-deploy-default": "0.1.3",
        "fis-kernel": "2.0.19",
        "fis-optimizer-clean-css": "0.0.9",
        "fis-optimizer-png-compressor": "0.1.6",
        "fis-optimizer-uglify-js": "0.1.14",
        "fis-packager-map": "0.0.9",
        "fis-postprocessor-jswrapper": "0.0.12",
        "fis-prepackager-derived": "0.0.3",
        "fis-preprocessor-components": "1.0.19",
        "fis-spriter-csssprites": "0.3.11"
    },
    "description": "front-end integrated solution.",
    "devDependencies": {},
    "directories": {},
    "dist": {
        "shasum": "61ce1174074fcdef0073f47fdbd79b4fc4e91e22",
        "tarball": "https://registry.npmjs.org/fis/-/fis-1.10.5.tgz"
    },
    "engines": {
        "node": ">= 0.8.0"
    },
    "gitHead": "19b38bc7be1d9198e421422e9e0b87bbc482c134",
    "homepage": "http://fis.baidu.com/",
    "keywords": [
        "fis"
    ],
    "license": "MIT",
    "main": "fis.js",
    "maintainers": [
        {
            "name": "fis-dev",
            "email": "longyun_zh@163.com"
        },
        {
            "name": "fouber",
            "email": "longyun_zh@163.com"
        },
        {
            "name": "fansekey",
            "email": "fansekey@gmail.com"
        },
        {
            "name": "2betop",
            "email": "2betop.cn@gmail.com"
        },
        {
            "name": "hefangshi",
            "email": "hefangshi@gmail.com"
        }
    ],
    "name": "fis",
    "optionalDependencies": {},
    "preferGlobal": true,
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+https://github.com/fis-dev/fis.git"
    },
    "scripts": {
        "test": "mocha test/ut --recursive",
        "uninstall": "node -e \"var cp = require('child_process'); cp.exec('bin/fis server stop');\""
    },
    "version": "1.10.5"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module fis](#apidoc.module.fis)
1.  [function <span class="apidocSignatureSpan">fis.</span>cache ()](#apidoc.element.fis.cache)
1.  [function <span class="apidocSignatureSpan">fis.</span>cache.Cache ()](#apidoc.element.fis.cache.Cache)
1.  [function <span class="apidocSignatureSpan">fis.</span>compile (file)](#apidoc.element.fis.compile)
1.  [function <span class="apidocSignatureSpan">fis.</span>config.Config ()](#apidoc.element.fis.config.Config)
1.  [function <span class="apidocSignatureSpan">fis.</span>file ()](#apidoc.element.fis.file)
1.  [function <span class="apidocSignatureSpan">fis.</span>release (opt, callback)](#apidoc.element.fis.release)
1.  [function <span class="apidocSignatureSpan">fis.</span>require ()](#apidoc.element.fis.require)
1.  [function <span class="apidocSignatureSpan">fis.</span>time (title)](#apidoc.element.fis.time)
1.  [function <span class="apidocSignatureSpan">fis.</span>uri (path, dirname)](#apidoc.element.fis.uri)
1.  [function <span class="apidocSignatureSpan">fis.</span>util (path)](#apidoc.element.fis.util)
1.  object <span class="apidocSignatureSpan">fis.</span>cache.Cache.prototype
1.  object <span class="apidocSignatureSpan">fis.</span>cli
1.  object <span class="apidocSignatureSpan">fis.</span>cli.colors
1.  object <span class="apidocSignatureSpan">fis.</span>compile.settings
1.  object <span class="apidocSignatureSpan">fis.</span>config
1.  object <span class="apidocSignatureSpan">fis.</span>config.Config.prototype
1.  object <span class="apidocSignatureSpan">fis.</span>emitter
1.  object <span class="apidocSignatureSpan">fis.</span>info
1.  object <span class="apidocSignatureSpan">fis.</span>log
1.  object <span class="apidocSignatureSpan">fis.</span>log.on
1.  object <span class="apidocSignatureSpan">fis.</span>project
1.  string <span class="apidocSignatureSpan">fis.</span>version

#### [module fis.cache](#apidoc.module.fis.cache)
1.  boolean <span class="apidocSignatureSpan">fis.cache.</span>enable
1.  [function <span class="apidocSignatureSpan">fis.</span>cache ()](#apidoc.element.fis.cache.cache)
1.  [function <span class="apidocSignatureSpan">fis.cache.</span>Cache ()](#apidoc.element.fis.cache.Cache)
1.  [function <span class="apidocSignatureSpan">fis.cache.</span>clean (name)](#apidoc.element.fis.cache.clean)

#### [module fis.cache.Cache](#apidoc.module.fis.cache.Cache)
1.  [function <span class="apidocSignatureSpan">fis.cache.</span>Cache ()](#apidoc.element.fis.cache.Cache.Cache)

#### [module fis.cache.Cache.prototype](#apidoc.module.fis.cache.Cache.prototype)
1.  [function <span class="apidocSignatureSpan">fis.cache.Cache.prototype.</span>addDeps (file)](#apidoc.element.fis.cache.Cache.prototype.addDeps)
1.  [function <span class="apidocSignatureSpan">fis.cache.Cache.prototype.</span>constructor (path, dir)](#apidoc.element.fis.cache.Cache.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">fis.cache.Cache.prototype.</span>mergeDeps (cache)](#apidoc.element.fis.cache.Cache.prototype.mergeDeps)
1.  [function <span class="apidocSignatureSpan">fis.cache.Cache.prototype.</span>removeDeps (file)](#apidoc.element.fis.cache.Cache.prototype.removeDeps)
1.  [function <span class="apidocSignatureSpan">fis.cache.Cache.prototype.</span>revert (file)](#apidoc.element.fis.cache.Cache.prototype.revert)
1.  [function <span class="apidocSignatureSpan">fis.cache.Cache.prototype.</span>save (content, info)](#apidoc.element.fis.cache.Cache.prototype.save)

#### [module fis.cli](#apidoc.module.fis.cli)
1.  [function <span class="apidocSignatureSpan">fis.cli.</span>help ()](#apidoc.element.fis.cli.help)
1.  [function <span class="apidocSignatureSpan">fis.cli.</span>run (argv)](#apidoc.element.fis.cli.run)
1.  [function <span class="apidocSignatureSpan">fis.cli.</span>version ()](#apidoc.element.fis.cli.version)
1.  object <span class="apidocSignatureSpan">fis.cli.</span>colors
1.  object <span class="apidocSignatureSpan">fis.cli.</span>commander
1.  object <span class="apidocSignatureSpan">fis.cli.</span>info
1.  string <span class="apidocSignatureSpan">fis.cli.</span>name

#### [module fis.cli.colors](#apidoc.module.fis.cli.colors)
1.  [function <span class="apidocSignatureSpan">fis.cli.colors.</span>addSequencer (name, map)](#apidoc.element.fis.cli.colors.addSequencer)
1.  [function <span class="apidocSignatureSpan">fis.cli.colors.</span>black (str)](#apidoc.element.fis.cli.colors.black)
1.  [function <span class="apidocSignatureSpan">fis.cli.colors.</span>blackBG (str)](#apidoc.element.fis.cli.colors.blackBG)
1.  [function <span class="apidocSignatureSpan">fis.cli.colors.</span>blue (str)](#apidoc.element.fis.cli.colors.blue)
1.  [function <span class="apidocSignatureSpan">fis.cli.colors.</span>blueBG (str)](#apidoc.element.fis.cli.colors.blueBG)
1.  [function <span class="apidocSignatureSpan">fis.cli.colors.</span>bold (str)](#apidoc.element.fis.cli.colors.bold)
1.  [function <span class="apidocSignatureSpan">fis.cli.colors.</span>cyan (str)](#apidoc.element.fis.cli.colors.cyan)
1.  [function <span class="apidocSignatureSpan">fis.cli.colors.</span>cyanBG (str)](#apidoc.element.fis.cli.colors.cyanBG)
1.  [function <span class="apidocSignatureSpan">fis.cli.colors.</span>green (str)](#apidoc.element.fis.cli.colors.green)
1.  [function <span class="apidocSignatureSpan">fis.cli.colors.</span>greenBG (str)](#apidoc.element.fis.cli.colors.greenBG)
1.  [function <span class="apidocSignatureSpan">fis.cli.colors.</span>grey (str)](#apidoc.element.fis.cli.colors.grey)
1.  [function <span class="apidocSignatureSpan">fis.cli.colors.</span>greyBG (str)](#apidoc.element.fis.cli.colors.greyBG)
1.  [function <span class="apidocSignatureSpan">fis.cli.colors.</span>inverse (str)](#apidoc.element.fis.cli.colors.inverse)
1.  [function <span class="apidocSignatureSpan">fis.cli.colors.</span>italic (str)](#apidoc.element.fis.cli.colors.italic)
1.  [function <span class="apidocSignatureSpan">fis.cli.colors.</span>magenta (str)](#apidoc.element.fis.cli.colors.magenta)
1.  [function <span class="apidocSignatureSpan">fis.cli.colors.</span>magentaBG (str)](#apidoc.element.fis.cli.colors.magentaBG)
1.  [function <span class="apidocSignatureSpan">fis.cli.colors.</span>rainbow (str)](#apidoc.element.fis.cli.colors.rainbow)
1.  [function <span class="apidocSignatureSpan">fis.cli.colors.</span>red (str)](#apidoc.element.fis.cli.colors.red)
1.  [function <span class="apidocSignatureSpan">fis.cli.colors.</span>redBG (str)](#apidoc.element.fis.cli.colors.redBG)
1.  [function <span class="apidocSignatureSpan">fis.cli.colors.</span>setTheme (theme)](#apidoc.element.fis.cli.colors.setTheme)
1.  [function <span class="apidocSignatureSpan">fis.cli.colors.</span>strikethrough (str)](#apidoc.element.fis.cli.colors.strikethrough)
1.  [function <span class="apidocSignatureSpan">fis.cli.colors.</span>stripColors (str)](#apidoc.element.fis.cli.colors.stripColors)
1.  [function <span class="apidocSignatureSpan">fis.cli.colors.</span>underline (str)](#apidoc.element.fis.cli.colors.underline)
1.  [function <span class="apidocSignatureSpan">fis.cli.colors.</span>white (str)](#apidoc.element.fis.cli.colors.white)
1.  [function <span class="apidocSignatureSpan">fis.cli.colors.</span>whiteBG (str)](#apidoc.element.fis.cli.colors.whiteBG)
1.  [function <span class="apidocSignatureSpan">fis.cli.colors.</span>yellow (str)](#apidoc.element.fis.cli.colors.yellow)
1.  [function <span class="apidocSignatureSpan">fis.cli.colors.</span>yellowBG (str)](#apidoc.element.fis.cli.colors.yellowBG)
1.  [function <span class="apidocSignatureSpan">fis.cli.colors.</span>zalgo (str)](#apidoc.element.fis.cli.colors.zalgo)
1.  [function <span class="apidocSignatureSpan">fis.cli.colors.</span>zebra (str)](#apidoc.element.fis.cli.colors.zebra)
1.  object <span class="apidocSignatureSpan">fis.cli.colors.</span>themes
1.  string <span class="apidocSignatureSpan">fis.cli.colors.</span>mode

#### [module fis.compile](#apidoc.module.fis.compile)
1.  [function <span class="apidocSignatureSpan">fis.</span>compile (file)](#apidoc.element.fis.compile.compile)
1.  [function <span class="apidocSignatureSpan">fis.compile.</span>analyseComment (comment, callback)](#apidoc.element.fis.compile.analyseComment)
1.  [function <span class="apidocSignatureSpan">fis.compile.</span>clean (name)](#apidoc.element.fis.compile.clean)
1.  [function <span class="apidocSignatureSpan">fis.compile.</span>extCss (content, callback)](#apidoc.element.fis.compile.extCss)
1.  [function <span class="apidocSignatureSpan">fis.compile.</span>extHtml (content, callback)](#apidoc.element.fis.compile.extHtml)
1.  [function <span class="apidocSignatureSpan">fis.compile.</span>extJs (content, callback)](#apidoc.element.fis.compile.extJs)
1.  [function <span class="apidocSignatureSpan">fis.compile.</span>isInline (info)](#apidoc.element.fis.compile.isInline)
1.  [function <span class="apidocSignatureSpan">fis.compile.</span>setup (opt)](#apidoc.element.fis.compile.setup)
1.  object <span class="apidocSignatureSpan">fis.compile.</span>lang
1.  object <span class="apidocSignatureSpan">fis.compile.</span>settings

#### [module fis.compile.settings](#apidoc.module.fis.compile.settings)
1.  boolean <span class="apidocSignatureSpan">fis.compile.settings.</span>debug
1.  boolean <span class="apidocSignatureSpan">fis.compile.settings.</span>domain
1.  boolean <span class="apidocSignatureSpan">fis.compile.settings.</span>hash
1.  boolean <span class="apidocSignatureSpan">fis.compile.settings.</span>lint
1.  boolean <span class="apidocSignatureSpan">fis.compile.settings.</span>optimize
1.  boolean <span class="apidocSignatureSpan">fis.compile.settings.</span>test
1.  boolean <span class="apidocSignatureSpan">fis.compile.settings.</span>unique
1.  [function <span class="apidocSignatureSpan">fis.compile.settings.</span>afterCacheRevert ()](#apidoc.element.fis.compile.settings.afterCacheRevert)
1.  [function <span class="apidocSignatureSpan">fis.compile.settings.</span>afterCompile ()](#apidoc.element.fis.compile.settings.afterCompile)
1.  [function <span class="apidocSignatureSpan">fis.compile.settings.</span>beforeCacheRevert ()](#apidoc.element.fis.compile.settings.beforeCacheRevert)
1.  [function <span class="apidocSignatureSpan">fis.compile.settings.</span>beforeCompile ()](#apidoc.element.fis.compile.settings.beforeCompile)

#### [module fis.config](#apidoc.module.fis.config)
1.  [function <span class="apidocSignatureSpan">fis.config.</span>Config ()](#apidoc.element.fis.config.Config)
1.  object <span class="apidocSignatureSpan">fis.config.</span>data

#### [module fis.config.Config](#apidoc.module.fis.config.Config)
1.  [function <span class="apidocSignatureSpan">fis.config.</span>Config ()](#apidoc.element.fis.config.Config.Config)

#### [module fis.config.Config.prototype](#apidoc.module.fis.config.Config.prototype)
1.  [function <span class="apidocSignatureSpan">fis.config.Config.prototype.</span>constructor ()](#apidoc.element.fis.config.Config.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">fis.config.Config.prototype.</span>del (path)](#apidoc.element.fis.config.Config.prototype.del)
1.  [function <span class="apidocSignatureSpan">fis.config.Config.prototype.</span>get (path, def)](#apidoc.element.fis.config.Config.prototype.get)
1.  [function <span class="apidocSignatureSpan">fis.config.Config.prototype.</span>init ()](#apidoc.element.fis.config.Config.prototype.init)
1.  [function <span class="apidocSignatureSpan">fis.config.Config.prototype.</span>merge ()](#apidoc.element.fis.config.Config.prototype.merge)
1.  [function <span class="apidocSignatureSpan">fis.config.Config.prototype.</span>require (name)](#apidoc.element.fis.config.Config.prototype.require)
1.  [function <span class="apidocSignatureSpan">fis.config.Config.prototype.</span>set (path, value)](#apidoc.element.fis.config.Config.prototype.set)

#### [module fis.file](#apidoc.module.fis.file)
1.  [function <span class="apidocSignatureSpan">fis.</span>file ()](#apidoc.element.fis.file.file)
1.  [function <span class="apidocSignatureSpan">fis.file.</span>wrap (file)](#apidoc.element.fis.file.wrap)

#### [module fis.log](#apidoc.module.fis.log)
1.  boolean <span class="apidocSignatureSpan">fis.log.</span>alert
1.  boolean <span class="apidocSignatureSpan">fis.log.</span>throw
1.  [function <span class="apidocSignatureSpan">fis.log.</span>debug (msg)](#apidoc.element.fis.log.debug)
1.  [function <span class="apidocSignatureSpan">fis.log.</span>error (err)](#apidoc.element.fis.log.error)
1.  [function <span class="apidocSignatureSpan">fis.log.</span>notice (msg)](#apidoc.element.fis.log.notice)
1.  [function <span class="apidocSignatureSpan">fis.log.</span>now (withoutMilliseconds)](#apidoc.element.fis.log.now)
1.  [function <span class="apidocSignatureSpan">fis.log.</span>warning (msg)](#apidoc.element.fis.log.warning)
1.  number <span class="apidocSignatureSpan">fis.log.</span>L_ALL
1.  number <span class="apidocSignatureSpan">fis.log.</span>L_DEBUG
1.  number <span class="apidocSignatureSpan">fis.log.</span>L_ERROR
1.  number <span class="apidocSignatureSpan">fis.log.</span>L_NORMAL
1.  number <span class="apidocSignatureSpan">fis.log.</span>L_NOTIC
1.  number <span class="apidocSignatureSpan">fis.log.</span>L_WARNI
1.  number <span class="apidocSignatureSpan">fis.log.</span>level
1.  object <span class="apidocSignatureSpan">fis.log.</span>on

#### [module fis.log.on](#apidoc.module.fis.log.on)
1.  [function <span class="apidocSignatureSpan">fis.log.on.</span>any (type, msg)](#apidoc.element.fis.log.on.any)
1.  [function <span class="apidocSignatureSpan">fis.log.on.</span>debug (msg)](#apidoc.element.fis.log.on.debug)
1.  [function <span class="apidocSignatureSpan">fis.log.on.</span>error (msg)](#apidoc.element.fis.log.on.error)
1.  [function <span class="apidocSignatureSpan">fis.log.on.</span>notice (msg)](#apidoc.element.fis.log.on.notice)
1.  [function <span class="apidocSignatureSpan">fis.log.on.</span>warning (msg)](#apidoc.element.fis.log.on.warning)

#### [module fis.project](#apidoc.module.fis.project)
1.  [function <span class="apidocSignatureSpan">fis.project.</span>getCachePath ()](#apidoc.element.fis.project.getCachePath)
1.  [function <span class="apidocSignatureSpan">fis.project.</span>getProjectPath ()](#apidoc.element.fis.project.getProjectPath)
1.  [function <span class="apidocSignatureSpan">fis.project.</span>getSource ()](#apidoc.element.fis.project.getSource)
1.  [function <span class="apidocSignatureSpan">fis.project.</span>getTempPath ()](#apidoc.element.fis.project.getTempPath)
1.  [function <span class="apidocSignatureSpan">fis.project.</span>setProjectRoot (path)](#apidoc.element.fis.project.setProjectRoot)
1.  [function <span class="apidocSignatureSpan">fis.project.</span>setTempRoot (tmp)](#apidoc.element.fis.project.setTempRoot)
1.  string <span class="apidocSignatureSpan">fis.project.</span>DEFAULT_REMOTE_REPOS

#### [module fis.uri](#apidoc.module.fis.uri)
1.  [function <span class="apidocSignatureSpan">fis.</span>uri (path, dirname)](#apidoc.element.fis.uri.uri)
1.  [function <span class="apidocSignatureSpan">fis.uri.</span>getId (path, dirname)](#apidoc.element.fis.uri.getId)
1.  [function <span class="apidocSignatureSpan">fis.uri.</span>replaceDefine (value, escape)](#apidoc.element.fis.uri.replaceDefine)
1.  [function <span class="apidocSignatureSpan">fis.uri.</span>replaceMatches (value, matches)](#apidoc.element.fis.uri.replaceMatches)
1.  [function <span class="apidocSignatureSpan">fis.uri.</span>replaceProperties (source, matches, target)](#apidoc.element.fis.uri.replaceProperties)
1.  [function <span class="apidocSignatureSpan">fis.uri.</span>roadmap (subpath, path, obj)](#apidoc.element.fis.uri.roadmap)

#### [module fis.util](#apidoc.module.fis.util)
1.  [function <span class="apidocSignatureSpan">fis.</span>util (path)](#apidoc.element.fis.util.util)
1.  [function <span class="apidocSignatureSpan">fis.util.</span>base64 (data)](#apidoc.element.fis.util.base64)
1.  [function <span class="apidocSignatureSpan">fis.util.</span>camelcase (str)](#apidoc.element.fis.util.camelcase)
1.  [function <span class="apidocSignatureSpan">fis.util.</span>clone (source)](#apidoc.element.fis.util.clone)
1.  [function <span class="apidocSignatureSpan">fis.util.</span>copy (rSource, target, include, exclude, uncover, move)](#apidoc.element.fis.util.copy)
1.  [function <span class="apidocSignatureSpan">fis.util.</span>del (rPath, include, exclude)](#apidoc.element.fis.util.del)
1.  [function <span class="apidocSignatureSpan">fis.util.</span>download (url, callback, extract, opt)](#apidoc.element.fis.util.download)
1.  [function <span class="apidocSignatureSpan">fis.util.</span>escapeReg (str)](#apidoc.element.fis.util.escapeReg)
1.  [function <span class="apidocSignatureSpan">fis.util.</span>escapeShellArg (cmd)](#apidoc.element.fis.util.escapeShellArg)
1.  [function <span class="apidocSignatureSpan">fis.util.</span>escapeShellCmd (str)](#apidoc.element.fis.util.escapeShellCmd)
1.  [function <span class="apidocSignatureSpan">fis.util.</span>exists (path)](#apidoc.element.fis.util.exists)
1.  [function <span class="apidocSignatureSpan">fis.util.</span>ext (str)](#apidoc.element.fis.util.ext)
1.  [function <span class="apidocSignatureSpan">fis.util.</span>filter (str, include, exclude)](#apidoc.element.fis.util.filter)
1.  [function <span class="apidocSignatureSpan">fis.util.</span>find (rPath, include, exclude, root)](#apidoc.element.fis.util.find)
1.  [function <span class="apidocSignatureSpan">fis.util.</span>getMimeType (ext)](#apidoc.element.fis.util.getMimeType)
1.  [function <span class="apidocSignatureSpan">fis.util.</span>glob (pattern, str)](#apidoc.element.fis.util.glob)
1.  [function <span class="apidocSignatureSpan">fis.util.</span>install (name, version, opt)](#apidoc.element.fis.util.install)
1.  [function <span class="apidocSignatureSpan">fis.util.</span>is (source, type)](#apidoc.element.fis.util.is)
1.  [function <span class="apidocSignatureSpan">fis.util.</span>isAbsolute (path)](#apidoc.element.fis.util.isAbsolute)
1.  [function <span class="apidocSignatureSpan">fis.util.</span>isDir (path)](#apidoc.element.fis.util.isDir)
1.  [function <span class="apidocSignatureSpan">fis.util.</span>isEmpty (obj)](#apidoc.element.fis.util.isEmpty)
1.  [function <span class="apidocSignatureSpan">fis.util.</span>isFile (path)](#apidoc.element.fis.util.isFile)
1.  [function <span class="apidocSignatureSpan">fis.util.</span>isImageFile (path)](#apidoc.element.fis.util.isImageFile)
1.  [function <span class="apidocSignatureSpan">fis.util.</span>isTextFile (path)](#apidoc.element.fis.util.isTextFile)
1.  [function <span class="apidocSignatureSpan">fis.util.</span>isUtf8 (bytes)](#apidoc.element.fis.util.isUtf8)
1.  [function <span class="apidocSignatureSpan">fis.util.</span>isWin ()](#apidoc.element.fis.util.isWin)
1.  [function <span class="apidocSignatureSpan">fis.util.</span>map (obj, callback, merge)](#apidoc.element.fis.util.map)
1.  [function <span class="apidocSignatureSpan">fis.util.</span>md5 (data, len)](#apidoc.element.fis.util.md5)
1.  [function <span class="apidocSignatureSpan">fis.util.</span>merge (source, target)](#apidoc.element.fis.util.merge)
1.  [function <span class="apidocSignatureSpan">fis.util.</span>mkdir (path, mode)](#apidoc.element.fis.util.mkdir)
1.  [function <span class="apidocSignatureSpan">fis.util.</span>mtime (path)](#apidoc.element.fis.util.mtime)
1.  [function <span class="apidocSignatureSpan">fis.util.</span>nohup (cmd, options, callback)](#apidoc.element.fis.util.nohup)
1.  [function <span class="apidocSignatureSpan">fis.util.</span>normalize (path)](#apidoc.element.fis.util.normalize)
1.  [function <span class="apidocSignatureSpan">fis.util.</span>pad (str, len, fill, pre)](#apidoc.element.fis.util.pad)
1.  [function <span class="apidocSignatureSpan">fis.util.</span>parseUrl (url, opt)](#apidoc.element.fis.util.parseUrl)
1.  [function <span class="apidocSignatureSpan">fis.util.</span>pathinfo (path)](#apidoc.element.fis.util.pathinfo)
1.  [function <span class="apidocSignatureSpan">fis.util.</span>pipe (type, callback, def)](#apidoc.element.fis.util.pipe)
1.  [function <span class="apidocSignatureSpan">fis.util.</span>query (str)](#apidoc.element.fis.util.query)
1.  [function <span class="apidocSignatureSpan">fis.util.</span>read (path, convert)](#apidoc.element.fis.util.read)
1.  [function <span class="apidocSignatureSpan">fis.util.</span>readBuffer (buffer)](#apidoc.element.fis.util.readBuffer)
1.  [function <span class="apidocSignatureSpan">fis.util.</span>readJSON (path)](#apidoc.element.fis.util.readJSON)
1.  [function <span class="apidocSignatureSpan">fis.util.</span>realpath (path)](#apidoc.element.fis.util.realpath)
1.  [function <span class="apidocSignatureSpan">fis.util.</span>realpathSafe (path)](#apidoc.element.fis.util.realpathSafe)
1.  [function <span class="apidocSignatureSpan">fis.util.</span>stringQuote (str, quotes)](#apidoc.element.fis.util.stringQuote)
1.  [function <span class="apidocSignatureSpan">fis.util.</span>toEncoding (str, encoding)](#apidoc.element.fis.util.toEncoding)
1.  [function <span class="apidocSignatureSpan">fis.util.</span>touch (path, mtime)](#apidoc.element.fis.util.touch)
1.  [function <span class="apidocSignatureSpan">fis.util.</span>upload (url, opt, data, content, subpath, callback)](#apidoc.element.fis.util.upload)
1.  [function <span class="apidocSignatureSpan">fis.util.</span>write (path, data, charset, append)](#apidoc.element.fis.util.write)



# <a name="apidoc.module.fis"></a>[module fis](#apidoc.module.fis)

#### <a name="apidoc.element.fis.cache"></a>[function <span class="apidocSignatureSpan">fis.</span>cache ()](#apidoc.element.fis.cache)
- description and source-code
```javascript
cache = function (){
    return new F(arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fis.cache.Cache"></a>[function <span class="apidocSignatureSpan">fis.</span>cache.Cache ()](#apidoc.element.fis.cache.Cache)
- description and source-code
```javascript
cache.Cache = function (){
    parent.apply(this, arguments);
    constructor.apply(this, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fis.compile"></a>[function <span class="apidocSignatureSpan">fis.</span>compile (file)](#apidoc.element.fis.compile)
- description and source-code
```javascript
compile = function (file){
    if(!CACHE_DIR){
        fis.log.error('uninitialized compile cache directory.');
    }
    file = fis.file.wrap(file);
    if(!file.realpath){
        error('unable to compile [' + file.subpath + ']: Invalid file realpath.');
    }
    fis.log.debug('compile [' + file.realpath + '] start');
    fis.emitter.emit('compile:start', file);
    if(file.isFile()){
        if(file.useCompile && file.ext && file.ext !== '.'){
            var cache = file.cache = fis.cache(file.realpath, CACHE_DIR),
                revertObj = {};
            if(file.useCache && cache.revert(revertObj)){
                exports.settings.beforeCacheRevert(file);
                file.requires = revertObj.info.requires;
                file.extras = revertObj.info.extras;
                if(file.isText()){
                    revertObj.content = revertObj.content.toString('utf8');
                }
                file.setContent(revertObj.content);
                exports.settings.afterCacheRevert(file);
            } else {
                exports.settings.beforeCompile(file);
                file.setContent(fis.util.read(file.realpath));
                process(file);
                exports.settings.afterCompile(file);
                revertObj = {
                    requires : file.requires,
                    extras : file.extras
                };
                cache.save(file.getContent(), revertObj);
            }
        } else {
            file.setContent(file.isText() ? fis.util.read(file.realpath) : fis.util.fs.readFileSync(file.realpath));
        }
    } else if(file.useCompile && file.ext && file.ext !== '.'){
        process(file);
    }
    if(exports.settings.hash && file.useHash){
        file.getHash();
    }
    file.compiled = true;
    fis.log.debug('compile [' + file.realpath + '] end');
    fis.emitter.emit('compile:end', file);
    embeddedUnlock(file);
    return file;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fis.config.Config"></a>[function <span class="apidocSignatureSpan">fis.</span>config.Config ()](#apidoc.element.fis.config.Config)
- description and source-code
```javascript
config.Config = function (){
    parent.apply(this, arguments);
    constructor.apply(this, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fis.file"></a>[function <span class="apidocSignatureSpan">fis.</span>file ()](#apidoc.element.fis.file)
- description and source-code
```javascript
file = function (){
    return new F(arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fis.release"></a>[function <span class="apidocSignatureSpan">fis.</span>release (opt, callback)](#apidoc.element.fis.release)
- description and source-code
```javascript
release = function (opt, callback){
    if(typeof opt === 'function'){
        callback = opt;
        opt = {};
    } else {
        opt = opt || {};
    }

    var src = {};
    if (Array.isArray(opt.srcCache) && opt.srcCache.length) {
        opt.srcCache.forEach(function (path) {
            if (!fis.util.isFile(path)) return;
            var file = fis.file(path);
            if (file.release) {
                src[file.subpath] = file;
            }
        });
    } else {
        src = fis.project.getSource();
    }

    var ret = {
        src : src,
        ids : {},
        pkg : {},
        map : {
            res : {},
            pkg : {}
        }
    };
    opt.hash = opt.md5 > 0;
    fis.compile.setup(opt);
    fis.util.map(ret.src, function(subpath, file){
        if(opt.beforeEach) {
            opt.beforeEach(file, ret);
        }

        file = fis.compile(file);

        if(opt.afterEach) {
            opt.afterEach(file, ret);
        }

        if(file.release && file.useMap) {
            //add resource map
            var id = file.getId();
            ret.ids[id] = file;
            if(file.isJsLike){
                file.addSameNameRequire('.css');
            } else if(file.isHtmlLike){
                file.addSameNameRequire('.js');
                file.addSameNameRequire('.css');
            }
            var res = ret.map.res[id] = {
                uri  : file.getUrl(opt.hash, opt.domain),
                type : file.rExt.replace(/^\./, '')
            };
            for(var key in file.extras){
                if(file.extras.hasOwnProperty(key)){
                    res.extras = file.extras;
                    break;
                }
            }
            if(file.requires && file.requires.length){
                res.deps = file.requires;
            }
        }
    });

    //project root
    var root = fis.project.getProjectPath();

    var ns = fis.config.get('namespace');

    //get pack config
    var conf = fis.config.get('pack');
    if(typeof conf === 'undefined'){
        //from fis-pack.json
        var file = root + '/fis-pack.json';
        if(fis.util.isFile(file)){
            fis.config.set('pack', conf = fis.util.readJSON(file));
        }
    }

    //package callback
    var cb = function(packager, settings, key){
        fis.log.debug('[' + key + '] start');
        packager(ret, conf, settings, opt);
        fis.log.debug('[' + key + '] end');
    };

    //prepackage
    fis.util.pipe('prepackager', cb, opt.prepackager);

    //package
    if(opt.pack){
        //package
        fis.util.pipe('packager', cb, opt.packager);
        //css sprites
        fis.util.pipe('spriter', cb, opt.spriter);
    }

    //postpackage
    fis.util.pipe('postpackager', cb, opt.postpackager);

    //create map.json
    var map = fis.file(root, (ns ? ns + '-' : '') + 'map.json');
    if(map.release){
        map.setContent(JSON.stringify(ret.map, null, opt.optimize ? null : 4));
        ret.pkg[map.subpath] = map;
    }

    //done
    if(callback){
        callback(ret);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fis.require"></a>[function <span class="apidocSignatureSpan">fis.</span>require ()](#apidoc.element.fis.require)
- description and source-code
```javascript
require = function (){
    var path;
    var name = Array.prototype.slice.call(arguments, 0).join('-');
    if(fis.require._cache.hasOwnProperty(name)) return fis.require._cache[name];
    var names = [];
    for(var i = 0, len = fis.require.prefixes.length; i < len; i++){
        try {
            var pluginName = fis.require.prefixes[i] + '-' + name;
            names.push(pluginName);
            path = require.resolve(pluginName);
            try {
                return fis.require._cache[name] = require(pluginName);
            } catch (e){
                fis.log.error('load plugin [' + pluginName + '] error : ' + e.message);
            }
        } catch (e){
            if (e.code !== 'MODULE_NOT_FOUND') {
                throw e;
            }
        }
    }
    fis.log.error('unable to load plugin [' + names.join('] or [') + ']');
}
```
- example usage
```shell
...
    '  Usage: ' + fis.cli.name + ' <command>',
    '',
    '  Commands:',
    ''
];

fis.cli.help.commands.forEach(function(name){
    var cmd = fis.require('command', name);
    name = cmd.name || name;
    name = fis.util.pad(name, 12);
    content.push('    ' + name + (cmd.desc || ''));
});

content = content.concat([
    '',
...
```

#### <a name="apidoc.element.fis.time"></a>[function <span class="apidocSignatureSpan">fis.</span>time (title)](#apidoc.element.fis.time)
- description and source-code
```javascript
time = function (title){
    console.log(title + ' : ' + (Date.now() - last) + 'ms');
    last = Date.now();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fis.uri"></a>[function <span class="apidocSignatureSpan">fis.</span>uri (path, dirname)](#apidoc.element.fis.uri)
- description and source-code
```javascript
uri = function (path, dirname){
    var info = fis.util.stringQuote(path),
        qInfo = fis.util.query(info.rest);
    info.query = qInfo.query;
    info.hash = qInfo.hash;
    info.rest = qInfo.rest;
    if(info.rest){
        path = info.rest;
        if(path.indexOf(':') === -1){
            var file;
            if(path[0] === '/'){
                file = fis.project.getProjectPath(path);
            } else if(dirname) {
                file = fis.util(dirname, path);
            } else {
                fis.log.error('invalid dirname.');
            }

            var root = fis.project.getProjectPath();
            if(file && fis.util.isFile(file) && file.indexOf(root) === 0){
                info.file = fis.file(file);
            }
        }
    }
    return info;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fis.util"></a>[function <span class="apidocSignatureSpan">fis.</span>util (path)](#apidoc.element.fis.util)
- description and source-code
```javascript
util = function (path){
    var type = typeof path;
        if(arguments.length > 1) {
            path = Array.prototype.join.call(arguments, '/');
        } else if(type === 'string') {
            //do nothing for quickly determining.
        } else if(type === 'object') {
            path = Array.prototype.join.call(path, '/');
        } else if(type === 'undefined') {
            path = '';
        }
        if(path){
            path = pth.normalize(path.replace(/[\/\\]+/g, '/')).replace(/\\/g, '/');
            if(path !== '/'){
                path = path.replace(/\/$/, '');
            }
        }
        return path;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.fis.cache"></a>[module fis.cache](#apidoc.module.fis.cache)

#### <a name="apidoc.element.fis.cache.cache"></a>[function <span class="apidocSignatureSpan">fis.</span>cache ()](#apidoc.element.fis.cache.cache)
- description and source-code
```javascript
cache = function (){
    return new F(arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fis.cache.Cache"></a>[function <span class="apidocSignatureSpan">fis.cache.</span>Cache ()](#apidoc.element.fis.cache.Cache)
- description and source-code
```javascript
Cache = function (){
    parent.apply(this, arguments);
    constructor.apply(this, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fis.cache.clean"></a>[function <span class="apidocSignatureSpan">fis.cache.</span>clean (name)](#apidoc.element.fis.cache.clean)
- description and source-code
```javascript
clean = function (name){
    name = name || '';
    var path = fis.project.getCachePath(name);
    if(fis.util.exists(path)){
        fis.util.del(path);
    }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.fis.cache.Cache"></a>[module fis.cache.Cache](#apidoc.module.fis.cache.Cache)

#### <a name="apidoc.element.fis.cache.Cache.Cache"></a>[function <span class="apidocSignatureSpan">fis.cache.</span>Cache ()](#apidoc.element.fis.cache.Cache.Cache)
- description and source-code
```javascript
Cache = function (){
    parent.apply(this, arguments);
    constructor.apply(this, arguments);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.fis.cache.Cache.prototype"></a>[module fis.cache.Cache.prototype](#apidoc.module.fis.cache.Cache.prototype)

#### <a name="apidoc.element.fis.cache.Cache.prototype.addDeps"></a>[function <span class="apidocSignatureSpan">fis.cache.Cache.prototype.</span>addDeps (file)](#apidoc.element.fis.cache.Cache.prototype.addDeps)
- description and source-code
```javascript
addDeps = function (file){
    var path = fis.util.realpath(file);
    if(path){
        this.deps[path] = fis.util.mtime(path).getTime();
    } else {
        fis.log.warning('unable to add dependency file[' + file + ']: No such file.');
    }
    return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fis.cache.Cache.prototype.constructor"></a>[function <span class="apidocSignatureSpan">fis.cache.Cache.prototype.</span>constructor (path, dir)](#apidoc.element.fis.cache.Cache.prototype.constructor)
- description and source-code
```javascript
constructor = function (path, dir){
    var file = fis.util.realpath(path);
    if(!fis.util.isFile(file)){
        fis.log.error('unable to cache file[' + path + ']: No such file.');
    }
    this.timestamp = fis.util.mtime(file).getTime();
    this.deps = {};
    this.version = fis.version;

    var info = fis.util.pathinfo(file);
    var basename = fis.project.getCachePath(dir, info.basename);
    var hash = fis.util.md5(file, 10);
    this.cacheFile = basename + '-c-' + hash + '.tmp';
    this.cacheInfo = basename + '-o-' + hash + '.json';
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fis.cache.Cache.prototype.mergeDeps"></a>[function <span class="apidocSignatureSpan">fis.cache.Cache.prototype.</span>mergeDeps (cache)](#apidoc.element.fis.cache.Cache.prototype.mergeDeps)
- description and source-code
```javascript
mergeDeps = function (cache){
    var deps = {};
    if(cache instanceof Cache){
        deps = cache.deps
    } else if(typeof cache === 'object'){
        deps = cache
    } else {
        fis.log.error('unable to merge deps of data[' + cache + ']');
    }
    fis.util.map(deps, this.deps, true);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fis.cache.Cache.prototype.removeDeps"></a>[function <span class="apidocSignatureSpan">fis.cache.Cache.prototype.</span>removeDeps (file)](#apidoc.element.fis.cache.Cache.prototype.removeDeps)
- description and source-code
```javascript
removeDeps = function (file){
    var path = fis.util.realpath(file);
    if(path && this.deps[path]){
        delete this.deps[path];
    }
    return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fis.cache.Cache.prototype.revert"></a>[function <span class="apidocSignatureSpan">fis.cache.Cache.prototype.</span>revert (file)](#apidoc.element.fis.cache.Cache.prototype.revert)
- description and source-code
```javascript
revert = function (file){
    fis.log.debug('revert cache');
    if(
        exports.enable
        && fis.util.exists(this.cacheInfo)
        && fis.util.exists(this.cacheFile)
    ){
        fis.log.debug('cache file exists');
        var infos = fis.util.readJSON(this.cacheInfo);
        fis.log.debug('cache info read');
        if(infos.version == this.version && infos.timestamp == this.timestamp){
            var deps = infos['deps'];
            for(var f in deps){
                if(deps.hasOwnProperty(f)){
                    var d = fis.util.mtime(f);
                    if(d == 0 || deps[f] != d.getTime()){
                        fis.log.debug('cache is expired');
                        return false;
                    }
                }
            }
            this.deps = deps;
            fis.log.debug('cache is valid');
            if(file){
                file.info = infos.info;
                file.content = fis.util.fs.readFileSync(this.cacheFile);
            }
            fis.log.debug('revert cache finished');
            return true;
        }
    }
    fis.log.debug('cache is expired');
    return false;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fis.cache.Cache.prototype.save"></a>[function <span class="apidocSignatureSpan">fis.cache.Cache.prototype.</span>save (content, info)](#apidoc.element.fis.cache.Cache.prototype.save)
- description and source-code
```javascript
save = function (content, info){
    var infos = {
        version : this.version,
        timestamp : this.timestamp,
        deps : this.deps,
        info : info
    };
    fis.util.write(this.cacheInfo, JSON.stringify(infos));
    fis.util.write(this.cacheFile, content);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.fis.cli"></a>[module fis.cli](#apidoc.module.fis.cli)

#### <a name="apidoc.element.fis.cli.help"></a>[function <span class="apidocSignatureSpan">fis.cli.</span>help ()](#apidoc.element.fis.cli.help)
- description and source-code
```javascript
help = function (){
    var content = [
        '',
        '  Usage: ' + fis.cli.name + ' <command>',
        '',
        '  Commands:',
        ''
    ];

    fis.cli.help.commands.forEach(function(name){
        var cmd = fis.require('command', name);
        name = cmd.name || name;
        name = fis.util.pad(name, 12);
        content.push('    ' + name + (cmd.desc || ''));
    });

    content = content.concat([
        '',
        '  Options:',
        '',
        '    -h, --help     output usage information',
        '    -v, --version  output the version number',
        '    --no-color     disable colored output',
        ''
    ]);
    console.log(content.join('\n'));
}
```
- example usage
```shell
...

if(hasArgv(argv, '--no-color')){
    fis.cli.colors.mode = 'none';
}

var first = argv[2];
if(argv.length < 3 || first === '-h' ||  first === '--help'){
    fis.cli.help();
} else if(first === '-v' || first === '--version'){
    fis.cli.version();
} else if(first[0] === '-'){
    fis.cli.help();
} else {
    //register command
    var commander = fis.cli.commander = require('commander');
...
```

#### <a name="apidoc.element.fis.cli.run"></a>[function <span class="apidocSignatureSpan">fis.cli.</span>run (argv)](#apidoc.element.fis.cli.run)
- description and source-code
```javascript
run = function (argv){

    fis.processCWD = process.cwd();

    if(hasArgv(argv, '--no-color')){
        fis.cli.colors.mode = 'none';
    }

    var first = argv[2];
    if(argv.length < 3 || first === '-h' ||  first === '--help'){
        fis.cli.help();
    } else if(first === '-v' || first === '--version'){
        fis.cli.version();
    } else if(first[0] === '-'){
        fis.cli.help();
    } else {
        //register command
        var commander = fis.cli.commander = require('commander');
        var cmd = fis.require('command', argv[2]);
        cmd.register(
            commander
                .command(cmd.name || first)
                .usage(cmd.usage)
                .description(cmd.desc)
        );
        commander.parse(argv);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fis.cli.version"></a>[function <span class="apidocSignatureSpan">fis.cli.</span>version ()](#apidoc.element.fis.cli.version)
- description and source-code
```javascript
version = function (){
    var content = [
        '',
        '  v' + fis.cli.info.version,
        '',
        ' __' + '/\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\'.bold.red + '__' + '/\\\\\\\\\\\\\\\\\\\\\\'.bold.yellow + '_____' + '/\\\\\\\\\\\\\\\\\\\\\\'.bold.green + '___',
        '  _' + '\\/\\\\\\///////////'.bold.red + '__' + '\\/////\\\\\\///'.bold.yellow + '____' + '/\\\\\\/////////\\\\\\'.bold
.green + '_' + '       ',
        '   _' + '\\/\\\\\\'.bold.red + '_________________' + '\\/\\\\\\'.bold.yellow + '______' + '\\//\\\\\\'.bold.green + '______
' + '\\///'.bold.green + '__',
        '    _' + '\\/\\\\\\\\\\\\\\\\\\\\\\'.bold.red + '_________' + '\\/\\\\\\'.bold.yellow + '_______' + '\\////\\\\\\'.bold
.green + '_________' + '     ',
        '     _' + '\\/\\\\\\///////'.bold.red + '__________' + '\\/\\\\\\'.bold.yellow + '__________' + '\\////\\\\\\'.bold.green
 + '______' + '    ',
        '      _' + '\\/\\\\\\'.bold.red + '_________________' + '\\/\\\\\\'.bold.yellow + '_____________' + '\\////\\\\\\'.bold
.green + '___' + '   ',
        '       _' + '\\/\\\\\\'.bold.red + '_________________' + '\\/\\\\\\'.bold.yellow + '______' + '/\\\\\\'.bold.green + '______
' + '\\//\\\\\\'.bold.green + '__',
        '        _' + '\\/\\\\\\'.bold.red + '______________' + '/\\\\\\\\\\\\\\\\\\\\\\'.bold.yellow + '_' + '\\///\\\\\\\\\\\\\\\\\\\\\\/'.bold.green + '___',
        '         _' + '\\///'.bold.red + '______________' + '\\///////////'.bold.yellow + '____' + '\\///////////'.bold.green + '
_____',
        ''
    ].join('\n');
    console.log(content);
}
```
- example usage
```shell
...
    fis.cli.colors.mode = 'none';
}

var first = argv[2];
if(argv.length < 3 || first === '-h' ||  first === '--help'){
    fis.cli.help();
} else if(first === '-v' || first === '--version'){
    fis.cli.version();
} else if(first[0] === '-'){
    fis.cli.help();
} else {
    //register command
    var commander = fis.cli.commander = require('commander');
    var cmd = fis.require('command', argv[2]);
    cmd.register(
...
```



# <a name="apidoc.module.fis.cli.colors"></a>[module fis.cli.colors](#apidoc.module.fis.cli.colors)

#### <a name="apidoc.element.fis.cli.colors.addSequencer"></a>[function <span class="apidocSignatureSpan">fis.cli.colors.</span>addSequencer (name, map)](#apidoc.element.fis.cli.colors.addSequencer)
- description and source-code
```javascript
addSequencer = function (name, map) {
  addProperty(name, sequencer(map));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fis.cli.colors.black"></a>[function <span class="apidocSignatureSpan">fis.cli.colors.</span>black (str)](#apidoc.element.fis.cli.colors.black)
- description and source-code
```javascript
black = function (str) {
  return func.apply(str);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fis.cli.colors.blackBG"></a>[function <span class="apidocSignatureSpan">fis.cli.colors.</span>blackBG (str)](#apidoc.element.fis.cli.colors.blackBG)
- description and source-code
```javascript
blackBG = function (str) {
  return func.apply(str);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fis.cli.colors.blue"></a>[function <span class="apidocSignatureSpan">fis.cli.colors.</span>blue (str)](#apidoc.element.fis.cli.colors.blue)
- description and source-code
```javascript
blue = function (str) {
  return func.apply(str);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fis.cli.colors.blueBG"></a>[function <span class="apidocSignatureSpan">fis.cli.colors.</span>blueBG (str)](#apidoc.element.fis.cli.colors.blueBG)
- description and source-code
```javascript
blueBG = function (str) {
  return func.apply(str);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fis.cli.colors.bold"></a>[function <span class="apidocSignatureSpan">fis.cli.colors.</span>bold (str)](#apidoc.element.fis.cli.colors.bold)
- description and source-code
```javascript
bold = function (str) {
  return func.apply(str);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fis.cli.colors.cyan"></a>[function <span class="apidocSignatureSpan">fis.cli.colors.</span>cyan (str)](#apidoc.element.fis.cli.colors.cyan)
- description and source-code
```javascript
cyan = function (str) {
  return func.apply(str);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fis.cli.colors.cyanBG"></a>[function <span class="apidocSignatureSpan">fis.cli.colors.</span>cyanBG (str)](#apidoc.element.fis.cli.colors.cyanBG)
- description and source-code
```javascript
cyanBG = function (str) {
  return func.apply(str);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fis.cli.colors.green"></a>[function <span class="apidocSignatureSpan">fis.cli.colors.</span>green (str)](#apidoc.element.fis.cli.colors.green)
- description and source-code
```javascript
green = function (str) {
  return func.apply(str);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fis.cli.colors.greenBG"></a>[function <span class="apidocSignatureSpan">fis.cli.colors.</span>greenBG (str)](#apidoc.element.fis.cli.colors.greenBG)
- description and source-code
```javascript
greenBG = function (str) {
  return func.apply(str);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fis.cli.colors.grey"></a>[function <span class="apidocSignatureSpan">fis.cli.colors.</span>grey (str)](#apidoc.element.fis.cli.colors.grey)
- description and source-code
```javascript
grey = function (str) {
  return func.apply(str);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fis.cli.colors.greyBG"></a>[function <span class="apidocSignatureSpan">fis.cli.colors.</span>greyBG (str)](#apidoc.element.fis.cli.colors.greyBG)
- description and source-code
```javascript
greyBG = function (str) {
  return func.apply(str);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fis.cli.colors.inverse"></a>[function <span class="apidocSignatureSpan">fis.cli.colors.</span>inverse (str)](#apidoc.element.fis.cli.colors.inverse)
- description and source-code
```javascript
inverse = function (str) {
  return func.apply(str);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fis.cli.colors.italic"></a>[function <span class="apidocSignatureSpan">fis.cli.colors.</span>italic (str)](#apidoc.element.fis.cli.colors.italic)
- description and source-code
```javascript
italic = function (str) {
  return func.apply(str);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fis.cli.colors.magenta"></a>[function <span class="apidocSignatureSpan">fis.cli.colors.</span>magenta (str)](#apidoc.element.fis.cli.colors.magenta)
- description and source-code
```javascript
magenta = function (str) {
  return func.apply(str);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fis.cli.colors.magentaBG"></a>[function <span class="apidocSignatureSpan">fis.cli.colors.</span>magentaBG (str)](#apidoc.element.fis.cli.colors.magentaBG)
- description and source-code
```javascript
magentaBG = function (str) {
  return func.apply(str);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fis.cli.colors.rainbow"></a>[function <span class="apidocSignatureSpan">fis.cli.colors.</span>rainbow (str)](#apidoc.element.fis.cli.colors.rainbow)
- description and source-code
```javascript
rainbow = function (str) {
  return func.apply(str);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fis.cli.colors.red"></a>[function <span class="apidocSignatureSpan">fis.cli.colors.</span>red (str)](#apidoc.element.fis.cli.colors.red)
- description and source-code
```javascript
red = function (str) {
  return func.apply(str);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fis.cli.colors.redBG"></a>[function <span class="apidocSignatureSpan">fis.cli.colors.</span>redBG (str)](#apidoc.element.fis.cli.colors.redBG)
- description and source-code
```javascript
redBG = function (str) {
  return func.apply(str);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fis.cli.colors.setTheme"></a>[function <span class="apidocSignatureSpan">fis.cli.colors.</span>setTheme (theme)](#apidoc.element.fis.cli.colors.setTheme)
- description and source-code
```javascript
setTheme = function (theme) {
  if (typeof theme === 'string') {
    try {
      exports.themes[theme] = require(theme);
      applyTheme(exports.themes[theme]);
      return exports.themes[theme];
    } catch (err) {
      console.log(err);
      return err;
    }
  } else {
    applyTheme(theme);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fis.cli.colors.strikethrough"></a>[function <span class="apidocSignatureSpan">fis.cli.colors.</span>strikethrough (str)](#apidoc.element.fis.cli.colors.strikethrough)
- description and source-code
```javascript
strikethrough = function (str) {
  return func.apply(str);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fis.cli.colors.stripColors"></a>[function <span class="apidocSignatureSpan">fis.cli.colors.</span>stripColors (str)](#apidoc.element.fis.cli.colors.stripColors)
- description and source-code
```javascript
stripColors = function (str) {
  return func.apply(str);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fis.cli.colors.underline"></a>[function <span class="apidocSignatureSpan">fis.cli.colors.</span>underline (str)](#apidoc.element.fis.cli.colors.underline)
- description and source-code
```javascript
underline = function (str) {
  return func.apply(str);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fis.cli.colors.white"></a>[function <span class="apidocSignatureSpan">fis.cli.colors.</span>white (str)](#apidoc.element.fis.cli.colors.white)
- description and source-code
```javascript
white = function (str) {
  return func.apply(str);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fis.cli.colors.whiteBG"></a>[function <span class="apidocSignatureSpan">fis.cli.colors.</span>whiteBG (str)](#apidoc.element.fis.cli.colors.whiteBG)
- description and source-code
```javascript
whiteBG = function (str) {
  return func.apply(str);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fis.cli.colors.yellow"></a>[function <span class="apidocSignatureSpan">fis.cli.colors.</span>yellow (str)](#apidoc.element.fis.cli.colors.yellow)
- description and source-code
```javascript
yellow = function (str) {
  return func.apply(str);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fis.cli.colors.yellowBG"></a>[function <span class="apidocSignatureSpan">fis.cli.colors.</span>yellowBG (str)](#apidoc.element.fis.cli.colors.yellowBG)
- description and source-code
```javascript
yellowBG = function (str) {
  return func.apply(str);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fis.cli.colors.zalgo"></a>[function <span class="apidocSignatureSpan">fis.cli.colors.</span>zalgo (str)](#apidoc.element.fis.cli.colors.zalgo)
- description and source-code
```javascript
zalgo = function (str) {
  return func.apply(str);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fis.cli.colors.zebra"></a>[function <span class="apidocSignatureSpan">fis.cli.colors.</span>zebra (str)](#apidoc.element.fis.cli.colors.zebra)
- description and source-code
```javascript
zebra = function (str) {
  return func.apply(str);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.fis.compile"></a>[module fis.compile](#apidoc.module.fis.compile)

#### <a name="apidoc.element.fis.compile.compile"></a>[function <span class="apidocSignatureSpan">fis.</span>compile (file)](#apidoc.element.fis.compile.compile)
- description and source-code
```javascript
compile = function (file){
    if(!CACHE_DIR){
        fis.log.error('uninitialized compile cache directory.');
    }
    file = fis.file.wrap(file);
    if(!file.realpath){
        error('unable to compile [' + file.subpath + ']: Invalid file realpath.');
    }
    fis.log.debug('compile [' + file.realpath + '] start');
    fis.emitter.emit('compile:start', file);
    if(file.isFile()){
        if(file.useCompile && file.ext && file.ext !== '.'){
            var cache = file.cache = fis.cache(file.realpath, CACHE_DIR),
                revertObj = {};
            if(file.useCache && cache.revert(revertObj)){
                exports.settings.beforeCacheRevert(file);
                file.requires = revertObj.info.requires;
                file.extras = revertObj.info.extras;
                if(file.isText()){
                    revertObj.content = revertObj.content.toString('utf8');
                }
                file.setContent(revertObj.content);
                exports.settings.afterCacheRevert(file);
            } else {
                exports.settings.beforeCompile(file);
                file.setContent(fis.util.read(file.realpath));
                process(file);
                exports.settings.afterCompile(file);
                revertObj = {
                    requires : file.requires,
                    extras : file.extras
                };
                cache.save(file.getContent(), revertObj);
            }
        } else {
            file.setContent(file.isText() ? fis.util.read(file.realpath) : fis.util.fs.readFileSync(file.realpath));
        }
    } else if(file.useCompile && file.ext && file.ext !== '.'){
        process(file);
    }
    if(exports.settings.hash && file.useHash){
        file.getHash();
    }
    file.compiled = true;
    fis.log.debug('compile [' + file.realpath + '] end');
    fis.emitter.emit('compile:end', file);
    embeddedUnlock(file);
    return file;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fis.compile.analyseComment"></a>[function <span class="apidocSignatureSpan">fis.compile.</span>analyseComment (comment, callback)](#apidoc.element.fis.compile.analyseComment)
- description and source-code
```javascript
function analyseComment(comment, callback){
    var reg = /(@require\s+)('[^']+'|"[^"]+"|[^\s;!@#%^&*()]+)/g;
    callback = callback || function(m, prefix, value){
        return prefix + map.require.ld + value + map.require.rd;
    };
    return comment.replace(reg, callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fis.compile.clean"></a>[function <span class="apidocSignatureSpan">fis.compile.</span>clean (name)](#apidoc.element.fis.compile.clean)
- description and source-code
```javascript
clean = function (name){
    if(name){
        fis.cache.clean('compile/' + name);
    } else if(CACHE_DIR) {
        fis.cache.clean(CACHE_DIR);
    } else {
        fis.cache.clean('compile');
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fis.compile.extCss"></a>[function <span class="apidocSignatureSpan">fis.compile.</span>extCss (content, callback)](#apidoc.element.fis.compile.extCss)
- description and source-code
```javascript
function extCss(content, callback){
    var reg = /(\/\*[\s\S]*?(?:\*\/|$))|(?:@import\s+)?\burl\s*\(\s*("(?:[^\\"\r\n\f]|\\[\s\S])*"|'(?:[^\\'\n\r\f]|\\[\s\S])*'|[^)}\s]+)\s*\)(\s*;?)|\bsrc\s*=\s*("(?:[^\\"\r\n\f]|\\[\s\S])*"|'(?:[^\\'\n\r\f]|\\[\s\S])*'|[^\s}]+)/g;
    callback = callback || function(m, comment, url, last, filter){
        if(url){
            var key = isInline(fis.util.query(url)) ? 'embed' : 'uri';
            if(m.indexOf('@') === 0){
                if(key === 'embed'){
                    m = map.embed.ld + url + map.embed.rd + last.replace(/;$/, '');
                } else {
                    m = '@import url(' + map.uri.ld + url + map.uri.rd + ')' + last;
                }
            } else {
                m = 'url(' + map[key].ld + url + map[key].rd + ')' + last;
            }
        } else if(filter) {
            m = 'src=' + map.uri.ld + filter + map.uri.rd;
        } else if(comment) {
            m = analyseComment(comment);
        }
        return m;
    };
    return content.replace(reg, callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fis.compile.extHtml"></a>[function <span class="apidocSignatureSpan">fis.compile.</span>extHtml (content, callback)](#apidoc.element.fis.compile.extHtml)
- description and source-code
```javascript
function extHtml(content, callback){
    var reg = /(<script(?:(?=\s)[\s\S]*?["'\s\w\/\-]>|>))([\s\S]*?)(?=<\/script\s*>|$)|(<style(?:(?=\s)[\s\S]*?["'\s\w\/\-]>|>))([\s\S]*?)(?=<\/style\s*>|$)|<(img|embed|audio|video|link|object|source)\s+[\s\S]*?["'\s\w\/\-](?:>|$)|<!--inline\[([^\]]+)\]-->|<!--(?!\[)([\s\S]*?)(-->|$)/ig;
    callback = callback || function(m, $1, $2, $3, $4, $5, $6, $7, $8){
        if($1){//<script>
            var embed = '';
            $1 = $1.replace(/(\s(?:data-)?src\s*=\s*)('[^']+'|"[^"]+"|[^\s\/>]+)/ig, function(m, prefix, value){
                if(isInline(fis.util.query(value))){
                    embed += map.embed.ld + value + map.embed.rd;
                    return '';
                } else {
                    return prefix + map.uri.ld + value + map.uri.rd;
                }
            });
            if(embed){
                //embed file
                m = $1 + embed;
            } else if(!/\s+type\s*=/i.test($1) || /\s+type\s*=\s*(['"]?)text\/javascript\1/i.test($1)) {
                //without attrubite [type] or must be [text/javascript]
                m = $1 + extJs($2);
            } else {
                //other type as html
                m = $1 + extHtml($2);
            }
        } else if($3){//<style>
            m = $3 + extCss($4);
        } else if($5){//<img|embed|audio|video|link|object|source>
            var tag = $5.toLowerCase();
            if(tag === 'link'){
                var inline = '', isCssLink = false, isImportLink = false;
                var result = m.match(/\srel\s*=\s*('[^']+'|"[^"]+"|[^\s\/>]+)/i);
                if(result && result[1]){
                    var rel = result[1].replace(/^['"]|['"]$/g, '').toLowerCase();
                    isCssLink = rel === 'stylesheet';
                    isImportLink = rel === 'import';
                }
                m = m.replace(/(\s(?:data-)?href\s*=\s*)('[^']+'|"[^"]+"|[^\s\/>]+)/ig, function(_, prefix, value){
                    if((isCssLink || isImportLink) && isInline(fis.util.query(value))){
                        if(isCssLink) {
                            inline += '<style' + m.substring(5).replace(/\/(?=>$)/, '').replace(/\s+(?:charset|href|data-href|hreflang
|rel|rev|sizes|target)\s*=\s*(?:'[^']+'|"[^"]+"|[^\s\/>]+)/ig, '');
                        }
                        inline += map.embed.ld + value + map.embed.rd;
                        if(isCssLink) {
                            inline += '</style>';
                        }
                        return '';
                    } else {
                        return prefix + map.uri.ld + value + map.uri.rd;
                    }
                });
                m = inline || m;
            } else if(tag === 'object'){
                m = m.replace(/(\sdata\s*=\s*)('[^']+'|"[^"]+"|[^\s\/>]+)/ig, function(m, prefix, value){
                    return prefix + map.uri.ld + value + map.uri.rd;
                });
            } else {
                m = m.replace(/(\s(?:data-)?src\s*=\s*)('[^']+'|"[^"]+"|[^\s\/>]+)/ig, function(m, prefix, value){
                    var key = isInline(fis.util.query(value)) ? 'embed' : 'uri';
                    return prefix + map[key]['ld'] + value + map[key]['rd'];
                });
                if (tag == 'img') {
                    //<img src="image-src.png" srcset="image-1x.png 1x, image-2x.png 2x, image-3x.png 3x, image-4x.png 4x">
                    //http://www.webkit.org/demos/srcset/
                    m = m.replace(/(\ssrcset\s*=\s*)('[^']+'|"[^"]+"|[^\s\/>]+)/ig, function(m, prefix, value){
                        var info = fis.util.stringQuote(value);
                        var set = info.rest.split(',');
                        var imgset = [];
                        set.forEach(function (item) {
                            item = item.trim();
                            var p = item.indexOf(' ');
                            if (p == -1) {
                                imgset.push(item);
                                return;
                            } ...
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fis.compile.extJs"></a>[function <span class="apidocSignatureSpan">fis.compile.</span>extJs (content, callback)](#apidoc.element.fis.compile.extJs)
- description and source-code
```javascript
function extJs(content, callback){
    var reg = /"(?:[^\\"\r\n\f]|\\[\s\S])*"|'(?:[^\\'\n\r\f]|\\[\s\S])*'|(\/\/[^\r\n\f]+|\/\*[\s\S]*?(?:\*\/|$))|\b(__inline|__uri
|require)\s*\(\s*("(?:[^\\"\r\n\f]|\\[\s\S])*"|'(?:[^\\'\n\r\f]|\\[\s\S])*')\s*\)/g;
    callback = callback || function(m, comment, type, value){
        if(type){
            switch (type){
                case '__inline':
                    m = map.jsEmbed.ld + value + map.jsEmbed.rd;
                    break;
                case '__uri':
                    m = map.uri.ld + value + map.uri.rd;
                    break;
                case 'require':
                    m = 'require(' + map.require.ld + value + map.require.rd + ')';
                    break;
            }
        } else if(comment){
            m = analyseComment(comment);
        }
        return m;
    };
    return content.replace(reg, callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fis.compile.isInline"></a>[function <span class="apidocSignatureSpan">fis.compile.</span>isInline (info)](#apidoc.element.fis.compile.isInline)
- description and source-code
```javascript
function isInline(info){
    return /[?&]__inline(?:[=&'"]|$)/.test(info.query);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fis.compile.setup"></a>[function <span class="apidocSignatureSpan">fis.compile.</span>setup (opt)](#apidoc.element.fis.compile.setup)
- description and source-code
```javascript
setup = function (opt){
    var settings = exports.settings;
    if(opt){
        fis.util.map(settings, function(key){
            if(typeof opt[key] !== 'undefined'){
                settings[key] = opt[key];
            }
        });
    }
    CACHE_DIR = 'compile/';
    if(settings.unique){
        CACHE_DIR = 'compile_' + Date.now() + '-' + Math.random();
    } else {
        CACHE_DIR += ''
            + (settings.debug    ? 'debug'     : 'release')
            + (settings.optimize ? '-optimize' : '')
            + (settings.hash     ? '-hash'     : '')
            + (settings.domain   ? '-domain'   : '');
    }
    return CACHE_DIR;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.fis.compile.settings"></a>[module fis.compile.settings](#apidoc.module.fis.compile.settings)

#### <a name="apidoc.element.fis.compile.settings.afterCacheRevert"></a>[function <span class="apidocSignatureSpan">fis.compile.settings.</span>afterCacheRevert ()](#apidoc.element.fis.compile.settings.afterCacheRevert)
- description and source-code
```javascript
afterCacheRevert = function (){}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fis.compile.settings.afterCompile"></a>[function <span class="apidocSignatureSpan">fis.compile.settings.</span>afterCompile ()](#apidoc.element.fis.compile.settings.afterCompile)
- description and source-code
```javascript
afterCompile = function (){}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fis.compile.settings.beforeCacheRevert"></a>[function <span class="apidocSignatureSpan">fis.compile.settings.</span>beforeCacheRevert ()](#apidoc.element.fis.compile.settings.beforeCacheRevert)
- description and source-code
```javascript
beforeCacheRevert = function (){}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fis.compile.settings.beforeCompile"></a>[function <span class="apidocSignatureSpan">fis.compile.settings.</span>beforeCompile ()](#apidoc.element.fis.compile.settings.beforeCompile)
- description and source-code
```javascript
beforeCompile = function (){}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.fis.config"></a>[module fis.config](#apidoc.module.fis.config)

#### <a name="apidoc.element.fis.config.Config"></a>[function <span class="apidocSignatureSpan">fis.config.</span>Config ()](#apidoc.element.fis.config.Config)
- description and source-code
```javascript
Config = function (){
    parent.apply(this, arguments);
    constructor.apply(this, arguments);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.fis.config.Config"></a>[module fis.config.Config](#apidoc.module.fis.config.Config)

#### <a name="apidoc.element.fis.config.Config.Config"></a>[function <span class="apidocSignatureSpan">fis.config.</span>Config ()](#apidoc.element.fis.config.Config.Config)
- description and source-code
```javascript
Config = function (){
    parent.apply(this, arguments);
    constructor.apply(this, arguments);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.fis.config.Config.prototype"></a>[module fis.config.Config.prototype](#apidoc.module.fis.config.Config.prototype)

#### <a name="apidoc.element.fis.config.Config.prototype.constructor"></a>[function <span class="apidocSignatureSpan">fis.config.Config.prototype.</span>constructor ()](#apidoc.element.fis.config.Config.prototype.constructor)
- description and source-code
```javascript
constructor = function (){
    this.init.apply(this, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fis.config.Config.prototype.del"></a>[function <span class="apidocSignatureSpan">fis.config.Config.prototype.</span>del (path)](#apidoc.element.fis.config.Config.prototype.del)
- description and source-code
```javascript
del = function (path){
    path = String(path || '').trim();
    if(path){
        var paths = path.split('.'),
            data = this.data,
            last = paths.pop(), key;
        for(var i = 0, len = paths.length; i < len; i++){
            key = paths[i];
            if(typeof data[key] === 'object'){
                data = data[key];
            } else {
                return this;
            }
        }
        if(typeof data[last] !== 'undefined'){
            delete data[last];
        }
    }
    return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fis.config.Config.prototype.get"></a>[function <span class="apidocSignatureSpan">fis.config.Config.prototype.</span>get (path, def)](#apidoc.element.fis.config.Config.prototype.get)
- description and source-code
```javascript
get = function (path, def){
    var result = this.data || {};
    (path || '').split('.').forEach(function(key){
        if(key && (typeof result !== 'undefined')){
            result = result[key];
        }
    });
    if(typeof result === 'undefined'){
        return def;
    } else {
        return result;
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fis.config.Config.prototype.init"></a>[function <span class="apidocSignatureSpan">fis.config.Config.prototype.</span>init ()](#apidoc.element.fis.config.Config.prototype.init)
- description and source-code
```javascript
init = function (){
    this.data = {};
    if(arguments.length > 0){
        this.merge.apply(this, arguments);
    }
    return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fis.config.Config.prototype.merge"></a>[function <span class="apidocSignatureSpan">fis.config.Config.prototype.</span>merge ()](#apidoc.element.fis.config.Config.prototype.merge)
- description and source-code
```javascript
merge = function (){
    var self = this;
    [].slice.call(arguments).forEach(function(arg){
        if(typeof arg === 'object'){
            merge(self.data, arg);
        } else {
            fis.log.warning('unable to merge data[' + arg + '].');
        }
    });
    return this;
}
```
- example usage
```shell
...

'use strict';

//kernel
var fis = module.exports = require('fis-kernel');

//merge standard conf
fis.config.merge({
modules : {
    preprocessor: {
        js: 'components',
        css: 'components',
        html: 'components'
    },
    postprocessor : {
...
```

#### <a name="apidoc.element.fis.config.Config.prototype.require"></a>[function <span class="apidocSignatureSpan">fis.config.Config.prototype.</span>require (name)](#apidoc.element.fis.config.Config.prototype.require)
- description and source-code
```javascript
require = function (name){
    fis.require('config', name);
    return this;
}
```
- example usage
```shell
...
    '  Usage: ' + fis.cli.name + ' <command>',
    '',
    '  Commands:',
    ''
];

fis.cli.help.commands.forEach(function(name){
    var cmd = fis.require('command', name);
    name = cmd.name || name;
    name = fis.util.pad(name, 12);
    content.push('    ' + name + (cmd.desc || ''));
});

content = content.concat([
    '',
...
```

#### <a name="apidoc.element.fis.config.Config.prototype.set"></a>[function <span class="apidocSignatureSpan">fis.config.Config.prototype.</span>set (path, value)](#apidoc.element.fis.config.Config.prototype.set)
- description and source-code
```javascript
set = function (path, value){
    if(typeof value === 'undefined'){
        this.data = path;
    } else {
        path = String(path || '').trim();
        if(path){
            var paths = path.split('.'),
                last = paths.pop(),
                data = this.data || {};
            paths.forEach(function(key){
                var type = typeof data[key];
                if(type === 'object'){
                    data = data[key];
                } else if(type === 'undefined'){
                    data = data[key] = {};
                } else {
                    fis.log.error('forbidden to set property[' + key + '] of [' + type + '] data');
                }
            });
            data[last] = value;
        }
    }
    return this;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.fis.file"></a>[module fis.file](#apidoc.module.fis.file)

#### <a name="apidoc.element.fis.file.file"></a>[function <span class="apidocSignatureSpan">fis.</span>file ()](#apidoc.element.fis.file.file)
- description and source-code
```javascript
file = function (){
    return new F(arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fis.file.wrap"></a>[function <span class="apidocSignatureSpan">fis.file.</span>wrap (file)](#apidoc.element.fis.file.wrap)
- description and source-code
```javascript
wrap = function (file){
    if(typeof file === 'string'){
        return new File(file);
    } else if(file instanceof File){
        return file;
    } else {
        fis.log.error('unable to convert [' + (typeof file) + '] to [File] object.');
    }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.fis.log"></a>[module fis.log](#apidoc.module.fis.log)

#### <a name="apidoc.element.fis.log.debug"></a>[function <span class="apidocSignatureSpan">fis.log.</span>debug (msg)](#apidoc.element.fis.log.debug)
- description and source-code
```javascript
debug = function (msg){
    log('debug', exports.now() + ' ' + msg, exports.L_DEBUG);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fis.log.error"></a>[function <span class="apidocSignatureSpan">fis.log.</span>error (err)](#apidoc.element.fis.log.error)
- description and source-code
```javascript
error = function (err){
    if(!(err instanceof Error)){
        err = new Error(err.message || err);
    }
    if(exports.alert){
        err.message += '\u0007';
    }
    if(exports.throw){
        throw err
    } else {
        log('error', err.message, exports.L_ERROR);
        process.exit(1);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fis.log.notice"></a>[function <span class="apidocSignatureSpan">fis.log.</span>notice (msg)](#apidoc.element.fis.log.notice)
- description and source-code
```javascript
notice = function (msg){
    log('notice', msg, exports.L_NOTIC);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fis.log.now"></a>[function <span class="apidocSignatureSpan">fis.log.</span>now (withoutMilliseconds)](#apidoc.element.fis.log.now)
- description and source-code
```javascript
now = function (withoutMilliseconds){
    var d = new Date(), str;
    str = [
        d.getHours(),
        d.getMinutes(),
        d.getSeconds()
    ].join(':').replace(/\b\d\b/g, '0$&');
    if(!withoutMilliseconds){
        str += '.' + ('00' + d.getMilliseconds()).substr(-4);
    }
    return str;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fis.log.warning"></a>[function <span class="apidocSignatureSpan">fis.log.</span>warning (msg)](#apidoc.element.fis.log.warning)
- description and source-code
```javascript
warning = function (msg){
    log('warning', msg, exports.L_WARNI);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.fis.log.on"></a>[module fis.log.on](#apidoc.module.fis.log.on)

#### <a name="apidoc.element.fis.log.on.any"></a>[function <span class="apidocSignatureSpan">fis.log.on.</span>any (type, msg)](#apidoc.element.fis.log.on.any)
- description and source-code
```javascript
any = function (type, msg){}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fis.log.on.debug"></a>[function <span class="apidocSignatureSpan">fis.log.on.</span>debug (msg)](#apidoc.element.fis.log.on.debug)
- description and source-code
```javascript
debug = function (msg){ process.stdout.write('\n [DEBUG] ' + msg + '\n'); }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fis.log.on.error"></a>[function <span class="apidocSignatureSpan">fis.log.on.</span>error (msg)](#apidoc.element.fis.log.on.error)
- description and source-code
```javascript
error = function (msg){ process.stdout.write('\n [ERROR] ' + msg + '\n'); }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fis.log.on.notice"></a>[function <span class="apidocSignatureSpan">fis.log.on.</span>notice (msg)](#apidoc.element.fis.log.on.notice)
- description and source-code
```javascript
notice = function (msg){ process.stdout.write('\n [NOTIC] ' + msg + '\n'); }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fis.log.on.warning"></a>[function <span class="apidocSignatureSpan">fis.log.on.</span>warning (msg)](#apidoc.element.fis.log.on.warning)
- description and source-code
```javascript
warning = function (msg){ process.stdout.write('\n [WARNI] ' + msg + '\n'); }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.fis.project"></a>[module fis.project](#apidoc.module.fis.project)

#### <a name="apidoc.element.fis.project.getCachePath"></a>[function <span class="apidocSignatureSpan">fis.project.</span>getCachePath ()](#apidoc.element.fis.project.getCachePath)
- description and source-code
```javascript
getCachePath = function (){
    return getPath(exports.getTempPath('cache'), arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fis.project.getProjectPath"></a>[function <span class="apidocSignatureSpan">fis.project.</span>getProjectPath ()](#apidoc.element.fis.project.getProjectPath)
- description and source-code
```javascript
getProjectPath = function (){
    if(PROJECT_ROOT){
        return getPath(PROJECT_ROOT, arguments);
    } else {
        fis.log.error('undefined project root');
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fis.project.getSource"></a>[function <span class="apidocSignatureSpan">fis.project.</span>getSource ()](#apidoc.element.fis.project.getSource)
- description and source-code
```javascript
getSource = function (){
    var root = exports.getProjectPath(),
        source = {},
        project_exclude = /^(\/output\b|\/fis-[^\/]+)$/,
        include = fis.config.get('project.include'),
        exclude = fis.config.get('project.exclude');
    if (fis.util.is(exclude, 'Array')){
        project_exclude = [project_exclude].concat(exclude);
    }else if (exclude){
        project_exclude = [project_exclude, exclude];
    }
    fis.util.find(root, include, project_exclude, root).forEach(function(file){
        file = fis.file(file);
        if (file.release) {
            source[file.subpath] = file;
        }
    });
    return source;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fis.project.getTempPath"></a>[function <span class="apidocSignatureSpan">fis.project.</span>getTempPath ()](#apidoc.element.fis.project.getTempPath)
- description and source-code
```javascript
getTempPath = function (){
    if(!TEMP_ROOT){
        var list = ['FIS_TEMP_DIR', 'LOCALAPPDATA', 'APPDATA', 'HOME'];
        var name = fis.cli && fis.cli.name ? fis.cli.name : 'fis';
        var tmp;
        for(var i = 0, len = list.length; i < len; i++){
            if(tmp = process.env[list[i]]){
                break;
            }
        }
        tmp = tmp || __dirname + '/../';
        exports.setTempRoot(tmp + '/.' + name + '-tmp');
    }
    return getPath(TEMP_ROOT, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fis.project.setProjectRoot"></a>[function <span class="apidocSignatureSpan">fis.project.</span>setProjectRoot (path)](#apidoc.element.fis.project.setProjectRoot)
- description and source-code
```javascript
setProjectRoot = function (path){
    if(fis.util.isDir(path)){
        PROJECT_ROOT = fis.util.realpath(path);
    } else {
        fis.log.error('invalid project root path [' + path + ']');
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fis.project.setTempRoot"></a>[function <span class="apidocSignatureSpan">fis.project.</span>setTempRoot (tmp)](#apidoc.element.fis.project.setTempRoot)
- description and source-code
```javascript
setTempRoot = function (tmp){
    TEMP_ROOT = initDir(tmp);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.fis.uri"></a>[module fis.uri](#apidoc.module.fis.uri)

#### <a name="apidoc.element.fis.uri.uri"></a>[function <span class="apidocSignatureSpan">fis.</span>uri (path, dirname)](#apidoc.element.fis.uri.uri)
- description and source-code
```javascript
uri = function (path, dirname){
    var info = fis.util.stringQuote(path),
        qInfo = fis.util.query(info.rest);
    info.query = qInfo.query;
    info.hash = qInfo.hash;
    info.rest = qInfo.rest;
    if(info.rest){
        path = info.rest;
        if(path.indexOf(':') === -1){
            var file;
            if(path[0] === '/'){
                file = fis.project.getProjectPath(path);
            } else if(dirname) {
                file = fis.util(dirname, path);
            } else {
                fis.log.error('invalid dirname.');
            }

            var root = fis.project.getProjectPath();
            if(file && fis.util.isFile(file) && file.indexOf(root) === 0){
                info.file = fis.file(file);
            }
        }
    }
    return info;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fis.uri.getId"></a>[function <span class="apidocSignatureSpan">fis.uri.</span>getId (path, dirname)](#apidoc.element.fis.uri.getId)
- description and source-code
```javascript
getId = function (path, dirname){
    var info = uri(path, dirname);
    if(info.file){
        info.id = info.file.getId();
    } else {
        info.id = info.rest;
    }
    return info;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fis.uri.replaceDefine"></a>[function <span class="apidocSignatureSpan">fis.uri.</span>replaceDefine (value, escape)](#apidoc.element.fis.uri.replaceDefine)
- description and source-code
```javascript
function replaceDefine(value, escape){
    return value.replace(/\$\{([^\}]+)\}/g, function(all, $1){
        var val = fis.config.get($1);
        if(typeof val === 'undefined'){
            fis.log.error('undefined property [' + $1 + '].');
        } else {
            return escape ? fis.util.escapeReg(val) : val;
        }
        return all;
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fis.uri.replaceMatches"></a>[function <span class="apidocSignatureSpan">fis.uri.</span>replaceMatches (value, matches)](#apidoc.element.fis.uri.replaceMatches)
- description and source-code
```javascript
function replaceMatches(value, matches){
    return value.replace(/\$(\d+|&)/g, function(all, $1){
        var key = $1 === '&' ? '0' : $1;
        return matches.hasOwnProperty(key) ? (matches[key] || '') : all;
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fis.uri.replaceProperties"></a>[function <span class="apidocSignatureSpan">fis.uri.</span>replaceProperties (source, matches, target)](#apidoc.element.fis.uri.replaceProperties)
- description and source-code
```javascript
function replaceProperties(source, matches, target){
    var type = typeof source;
    if(type === 'object'){
        if(fis.util.is(source, 'Array')){
            target = target || [];
        } else {
            target = target || {};
        }
        fis.util.map(source, function(key, value){
            target[key] = replaceProperties(value, matches);
        });
        return target;
    } else if(type === 'string'){
        return replaceDefine(replaceMatches(source, matches));
// TODO support function type
//    } else if(type === 'function'){
//        return source(subpath || target.subpath, matches);
    } else {
        return source;
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fis.uri.roadmap"></a>[function <span class="apidocSignatureSpan">fis.uri.</span>roadmap (subpath, path, obj)](#apidoc.element.fis.uri.roadmap)
- description and source-code
```javascript
function roadmap(subpath, path, obj){
    var map = fis.config.get('roadmap.' + path, []);
    for(var i = 0, len = map.length; i < len; i++){
        var opt = map[i], reg = opt.reg;
        if(reg){
            if(typeof reg === 'string'){
                reg = fis.util.glob(replaceDefine(reg, true));
            } else if(!fis.util.is(reg, 'RegExp')){
                fis.log.error('invalid regexp [' + reg + '] of [roadmap.' + path + '.' + i + ']');
            }
            var matches = subpath.match(reg);
            if(matches){
                obj = obj || {};
                replaceProperties(opt, matches, obj);
                delete obj.reg;
                return obj;
            }
        } else {
            fis.log.error('[roadmap.' + path + '.' + i + '] missing property [reg].');
        }
    }
    return false;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.fis.util"></a>[module fis.util](#apidoc.module.fis.util)

#### <a name="apidoc.element.fis.util.util"></a>[function <span class="apidocSignatureSpan">fis.</span>util (path)](#apidoc.element.fis.util.util)
- description and source-code
```javascript
util = function (path){
    var type = typeof path;
        if(arguments.length > 1) {
            path = Array.prototype.join.call(arguments, '/');
        } else if(type === 'string') {
            //do nothing for quickly determining.
        } else if(type === 'object') {
            path = Array.prototype.join.call(path, '/');
        } else if(type === 'undefined') {
            path = '';
        }
        if(path){
            path = pth.normalize(path.replace(/[\/\\]+/g, '/')).replace(/\\/g, '/');
            if(path !== '/'){
                path = path.replace(/\/$/, '');
            }
        }
        return path;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fis.util.base64"></a>[function <span class="apidocSignatureSpan">fis.util.</span>base64 (data)](#apidoc.element.fis.util.base64)
- description and source-code
```javascript
base64 = function (data){
    if(data instanceof Buffer){
        //do nothing for quickly determining.
    } else if(data instanceof Array){
        data = new Buffer(data);
    } else {
        //convert to string.
        data = new Buffer(String(data || ''));
    }
    return data.toString('base64');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fis.util.camelcase"></a>[function <span class="apidocSignatureSpan">fis.util.</span>camelcase (str)](#apidoc.element.fis.util.camelcase)
- description and source-code
```javascript
camelcase = function (str){
    var ret = '';
    if(str){
        str.split(/[-_ ]+/).forEach(function(ele){
            ret += ele[0].toUpperCase() + ele.substring(1);
        });
    } else {
        ret = str;
    }
    return ret;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fis.util.clone"></a>[function <span class="apidocSignatureSpan">fis.util.</span>clone (source)](#apidoc.element.fis.util.clone)
- description and source-code
```javascript
clone = function (source) {
    var ret;
    switch(toString.call(source)){
        case '[object Object]':
            ret = {};
            _.map(source, function(k, v){
                ret[k] = _.clone(v);
            });
            break;
        case '[object Array]':
            ret = [];
            source.forEach(function(ele){
                ret.push(_.clone(ele));
            });
            break;
        default :
            ret = source;
    }
    return ret;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fis.util.copy"></a>[function <span class="apidocSignatureSpan">fis.util.</span>copy (rSource, target, include, exclude, uncover, move)](#apidoc.element.fis.util.copy)
- description and source-code
```javascript
copy = function (rSource, target, include, exclude, uncover, move){
    var removedAll = true,
        source = _.realpath(rSource);
    target = _(target);
    if(source){
        var stat = fs.statSync(source);
        if(stat.isDirectory()){
            fs.readdirSync(source).forEach(function(name){
                if(name != '.' && name != '..') {
                    removedAll = _.copy(
                        source + '/' + name,
                        target + '/' + name,
                        include, exclude,
                        uncover, move
                    ) && removedAll;
                }
            });
            if(move && removedAll) {
                fs.rmdirSync(source);
            }
        } else if(stat.isFile() && _.filter(source, include, exclude)){
            if(uncover && _exists(target)){
                //uncover
                removedAll = false;
            } else {
                _.write(target, fs.readFileSync(source, null));
                if(move) {
                    fs.unlinkSync(source);
                }
            }
        } else {
            removedAll = false;
        }
    } else {
        fis.log.error('unable to copy [' + rSource + ']: No such file or directory.');
    }
    return removedAll;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fis.util.del"></a>[function <span class="apidocSignatureSpan">fis.util.</span>del (rPath, include, exclude)](#apidoc.element.fis.util.del)
- description and source-code
```javascript
del = function (rPath, include, exclude){
    var removedAll = true;
    var path;
    if(rPath && _.exists(rPath)) {
        var stat = fs.lstatSync(rPath);
        var isFile = stat.isFile() || stat.isSymbolicLink();

        if (stat.isSymbolicLink()) {
            path = rPath;
        } else {
            path = _.realpath(rPath);
        }

        if(/^(?:\w:)?\/$/.test(path)){
            fis.log.error('unable to delete directory [' + rPath + '].');
        }

        if(stat.isDirectory()){
            fs.readdirSync(path).forEach(function(name){
                if(name != '.' && name != '..') {
                    removedAll = _.del(path + '/' + name, include, exclude) && removedAll;
                }
            });
            if(removedAll) {
                fs.rmdirSync(path);
            }
        } else if(isFile && _.filter(path, include, exclude)) {
            fs.unlinkSync(path);
        } else {
            removedAll = false;
        }
    } else {
        //fis.log.error('unable to delete [' + rPath + ']: No such file or directory.');
    }
    return removedAll;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fis.util.download"></a>[function <span class="apidocSignatureSpan">fis.util.</span>download (url, callback, extract, opt)](#apidoc.element.fis.util.download)
- description and source-code
```javascript
download = function (url, callback, extract, opt){
    opt  = _.parseUrl(url, opt || {});
    var http = opt.protocol === 'https:' ? require('https') : require('http'),
        name = _.md5(url, 8) + _.ext(url).ext,
        tmp  = fis.project.getTempPath('downloads', name),
        data = opt.data;
    delete opt.data;
    _.write(tmp, '');
    var writer = fs.createWriteStream(tmp),
        http_err_handler = function(err){
            writer.destroy();
            fs.unlinkSync(tmp);
            var msg = typeof err === 'object' ? err.message : err;
            if(callback){
                callback(msg);
            } else {
                fis.log.error('request error [' + msg + ']');
            }
        },
        req = http.request(opt, function(res){
            var status = res.statusCode;
            res
                .on('data', function(chunk){
                    writer.write(chunk);
                })
                .on('end', function(){
                    if(status >= 200 && status < 300 || status === 304){
                        if(extract){
                            fs
                                .createReadStream(tmp)
                                .pipe(getTar().Extract({ path : extract }))
                                .on('error', function(err){
                                    if(callback){
                                        callback(err);
                                    } else {
                                        fis.log.error('extract tar file [' + tmp + '] fail, error [' + err + ']');
                                    }
                                })
                                .on('end', function(){
                                    if(callback && (typeof callback(null, tmp, res) === 'undefined')){
                                        fs.unlinkSync(tmp);
                                    }
                                });
                        } else if(callback && (typeof callback(null, tmp, res) === 'undefined')){
                            fs.unlinkSync(tmp);
                        }
                    } else {
                        http_err_handler(status);
                    }
                })
                .on('error', http_err_handler);
        });
    req.on('error', http_err_handler);
    if(data){
        req.write(data);
    }
    req.end();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fis.util.escapeReg"></a>[function <span class="apidocSignatureSpan">fis.util.</span>escapeReg (str)](#apidoc.element.fis.util.escapeReg)
- description and source-code
```javascript
escapeReg = function (str){
    return str.replace(/[\.\\\+\*\?\[\^\]\$\(\){}=!<>\|:\/]/g, '\\$&');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fis.util.escapeShellArg"></a>[function <span class="apidocSignatureSpan">fis.util.</span>escapeShellArg (cmd)](#apidoc.element.fis.util.escapeShellArg)
- description and source-code
```javascript
escapeShellArg = function (cmd){
    return '"' + cmd + '"';
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fis.util.escapeShellCmd"></a>[function <span class="apidocSignatureSpan">fis.util.</span>escapeShellCmd (str)](#apidoc.element.fis.util.escapeShellCmd)
- description and source-code
```javascript
escapeShellCmd = function (str){
    return str.replace(/ /g, '"$&"');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fis.util.exists"></a>[function <span class="apidocSignatureSpan">fis.util.</span>exists (path)](#apidoc.element.fis.util.exists)
- description and source-code
```javascript
exists = function (path) {
  try {
    nullCheck(path);
    binding.stat(pathModule._makeLong(path), statValues);
    return true;
  } catch (e) {
    return false;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fis.util.ext"></a>[function <span class="apidocSignatureSpan">fis.util.</span>ext (str)](#apidoc.element.fis.util.ext)
- description and source-code
```javascript
ext = function (str){
    var info = _.query(str), pos;
    str = info.fullname = info.rest;
    if((pos = str.lastIndexOf('/')) > -1){
        if(pos === 0){
            info.rest = info.dirname = '/';
        } else {
            info.dirname = str.substring(0, pos);
            info.rest = info.dirname + '/';
        }
        str = str.substring(pos + 1);
    } else {
        info.rest = info.dirname = '';
    }
    if((pos = str.lastIndexOf('.')) > -1){
        info.ext = str.substring(pos).toLowerCase();
        info.filename = str.substring(0, pos);
        info.basename = info.filename + info.ext;
    } else {
        info.basename = info.filename = str;
        info.ext = '';
    }
    info.rest += info.filename;
    return info;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fis.util.filter"></a>[function <span class="apidocSignatureSpan">fis.util.</span>filter (str, include, exclude)](#apidoc.element.fis.util.filter)
- description and source-code
```javascript
filter = function (str, include, exclude){

    function normalize(pattern){
        var type = toString.call(pattern);
        switch (type){
            case '[object String]':
                return _.glob(pattern);
            case '[object RegExp]':
                return pattern;
            default:
                fis.log.error('invalid regexp [' + pattern + '].');
        }
    }

    function match(str, patterns){
        var matched = false;
        if (!_.is(patterns, 'Array')){
            patterns = [patterns];
        }
        patterns.every(function(pattern){
            if (!pattern){
                return true;
            }
            matched = matched || str.search(normalize(pattern)) > -1;
            return !matched;
        });
        return matched;
    }

    var isInclude, isExclude;

    if (include) {
        isInclude = match(str, include);
    }else{
        isInclude = true;
    }

    if (exclude) {
        isExclude = match(str, exclude);
    }

    return isInclude && !isExclude;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fis.util.find"></a>[function <span class="apidocSignatureSpan">fis.util.</span>find (rPath, include, exclude, root)](#apidoc.element.fis.util.find)
- description and source-code
```javascript
find = function (rPath, include, exclude, root){
    var list = [],
        path = _.realpath(rPath),
        filterPath = root ? path.substring(root.length) : path;
    if(path){
        var stat = fs.statSync(path);
        if(stat.isDirectory() && (include || _.filter(filterPath, include, exclude))){
            fs.readdirSync(path).forEach(function(p){
                if(p[0] != '.') {
                    list = list.concat(_.find(path + '/' + p, include, exclude, root));
                }
            });
        } else if(stat.isFile() && _.filter(filterPath, include, exclude)) {
            list.push(path);
        }
    } else {
        fis.log.error('unable to find [' + rPath + ']: No such file or directory.');
    }
    return list.sort();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fis.util.getMimeType"></a>[function <span class="apidocSignatureSpan">fis.util.</span>getMimeType (ext)](#apidoc.element.fis.util.getMimeType)
- description and source-code
```javascript
getMimeType = function (ext){
    if(ext[0] === '.'){
        ext = ext.substring(1);
    }
    return MIME_MAP[ext] || 'application/x-' + ext;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fis.util.glob"></a>[function <span class="apidocSignatureSpan">fis.util.</span>glob (pattern, str)](#apidoc.element.fis.util.glob)
- description and source-code
```javascript
glob = function (pattern, str){
    var sep = _.escapeReg('/');
    pattern = new RegExp('^' + sep + '?' +
        _.escapeReg(
                pattern
                    .replace(/\\/g, '/')
                    .replace(/^\//, '')
            )
            .replace(new RegExp(sep + '\\*\\*' + sep, 'g'), sep + '.*(?:' + sep + ')?')
            .replace(new RegExp(sep + '\\*\\*', 'g'), sep + '.*')
            .replace(/\\\*\\\*/g, '.*')
            .replace(/\\\*/g, '[^' + sep + ']*')
            .replace(/\\\?/g, '[^' + sep + ']') + '$',
        'i'
    );
    if(typeof str === 'string'){
        return pattern.test(str);
    } else {
        return pattern;
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fis.util.install"></a>[function <span class="apidocSignatureSpan">fis.util.</span>install (name, version, opt)](#apidoc.element.fis.util.install)
- description and source-code
```javascript
install = function (name, version, opt){
    version = version === '*' ? 'latest' : ( version || 'latest' );
    var remote = opt.remote.replace(/^\/$/, '');
    var url = remote + '/' + name + '/' + version + '.tar';
    var extract = opt.extract || process.cwd();
    if(opt.before){
        opt.before(name, version);
    }
    _.download(url, function(err){
        if(err){
            if(opt.error){
                opt.error(err);
            } else {
                fis.log.error( 'unable to download component [' +
                    name + '@' + version + '] from [' + url + '], error [' + err + ']');
            }
        } else {
            if(opt.done){
                opt.done(name, version);
            }
            process.stdout.write('install [' + name + '@' + version + ']\n');
            var pkg = _(extract, 'package.json');
            if(_.isFile(pkg)){
                var info = _.readJSON(pkg);
                fs.unlinkSync(pkg);
                _.map(info.dependencies || {}, function(depName, depVersion){
                    _.install(depName, depVersion, opt);
                });
            }
        }
    }, extract);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fis.util.is"></a>[function <span class="apidocSignatureSpan">fis.util.</span>is (source, type)](#apidoc.element.fis.util.is)
- description and source-code
```javascript
is = function (source, type){
    return toString.call(source) === '[object ' + type + ']';
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fis.util.isAbsolute"></a>[function <span class="apidocSignatureSpan">fis.util.</span>isAbsolute (path)](#apidoc.element.fis.util.isAbsolute)
- description and source-code
```javascript
isAbsolute = function (path) {
    if (IS_WIN) {
        return /^[a-z]:/i.test(path);
    } else {
        if(path === '/'){
            return true;
        } else {
            var split = path.split('/');
            if(split[0] === '~'){
                return true;
            } else if(split[0] === '' && split[1]) {
                return _.isDir('/' + split[1] + '/' + split[2]);
            } else {
                return false;
            }
        }
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fis.util.isDir"></a>[function <span class="apidocSignatureSpan">fis.util.</span>isDir (path)](#apidoc.element.fis.util.isDir)
- description and source-code
```javascript
isDir = function (path){
    return _exists(path) && fs.statSync(path).isDirectory();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fis.util.isEmpty"></a>[function <span class="apidocSignatureSpan">fis.util.</span>isEmpty (obj)](#apidoc.element.fis.util.isEmpty)
- description and source-code
```javascript
isEmpty = function (obj) {
    if (obj === null) return true;
    if (_.is(obj, 'Array')) return obj.length == 0;
    for (var key in obj) {
        if (obj.hasOwnProperty(key)) {
            return false;
        }
    }
    return true
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fis.util.isFile"></a>[function <span class="apidocSignatureSpan">fis.util.</span>isFile (path)](#apidoc.element.fis.util.isFile)
- description and source-code
```javascript
isFile = function (path){
    return _exists(path) && fs.statSync(path).isFile();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fis.util.isImageFile"></a>[function <span class="apidocSignatureSpan">fis.util.</span>isImageFile (path)](#apidoc.element.fis.util.isImageFile)
- description and source-code
```javascript
isImageFile = function (path){
    return getFileTypeReg('image').test(path || '');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fis.util.isTextFile"></a>[function <span class="apidocSignatureSpan">fis.util.</span>isTextFile (path)](#apidoc.element.fis.util.isTextFile)
- description and source-code
```javascript
isTextFile = function (path){
    return getFileTypeReg('text').test(path || '');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fis.util.isUtf8"></a>[function <span class="apidocSignatureSpan">fis.util.</span>isUtf8 (bytes)](#apidoc.element.fis.util.isUtf8)
- description and source-code
```javascript
isUtf8 = function (bytes) {
    var i = 0;
    while(i < bytes.length) {
        if((// ASCII
            0x00 <= bytes[i] && bytes[i] <= 0x7F
        )) {
            i += 1;
            continue;
        }

        if((// non-overlong 2-byte
            (0xC2 <= bytes[i] && bytes[i] <= 0xDF) &&
            (0x80 <= bytes[i+1] && bytes[i+1] <= 0xBF)
        )) {
            i += 2;
            continue;
        }

        if(
            (// excluding overlongs
                bytes[i] == 0xE0 &&
                (0xA0 <= bytes[i + 1] && bytes[i + 1] <= 0xBF) &&
                (0x80 <= bytes[i + 2] && bytes[i + 2] <= 0xBF)
            ) || (// straight 3-byte
                ((0xE1 <= bytes[i] && bytes[i] <= 0xEC) ||
                bytes[i] == 0xEE ||
                bytes[i] == 0xEF) &&
                (0x80 <= bytes[i + 1] && bytes[i + 1] <= 0xBF) &&
                (0x80 <= bytes[i + 2] && bytes[i + 2] <= 0xBF)
            ) || (// excluding surrogates
                bytes[i] == 0xED &&
                (0x80 <= bytes[i + 1] && bytes[i + 1] <= 0x9F) &&
                (0x80 <= bytes[i + 2] && bytes[i + 2] <= 0xBF)
            )
        ) {
            i += 3;
            continue;
        }

        if(
            (// planes 1-3
                bytes[i] == 0xF0 &&
                (0x90 <= bytes[i + 1] && bytes[i + 1] <= 0xBF) &&
                (0x80 <= bytes[i + 2] && bytes[i + 2] <= 0xBF) &&
                (0x80 <= bytes[i + 3] && bytes[i + 3] <= 0xBF)
            ) || (// planes 4-15
                (0xF1 <= bytes[i] && bytes[i] <= 0xF3) &&
                (0x80 <= bytes[i + 1] && bytes[i + 1] <= 0xBF) &&
                (0x80 <= bytes[i + 2] && bytes[i + 2] <= 0xBF) &&
                (0x80 <= bytes[i + 3] && bytes[i + 3] <= 0xBF)
            ) || (// plane 16
                bytes[i] == 0xF4 &&
                (0x80 <= bytes[i + 1] && bytes[i + 1] <= 0x8F) &&
                (0x80 <= bytes[i + 2] && bytes[i + 2] <= 0xBF) &&
                (0x80 <= bytes[i + 3] && bytes[i + 3] <= 0xBF)
            )
        ) {
            i += 4;
            continue;
        }
        return false;
    }
    return true;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fis.util.isWin"></a>[function <span class="apidocSignatureSpan">fis.util.</span>isWin ()](#apidoc.element.fis.util.isWin)
- description and source-code
```javascript
isWin = function (){
    return IS_WIN;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fis.util.map"></a>[function <span class="apidocSignatureSpan">fis.util.</span>map (obj, callback, merge)](#apidoc.element.fis.util.map)
- description and source-code
```javascript
map = function (obj, callback, merge){
    var index = 0;
    for(var key in obj){
        if(obj.hasOwnProperty(key)){
            if(merge){
                callback[key] = obj[key];
            } else if(callback(key, obj[key], index++)) {
                break;
            }
        }
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fis.util.md5"></a>[function <span class="apidocSignatureSpan">fis.util.</span>md5 (data, len)](#apidoc.element.fis.util.md5)
- description and source-code
```javascript
md5 = function (data, len){
    var md5sum = crypto.createHash('md5'),
        encoding = typeof data === 'string' ? 'utf8' : 'binary';
    md5sum.update(data, encoding);
    len = len || fis.config.get('project.md5Length', 7);
    return md5sum.digest('hex').substring(0, len);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fis.util.merge"></a>[function <span class="apidocSignatureSpan">fis.util.</span>merge (source, target)](#apidoc.element.fis.util.merge)
- description and source-code
```javascript
merge = function (source, target){
    if(_.is(source, 'Object') && _.is(target, 'Object')){
        _.map(target, function(key, value){
            source[key] = _.merge(source[key], value);
        });
    } else {
        source = target;
    }
    return source;
}
```
- example usage
```shell
...

'use strict';

//kernel
var fis = module.exports = require('fis-kernel');

//merge standard conf
fis.config.merge({
modules : {
    preprocessor: {
        js: 'components',
        css: 'components',
        html: 'components'
    },
    postprocessor : {
...
```

#### <a name="apidoc.element.fis.util.mkdir"></a>[function <span class="apidocSignatureSpan">fis.util.</span>mkdir (path, mode)](#apidoc.element.fis.util.mkdir)
- description and source-code
```javascript
mkdir = function (path, mode){
    if (typeof mode === 'undefined') {
        //511 === 0777
        mode = 511 & (~process.umask());
    }
    if(_exists(path)) return;
    path.split('/').reduce(function(prev, next) {
        if(prev && !_exists(prev)) {
            fs.mkdirSync(prev, mode);
        }
        return prev + '/' + next;
    });
    if(!_exists(path)) {
        fs.mkdirSync(path, mode);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fis.util.mtime"></a>[function <span class="apidocSignatureSpan">fis.util.</span>mtime (path)](#apidoc.element.fis.util.mtime)
- description and source-code
```javascript
mtime = function (path){
    var time = 0;
    if(_exists(path)){
        time = fs.statSync(path).mtime;
    }
    return time;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fis.util.nohup"></a>[function <span class="apidocSignatureSpan">fis.util.</span>nohup (cmd, options, callback)](#apidoc.element.fis.util.nohup)
- description and source-code
```javascript
nohup = function (cmd, options, callback){
    if(typeof options === 'function'){
        callback = options;
        options = null;
    }
    var exec = require('child_process').exec;
    if(IS_WIN){
        var cmdEscape = cmd.replace(/"/g, '""'),
            file = fis.project.getTempPath('nohup-' + _.md5(cmd) + '.vbs'),
            script = '';
        script += 'Dim shell\n';
        script += 'Set shell = Wscript.CreateObject("WScript.Shell")\n';
        script += 'ret = shell.Run("cmd.exe /c start /b ' + cmdEscape + '", 0, TRUE)\n';
        script += 'WScript.StdOut.Write(ret)\n';
        script += 'Set shell = NoThing';
        _.write(file, script);
        return exec('cscript.exe /nologo "' + file + '"', options, function(error, stdout){
            if(stdout != '0'){
                fis.log.error('exec command[' + cmd + '] fail.');
            }
            fs.unlinkSync(file);
            if(typeof callback === 'function') {
                callback();
            }
        });
    } else {
        return exec('nohup ' + cmd + ' > /dev/null 2>&1 &', options, function(error, stdout){
            if(error !== null) {
                fis.log.error('exec command[' + cmd + '] fail, stdout [' + stdout + '].');
            }
            if(typeof callback === 'function') {
                callback();
            }
        });
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fis.util.normalize"></a>[function <span class="apidocSignatureSpan">fis.util.</span>normalize (path)](#apidoc.element.fis.util.normalize)
- description and source-code
```javascript
normalize = function (path){
    var type = typeof path;
        if(arguments.length > 1) {
            path = Array.prototype.join.call(arguments, '/');
        } else if(type === 'string') {
            //do nothing for quickly determining.
        } else if(type === 'object') {
            path = Array.prototype.join.call(path, '/');
        } else if(type === 'undefined') {
            path = '';
        }
        if(path){
            path = pth.normalize(path.replace(/[\/\\]+/g, '/')).replace(/\\/g, '/');
            if(path !== '/'){
                path = path.replace(/\/$/, '');
            }
        }
        return path;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fis.util.pad"></a>[function <span class="apidocSignatureSpan">fis.util.</span>pad (str, len, fill, pre)](#apidoc.element.fis.util.pad)
- description and source-code
```javascript
pad = function (str, len, fill, pre){
    if(str.length < len){
        fill = (new Array(len)).join(fill || ' ');
        if(pre){
            str = (fill + str).substr(-len);
        } else {
            str = (str + fill).substring(0, len);
        }
    }
    return str;
}
```
- example usage
```shell
...
    '  Commands:',
    ''
];

fis.cli.help.commands.forEach(function(name){
    var cmd = fis.require('command', name);
    name = cmd.name || name;
    name = fis.util.pad(name, 12);
    content.push('    ' + name + (cmd.desc || ''));
});

content = content.concat([
    '',
    '  Options:',
    '',
...
```

#### <a name="apidoc.element.fis.util.parseUrl"></a>[function <span class="apidocSignatureSpan">fis.util.</span>parseUrl (url, opt)](#apidoc.element.fis.util.parseUrl)
- description and source-code
```javascript
parseUrl = function (url, opt){
    opt = opt || {};
    url = Url.parse(url);
    var ssl = url.protocol === 'https:';
    opt.host = opt.host
        || opt.hostname
        || ((ssl || url.protocol === 'http:') ? url.hostname : 'localhost');
    opt.port = opt.port || (url.port || (ssl ? 443 : 80));
    opt.path = opt.path || (url.pathname + (url.search ? url.search : ''));
    opt.method = opt.method || 'GET';
    opt.agent = opt.agent || false;
    return opt;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fis.util.pathinfo"></a>[function <span class="apidocSignatureSpan">fis.util.</span>pathinfo (path)](#apidoc.element.fis.util.pathinfo)
- description and source-code
```javascript
pathinfo = function (path){
    //can not use _() method directly for the case _.pathinfo('a/').
    var type = typeof path;
    if(arguments.length > 1) {
        path = Array.prototype.join.call(arguments, '/');
    } else if(type === 'string') {
        //do nothing for quickly determining.
    } else if(type === 'object') {
        path = Array.prototype.join.call(path, '/');
    }
    return _.ext(path);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fis.util.pipe"></a>[function <span class="apidocSignatureSpan">fis.util.</span>pipe (type, callback, def)](#apidoc.element.fis.util.pipe)
- description and source-code
```javascript
pipe = function (type, callback, def){
    var processors = fis.config.get('modules.' + type, def);
    if(processors){
        var typeOf = typeof processors;
        if(typeOf === 'string'){
            processors = processors.trim().split(/\s*,\s*/);
        } else if(typeOf === 'function'){
            processors = [ processors ];
        }
        type = type.split('.')[0];
        processors.forEach(function(processor, index){
            var typeOf = typeof processor, key;
            if(typeOf === 'string'){
                key = type + '.' + processor;
                processor = fis.require(type, processor);
            } else {
                key = type + '.' + index;
            }
            if(typeof processor === 'function'){
                var settings = fis.config.get('settings.' + key, {});
                if(processor.defaultOptions){
                    settings = _.merge(processor.defaultOptions, settings);
                }
                callback(processor, settings, key);
            } else {
                fis.log.warning('invalid processor [modules.' + key + ']');
            }
        });
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fis.util.query"></a>[function <span class="apidocSignatureSpan">fis.util.</span>query (str)](#apidoc.element.fis.util.query)
- description and source-code
```javascript
query = function (str){
    var rest = str,
        pos = rest.indexOf('#'),
        hash = '',
        query = '';
    if(pos > -1){
        hash = rest.substring(pos);
        rest  = rest.substring(0, pos);
    }
    pos = rest.indexOf('?');
    if(pos > -1){
        query = rest.substring(pos);
        rest  = rest.substring(0, pos);
    }
    rest = rest.replace(/\\/g, '/');
    if(rest !== '/'){
        rest = rest.replace(/\/\.?$/, '');
    }
    return {
        origin : str,
        rest : rest,
        hash : hash,
        query : query
    };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fis.util.read"></a>[function <span class="apidocSignatureSpan">fis.util.</span>read (path, convert)](#apidoc.element.fis.util.read)
- description and source-code
```javascript
read = function (path, convert){
    var content = false;
    if(_exists(path)){
        content = fs.readFileSync(path);
        if(convert || _.isTextFile(path)){
            content = _.readBuffer(content);
        }
    } else {
        fis.log.error('unable to read file[' + path + ']: No such file or directory.');
    }
    return content;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fis.util.readBuffer"></a>[function <span class="apidocSignatureSpan">fis.util.</span>readBuffer (buffer)](#apidoc.element.fis.util.readBuffer)
- description and source-code
```javascript
readBuffer = function (buffer){
    if(_.isUtf8(buffer)){
        buffer = buffer.toString('utf8');
        if (buffer.charCodeAt(0) === 0xFEFF) {
            buffer = buffer.substring(1);
        }
    } else {
        buffer = getIconv().decode(buffer, 'gbk');
    }
    return buffer;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fis.util.readJSON"></a>[function <span class="apidocSignatureSpan">fis.util.</span>readJSON (path)](#apidoc.element.fis.util.readJSON)
- description and source-code
```javascript
readJSON = function (path){
    var json = _.read(path),
        result = {};
    try {
        result = JSON.parse(json);
    } catch(e){
        fis.log.error('parse json file[' + path + '] fail, error [' + e.message + ']');
    }
    return result;
}
```
- example usage
```shell
...
//colors
fis.cli.colors = require('colors');

//commander object
fis.cli.commander = null;

//package.json
fis.cli.info = fis.util.readJSON(__dirname + '/package.json');

//output help info
fis.cli.help = function(){
var content = [
    '',
    '  Usage: ' + fis.cli.name + ' <command>',
    '',
...
```

#### <a name="apidoc.element.fis.util.realpath"></a>[function <span class="apidocSignatureSpan">fis.util.</span>realpath (path)](#apidoc.element.fis.util.realpath)
- description and source-code
```javascript
realpath = function (path){
    if(path && _exists(path)){
        path = fs.realpathSync(path);
        if(IS_WIN){
            path = path.replace(/\\/g, '/');
        }
        if(path !== '/'){
            path = path.replace(/\/$/, '');
        }
        return path;
    } else {
        return false;
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fis.util.realpathSafe"></a>[function <span class="apidocSignatureSpan">fis.util.</span>realpathSafe (path)](#apidoc.element.fis.util.realpathSafe)
- description and source-code
```javascript
realpathSafe = function (path){
    return _.realpath(path) || _(path);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fis.util.stringQuote"></a>[function <span class="apidocSignatureSpan">fis.util.</span>stringQuote (str, quotes)](#apidoc.element.fis.util.stringQuote)
- description and source-code
```javascript
stringQuote = function (str, quotes){
    var info = {
        origin : str,
        rest   : str = str.trim(),
        quote  : ''
    };
    if(str){
        quotes = quotes || '\'"';
        var strLen = str.length - 1;
        for(var i = 0, len = quotes.length; i < len; i++){
            var c = quotes[i];
            if(str[0] === c && str[strLen] === c){
                info.quote = c;
                info.rest  = str.substring(1, strLen);
                break;
            }
        }
    }
    return info;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fis.util.toEncoding"></a>[function <span class="apidocSignatureSpan">fis.util.</span>toEncoding (str, encoding)](#apidoc.element.fis.util.toEncoding)
- description and source-code
```javascript
toEncoding = function (str, encoding){
    return getIconv().toEncoding(String(str), encoding);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fis.util.touch"></a>[function <span class="apidocSignatureSpan">fis.util.</span>touch (path, mtime)](#apidoc.element.fis.util.touch)
- description and source-code
```javascript
touch = function (path, mtime){
    if(!_exists(path)){
        _.write(path, '');
    }
    if(mtime instanceof Date){
        //do nothing for quickly determining.
    } else if(typeof mtime === 'number') {
        var time = new Date();
        time.setTime(mtime);
        mtime = time;
    } else {
        fis.log.error('invalid argument [mtime]');
    }
    fs.utimesSync(path, mtime, mtime);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fis.util.upload"></a>[function <span class="apidocSignatureSpan">fis.util.</span>upload (url, opt, data, content, subpath, callback)](#apidoc.element.fis.util.upload)
- description and source-code
```javascript
upload = function (url, opt, data, content, subpath, callback){
    if(typeof content === 'string'){
        content = new Buffer(content, 'utf8');
    } else if(!(content instanceof  Buffer)){
        fis.log.error('unable to upload content [' + (typeof content) + ']');
    }
    data = data || {};
    var endl = '\r\n';
    var boundary = '-----np' + Math.random();
    var collect = [];
    _.map(data, function(key, value){
        collect.push('--' + boundary + endl);
        collect.push('Content-Disposition: form-data; name="' + key + '"' + endl);
        collect.push(endl);
        collect.push(value + endl);
    });
    collect.push('--' + boundary + endl);
    collect.push('Content-Disposition: form-data; name="file"; filename="' + subpath + '"' + endl);
    collect.push(endl);
    collect.push(content);
    collect.push('--' + boundary + '--' + endl);

    var length = 0;
    collect.forEach(function(ele){
        length += ele.length;
    });

    opt = opt || {};
    opt.method = opt.method || 'POST';
    opt.headers = {
        'Content-Type': 'multipart/form-data; boundary=' + boundary,
        'Content-Length': length
    };
    opt = _.parseUrl(url, opt);
    var http = opt.protocol === 'https:' ? require('https') : require('http');
    var req = http.request(opt, function(res){
        var status = res.statusCode;
        var body = '';
        res
            .on('data', function(chunk){
                body += chunk;
            })
            .on('end', function(){
                if(status >= 200 && status < 300 || status === 304){
                    callback(null, body);
                } else {
                    callback(status);
                }
            })
            .on('error', function(err){
                callback(err.message || err);
            });
    });
    collect.forEach(function(d){
        req.write(d);
        if(d instanceof Buffer){
            req.write(endl);
        }
    });
    req.end();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fis.util.write"></a>[function <span class="apidocSignatureSpan">fis.util.</span>write (path, data, charset, append)](#apidoc.element.fis.util.write)
- description and source-code
```javascript
write = function (path, data, charset, append){
    if(!_exists(path)){
        _.mkdir(_.pathinfo(path).dirname);
    }
    if(charset){
        data = getIconv().encode(data, charset);
    }
    if(append) {
        fs.appendFileSync(path, data, null);
    } else {
        fs.writeFileSync(path, data, null);
    }
}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
