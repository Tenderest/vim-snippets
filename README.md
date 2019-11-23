# 这是我的snippets（代码块）备份  
1. 使用Vim插件使用vundle管理  
"  
" Ultisnips  
"  
Plugin 'SirVer/ultisnips'  
"  
" Ultisnips setting  
"  
"展开代码片段"  
let g:UltiSnipsExpandTrigger="\<C-i\>"  
"下一个触发点"  
let g:UltiSnipsJumpForwardTrigger="\<C-n\>"  
"上一个触发点"  
let g:UltiSnipsJumpBackwardTrigger="\<C-N\>"  
" 使用 UltiSnipsEdit 命令时垂直分割屏幕  
let g:UltiSnipsEditSplit="vertical"  
1. 使用自己的代码片段仓库
'Tenderest/vim-snippets'  
1. 文件目录在  
~/.vim/bundle/vim-snippets    
" 如果文件不是在 ~/.vim/mycoolsnippets  
" 每次进入Vim自动寻找目录下的Snippets文件配置  
let g:UltiSnipsSnippetDirectories=[$HOME.'/.vim/bundle/vim-snippets']  
" 如果文件在 ~/.vim/mycoolsnippets  
" let g:UltiSnipsSnippetDirectories=["UltiSnips", "mycoolsnippets"]  
1. 代码片段补全格式  
snippet \<"触发补全的名字"\> \<"对这个补全的一些描述"\> \<"参数 A表示自动补全 i 表示可以在某个单词里触发，不建议"\>  
" 代码片段  
${数字:todo}  
" 表示补全以后光标停留的位置，用花括号的部分会被选中用来提示替换  
" 数字代表顺序，从1开始，0是最后光标停留的位置  
endsnippet  
