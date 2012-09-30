vim-markdown-preview
====================

Vim: Preview a Markdown document in the default browser on Windows or Linux

Original code: <https://gist.github.com/960015>

Install
-------
    aptitude install markdown

~/.vimrc

    Bundle 'imbolc/vim-markdown-preview'
    au BufRead,BufNewFile *.md      setlocal filetype=markdown
    au FileType markdown            setlocal et sw=4 ts=4 sts=4
    au FileType markdown            map <F5> :call MarkdownPreview()<CR>
