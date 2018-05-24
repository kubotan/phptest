# travis ciによるCakePHPコーディング規約自動テストの試行ページ
- 下記のバッチのbuildがpassingとなっていればコーディング規約は問題ない。failingの場合は、参考例の様に改行入れろ！！的なdiffが表示される。

[![GitHub release](https://img.shields.io/github/release/kubotan/phptest.svg)](https://github.com/kubotan/phptest/releases)
[![Build Status]( https://travis-ci.org/kubotan/phptest.svg?branch=master)](https://travis-ci.org/kubotan/phptest)
[![contributions welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat)](https://github.com/kubotan/phptest/issues)
[![License: LGPL v3](https://img.shields.io/badge/License-LGPL%20v3-blue.svg)](https://github.com/kubotan/phptest/blob/master/LICENSE)


## 参考例

~~~
0.29s$ ~/.composer/vendor/bin/phpcs --report=diff ~/build/kubotan/phptest/src/
--- src/ng.php
+++ PHP_CodeSniffer
@@ -1 +1,3 @@
-<?php use Acme\Hoge;class Fuga{ // ~ anything ~ }
+<?php use Acme\Hoge;
+
+class Fuga{ // ~ anything ~ }
~~~

## 備考
- このチェックはプルリクなどで自動的に動くはず。
