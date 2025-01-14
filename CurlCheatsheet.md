# CurlCheatsheet
 Curl cheatsheet

[Devhints.io](/)

*   [Edit](https://github.com/rstacruz/cheatsheets/blob/master/curl.md)

Curl cheatsheet
===============

 [![](https://srv.carbonads.net/static/30242/4ba790229c6114149037637d63c301b1d9530897)](https://srv.carbonads.net/ads/click/x/GTND427ICYADPK7LC6BLYKQUCKSIC27UC6AIKZ3JCA7I5KJNCKADEKJKCW7DKKQJCE7DV2JLF67IP2JECESIPKQKC6SIC2JYF6BIKK3EHJNCLSIZ) [ Create a website that reflects your personal brand with Squarespace. Start your free trial. ](https://srv.carbonads.net/ads/click/x/GTND427ICYADPK7LC6BLYKQUCKSIC27UC6AIKZ3JCA7I5KJNCKADEKJKCW7DKKQJCE7DV2JLF67IP2JECESIPKQKC6SIC2JYF6BIKK3EHJNCLSIZ) [ads via Carbon](http://carbonads.net/?utm_source=devhintsio&utm_medium=ad_via_link&utm_campaign=in_unit&utm_term=carbon)

![](https://ad.doubleclick.net/ddm/trackimp/N718679.452584BUYSELLADS.COM/B29332811.401293654;dc_trk_aid=593420481;dc_trk_cid=207494836;ord=173689718;dc_lat=;dc_rdid=;tag_for_child_directed_treatment=;tfua=;ltd=;dc_tdv=1?)

Options[#](#options)
--------------------

### Options

```
-o <file>    # --output: write to file
-u user:pass # --user: Authentication 
```

```
-v           # --verbose
-vv          # Even more verbose
-s           # --silent: don't show progress meter or errors
-S           # --show-error: when used with --silent (-sS), show errors but no progress meter 
```

```
-i           # --include: Include the HTTP-header in the output
-I           # --head: headers only 
```

### Request

```
-X POST          # --request
-L               # follow link if page redirects
-F               # --form: HTTP POST data for multipart/form-data 
```

### Data

```
-d 'data'    # --data: HTTP post data, URL encoded (eg, status="Hello")
-d @file     # --data via file
-G           # --get: send -d data via get 
```

### Headers

```
-A <str>         # --user-agent
-b name=val      # --cookie
-b FILE          # --cookie
-H "X-Foo: y"    # --header
--compressed     # use deflate/gzip 
```

### SSL

```
 --cacert <file>
    --capath <dir> 
```

```
-E, --cert <cert>     # --cert: Client cert file
    --cert-type       # der/pem/eng
-k, --insecure        # for self-signed certs 
```

Examples[#](#examples)
----------------------

```
# Post data:
curl -d password=x http://x.com/y 
```

```
# Auth/data:
curl -u user:pass -d status="Hello" http://twitter.com/statuses/update.xml 
```

```
# multipart file upload
curl -v --include --form key1=value1 --form upload=@localfilename URL

# multipart form: send data from text field and upload file
curl -F person=anonymous -F secret=@file.txt http://example.com/submit.cgi 
```

```
# Use Curl to Check if a remote resource is available
# details: https://matthewsetter.com/check-if-file-is-available-with-curl/
curl -o /dev/null --silent -Iw "%{http_code}" https://example.com/my.remote.tarball.gz 
```

**0 Comments** for this cheatsheet. Write yours!

devhints.io / 

[

Over 357 curated cheatsheets, by developers for developers.

Devhints home



](/)

### Other CLI cheatsheets

*   [**Cron** cheatsheet](/cron)
*   [**Homebrew** cheatsheet](/homebrew)
*   [**httpie** cheatsheet](/httpie)
*   [**adb (Android Debug Bridge)** cheatsheet](/adb)
*   [**composer** cheatsheet](/composer)
*   [**Fish shell** cheatsheet](/fish-shell)

### Top cheatsheets

*   [**Elixir** cheatsheet](/elixir)
*   [**ES2015+** cheatsheet](/es6)
*   [**React.js** cheatsheet](/react)
*   [**Vim** cheatsheet](/vim)
*   [**Vimdiff** cheatsheet](/vim-diff)
*   [**Vim scripting** cheatsheet](/vimscript)