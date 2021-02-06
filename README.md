東京高専情報工学科の卒業論文のLaTeXひな型です。

先輩などから受け継がれているwordファイルの書式に似せて作りました。
  
  
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
