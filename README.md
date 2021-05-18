<!--
## The PowerShell Best Practices and Style Guide
-->

PowerShellのベストプラクティスとスタイルガイド

<!--
[Table Of Contents](#table-of-contents)
-->

[目次](#table-of-contents)


<!--
<p align="center"><a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/" style="display: inline-block; float: left; vertical-align: middle; margin: 10px;"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by-sa/4.0/88x31.png" /></a></p>
-->

<p align="center"><a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/" style="display: inline-block; float: left; vertical-align: middle; margin: 10px;"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by-sa/4.0/88x31.png" /></a></p>

<!--
This work is licensed under a [Creative Commons Attribution-ShareAlike 4.0 International License](http://creativecommons.org/licenses/by-sa/4.0/), please attribute to Don Jones, Matt Penny, Carlos Perez, Joel Bennett と  PowerShell Community.
-->

この作品は[Creative Commons Attribution-ShareAlike 4.0 International License](http://creativecommons.org/licenses/by-sa/4.0/)に基づいてライセンスされています。Don Jones, Matt Penny, Carlos Perez, Joel Bennett そして the PowerShell Communityに帰属させてください。

<!--
###### You are free to:
-->

###### あなたは以下のことを自由に行うことができます:

<!--
**Share** — copy and redistribute the material in any medium or format
-->

**共有** — 媒体や形式を問わず、コピーや再配布を行うこと。

<!--
**Adapt** — remix, transform, and build upon the material
-->

**改作** — 改変, 変形, そして 本作品をベースに別の作品を作ること。

<!--
The authors encourage you to redistribute this content as widely as possible, but require that you give credit to the primary authors below, and that you notify us on GitHub of any improvements you make.
-->

このコンテンツを可能な限り広く再配布することをお勧めします。ただし、以下の主要著者にクレジットを付与し、改良を加えた場合にはGitHubで通知することが必要です。

<!--
### What are Best Practices
-->
### ベストプラクティスとは何ですか？

<!--
_PowerShell Best Practices_ are what you should usually do as a starting point. They are ways of writing, thinking, and designing which make it _harder_ to get into trouble. The point of a _Best Practice_ is to help the reader to fall into the pit of success:
-->

_PowerShellのベストプラクティス_ は、出発点としてあなたが通常行うべきことです。
それらはトラブルに 「_巻き込まれにくく_」 するための書き方、考え方、そしてデザインの方法です。
_ベストプラクティス_ のポイントは、読者が成功の落とし穴に落ちるのを助けることです。

<!--
> **The Pit of Success:** in stark contrast to a summit, a peak, or a journey across a desert to find victory through many trials and surprises, we want our customers to simply fall into winning practices by using our platform and frameworks.  To the extent that we make it easy to get into trouble we fail.
-->

> **成功の落とし穴:** 山頂やピーク、あるいは砂漠を越えて多くの試練や驚きの中から勝利を見出す旅とは全く対照的に、私たちはお客様が私たちのプラットフォームやフレームワークを使うことで、単に勝利のための実践に陥ってほしいと考えています。困難に陥ることを容易にしたところで、私たちは失敗するのです。

<!--
> -- Rico Mariani, MS Research MindSwap Oct 2003.
-->

> -- Rico Mariani, MS Research MindSwap Oct 2003.

<!--
Like English spelling and grammar rules, PowerShell programming best practices and style rules nearly always have exceptions, but we are documenting a baseline for code structure, command design, programming, formatting, and even style which will help you to avoid common problems, and help you write more reusable, readable code -- because reusable code doesn't have to be rewritten, and readable code can be maintained.
-->

英語のスペルや文法のルールと同様に、PowerShellプログラミングのベストプラクティスやスタイルのルールにも例外がありますが、コード構造、コマンドデザイン、プログラミング、フォーマット、さらにはスタイルの基本を文書化することで、よくある問題を回避し、より再利用可能で読みやすいコードを書けるようにします。

<!--
Having said that, remember: the points in the Best Practices documents and the Style Guide are referred to as _practices_ and _guidelines_, not rules. If you're having trouble getting something done because you're trying to avoid _breaking_ a style or best practice rule, you've misunderstood the point: this document is pragmatic, rather than dogmatic. We'll leave dogmatism to teams and projects that require you to meet their specific guidelines.
-->

とはいえ、ベスト・プラクティス・ドキュメントやスタイル・ガイドに記載されているポイントは、ルールではなく「_プラクティス_」や「_ガイドライン_」と呼ばれていることを覚えておいてください。スタイルやベスト・プラクティスのルールに違反しないようにするために、何かを成し遂げるのに苦労しているとしたら、それはポイントを誤解しています。独断的なものは、特定のガイドラインを満たすことを要求するチームやプロジェクトに任せることにしましょう。


<!--
### Table of Contents
-->

### 目次

<!--
The guidelines are divided into these sections:
-->

このガイドラインはこれらのセクションに分かれています。:

<!--
* [Style Guide (Introduction)](Style-Guide/Introduction.md)
  * [Code Layout and Formatting](Style-Guide/Code-Layout-and-Formatting.md)
  * [Function Structure](Style-Guide/Function-Structure.md)
  * [Documentation and Comments](Style-Guide/Documentation-and-Comments.md)
  * [Readability](Style-Guide/Readability.md)
  * [Naming Conventions](Style-Guide/Naming-Conventions.md)
* [Best Practices (Introduction)](Best-Practices/Introduction.md)
  * [Naming Conventions](Best-Practices/Naming-Conventions.md)
  * [Building Reusable Tools](Best-Practices/Building-Reusable-Tools.md)
  * [Output and Formatting](Best-Practices/Output-and-Formatting.md)
  * [Error Handling](Best-Practices/Error-Handling.md)
  * [Performance](Best-Practices/Performance.md)
  * [Security](Best-Practices/Security.md)
  * [Language, Interop and .Net](Best-Practices/Language-Interop-and-.Net.md)
  * [Metadata, Versioning, and Packaging](Best-Practices/Metadata-Versioning-and-Packaging.md)
-->

* [Style Guide (Introduction)](Style-Guide/Introduction.md)
  * [Code Layout and Formatting](Style-Guide/Code-Layout-and-Formatting.md)
  * [Function Structure](Style-Guide/Function-Structure.md)
  * [Documentation and Comments](Style-Guide/Documentation-and-Comments.md)
  * [Readability](Style-Guide/Readability.md)
  * [Naming Conventions](Style-Guide/Naming-Conventions.md)
* [Best Practices (Introduction)](Best-Practices/Introduction.md)
  * [Naming Conventions](Best-Practices/Naming-Conventions.md)
  * [Building Reusable Tools](Best-Practices/Building-Reusable-Tools.md)
  * [Output and Formatting](Best-Practices/Output-and-Formatting.md)
  * [Error Handling](Best-Practices/Error-Handling.md)
  * [Performance](Best-Practices/Performance.md)
  * [Security](Best-Practices/Security.md)
  * [Language, Interop and .Net](Best-Practices/Language-Interop-and-.Net.md)
  * [Metadata, Versioning, and Packaging](Best-Practices/Metadata-Versioning-and-Packaging.md)


<!--
### Current State:
-->

### 現在の状態:


<!--
Remember [what we mean by _Best Practices_](#what-are-best-practices)
-->

[「_ベストプラクティス_」の意味](#what-are-best-practices)を思い出してください。


<!--
The *PowerShell Best Practices* are always evolving, and continue to be edited and updated as the language and tools (and our community understanding of them) evolve. We encourage you to check back for new editions at least twice a year, by visiting [https://github.com/PoshCode/PowerShellPracticeAndStyle](https://github.com/PoshCode/PowerShellPracticeAndStyle)
-->

*PowerShell Best Practices*は常に進化しており、言語やツール（およびそれらに対するコミュニティの理解）の進化に合わせて編集・更新され続けています。少なくとも年に2回は、[https://github.com/PoshCode/PowerShellPracticeAndStyle](https://github.com/PoshCode/PowerShellPracticeAndStyle)にアクセスして、新版をチェックすることをお勧めします。

<!--
The *PowerShell Style Guide* in particular is in PREVIEW, and we are still actively working out our disagreements about the rules in the guide through the GitHub issues system.
-->

特に*PowerShell Style Guide*はPREVIEWになっていて、GitHub issues systemを通じてガイドのルールに関する意見の相違を積極的に解消しているところです。

<!--
#### Contributing
-->

#### 貢献

<!--
Please use the issues system or GitHub pull requests to make corrections, contributions, and other changes to the text - we welcome your contributions!
-->

本文中の修正、寄稿、その他の変更は、課題システムやGitHubのプルリクエストをご利用ください。皆様のご協力をお待ちしております。

<!--
For more information, see [CONTRIBUTING](CONTRIBUTING.md)
-->

詳しくは、[CONTRIBUTING](CONTRIBUTING.md)をご覧ください。

<!--
#### Credits
-->

#### クレジット

<!--
_The Community Book of PowerShell Practices_ was originally compiled and edited by Don Jones and Matt Penny with input from the Windows PowerShell community on PowerShell.org
-->

_The Community Book of PowerShell Practices_ は、PowerShell.orgのWindows PowerShellコミュニティからの情報をもとに、Don JonesとMatt Pennyが編集したものです。

<!--
Portions copyright (c) Don Jones, Matt Penny, 2014-2015
-->

Portions copyright (c) Don Jones, Matt Penny, 2014-2015

<!--
_The PowerShell Style Guide_ was originally created by Carlos Perez, for his students, and all the good parts were written by him.
-->

PowerShell Style Guide_は、Carlos Perezが学生のために作成したもので、良い部分はすべて彼が書いています。

<!-- 
Portions copyright (c) Carlos Perez, 2015
-->

Portions copyright (c) Carlos Perez, 2015

<!--
Any mistakes in either of these documents are there because Joel Bennett got involved. Please submit [issues](https://github.com/PoshCode/PowerShellPracticeAndStyle/issues) and help us correct them.
-->

これらの文書のいずれかに誤りがある場合は、Joel Bennettが関与したためにあります。ぜひ[issue](https://github.com/PoshCode/PowerShellPracticeAndStyle/issues)を投稿して、訂正にご協力ください。

<!--
Portions copyright (c) Joel Bennett, 2015
-->

Portions copyright (c) Joel Bennett, 2015