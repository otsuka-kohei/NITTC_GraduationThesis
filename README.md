東京高専情報工学科の卒業論文のLaTeXテンプレートです。  

卒業論文テンプレートのWordファイルに似せて作りました。

sample.tex : 2021年2月現在の卒業論文テンプレート  
old.tex : リポジトリ管理者が高専生だったころの卒業論文テンプレート

コンパイル例 : [sample.pdf](https://github.com/otsuka-kohei/NITTC_GraduationThesis/files/5949085/sample.pdf)

参考に、VSCodeのTeX用拡張機能[LaTeX Workshop](https://marketplace.visualstudio.com/items?itemName=James-Yu.latex-workshop)用のコンパイルレシピを以下に示します。
```
{
    "latex-workshop.latex.recipes": [
        {
            "name": "ptex2pdf*2",
            "tools": [
                "ptex2pdf",
                "ptex2pdf"
            ]
        }
    ],
    "latex-workshop.latex.tools": [
        {
            "name": "ptex2pdf",
            "command": "ptex2pdf",
            "args": [
                "-u",
                "-l",
                "%DOC%"
            ]
        }
    ]
}
```
