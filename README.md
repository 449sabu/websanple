# websanple
`CSS`や`JavaScript`をraw形式で参照したい場合。<br>
`raw.githubusercontent`は、ファイルがCSSまたはJavaScriptファイルであっても、すべてのファイルで`text /plain`MIMEタイプを使用するようにします。<br>
したがって、`https：//raw.githubusercontent.com/‹user›/‹repo›/‹branch›/‹filepath›`にアクセスすると、正しいMIMEタイプではなく、プレーンテキストファイルになり、`<link href="#"/>`または`<scriptsrc="#"></ script>`は機能しません。<br>
GitHub Pagesはリポジトリを特別なURLでホストするため、ファイルをチェックインしてプッシュするだけです。<br>
ほとんどの場合、GitHubPagesでは特別なブランチgh-pagesにコミットする必要があることに注意してください。<br>
`https：//‹user›.github.io/<repo›`では、gh-pagesブランチにコミットされたすべてのファイル（最新のコミット）がこのURLに存在します。<br>
したがって、`<script src="https：//‹user›.github.io/‹repo›/file.js"></script>`を介してjsファイルにリンクできます。これは、正しいMIMEタイプになります。

***
参照：[Link and execute external JavaScript file hosted on GitHub](https://stackoverflow.com/questions/17341122/link-and-execute-external-javascript-file-hosted-on-github#:~:text=GitHub%20Pages%20is%20GitHub's%20official,a%20CSS%20or%20JavaScript%20file.)
