## vim

- <https://github.com/chriskempson/base16-vim/blob/master/colors/base16-default-light.vim> `c1c3e6c`
- <https://github.com/chriskempson/base16-vim/blob/master/colors/base16-default-dark.vim> `c1c3e6c`

```
3,10d | 4d | 5d | 36d | 42,49d |
4s#.*/#execute "silent !/bin/sh $HOME/.nightshell/# |
4s/\.sh// |
%s/base16-default/vrunchbang/ |

%s/181818/191d1f/ |
%s/282828/282e30/ |
%s/383838/444e52/ |
%s/585858/5d6b70/ |
%s/b8b8b8/999999/ |
%s/d8d8d8/bfbfbf/ |
%s/e8e8e8/e8e8e8/ |
%s/f8f8f8/ffffff/ |

%s/ab4642/bf5050/ |
%s/dc9656/bf7730/ |
%s/f7ca88/ab8b2b/ |
%s/a1b56c/629431/ |
%s/86c1b9/31947b/ |
%s/7cafc2/4892ab/ |
%s/ba8baf/7373ab/ |
%s/a16946/ab73ab/ |

%s/Character",    s:gui08, "", s:cterm08/Character",    s:gui05, "", s:cterm05/ |
%s/Cursor",        s:gui00, s:gui05, s:cterm00, s:cterm05/Cursor",        s:gui00, s:gui04, s:cterm00, s:cterm04/ |
%s/CursorLineNr",  s:gui04, s:gui01, s:cterm04, s:cterm01/CursorLineNr",  s:gui00, s:gui03, s:cterm00, s:cterm03/ |
%s/Identifier",   s:gui08, "", s:cterm08, "", "none/Identifier",   s:gui05, "", s:cterm05, "", "bold/ |
%s/LineNr",        s:gui03, s:gui01, s:cterm03/LineNr",        s:gui04, s:gui01, s:cterm04/ |
%s/MatchParen",    "", s:gui03, "", s:cterm03/MatchParen",    s:gui00, s:gui03, s:cterm00, s:cterm03/ |
%s/Search",        s:gui03, s:gui0A, s:cterm03, s:cterm0A,  "", "")/Search",        s:gui00, s:gui0A, s:cterm00, s:cterm0A,  "", "")/ |
%s/statusline",    s:gui04, s:gui02, s:cterm04, s:cterm02/statusline",    s:gui00, s:gui04, s:cterm00, s:cterm04/ |
%s/StatusLineNC",  s:gui03, s:gui01, s:cterm03, s:cterm01/StatusLineNC",  s:gui05, s:gui01, s:cterm05, s:cterm01/ |
%s/Visual",        "", s:gui02, "", s:cterm02/Visual",        s:gui06, s:gui02, s:cterm06, s:cterm02/ |
%s/VisualNOS",     s:gui08, "", s:cterm08, "", ""/VisualNOS",     "", s:gui01, "", s:cterm01, "none"/ |
%s/WildMenu",      s:gui08, s:gui0A, s:cterm08, ""/WildMenu",      s:gui00, s:gui06, s:cterm00, s:cterm06/ |

normal =gg
```

## nightshell

- <https://raw.githubusercontent.com/chriskempson/base16-shell/master/scripts/base16-default-light.sh> `376294b`
- <https://raw.githubusercontent.com/chriskempson/base16-shell/master/scripts/base16-default-dark.sh> `376294b`

```
2,4d |

%s#18/18/18#19/1d/1f# |
%s#28/28/28#28/2e/30# |
%s#38/38/38#44/4e/52# |
%s#58/58/58#5d/6b/70# |
%s#b8/b8/b8#99/99/99# |
%s#d8/d8/d8#bf/bf/bf# |
%s#e8/e8/e8#e8/e8/e8# |
%s#f8/f8/f8#ff/ff/ff# |
%s#ab/46/42#bf/50/50# |
%s#dc/96/56#bf/77/30# |
%s#f7/ca/88#ab/8b/2b# |
%s#a1/b5/6c#62/94/31# |
%s#86/c1/b9#31/94/7b# |
%s#7c/af/c2#48/92/ab# |
%s#ba/8b/af#73/73/ab# |
%s#a1/69/46#ab/73/ab# |

%s/181818/191d1f/ge |
%s/383838/444e52/g |
%s/d8d8d8/bfbfbf/g |
%s/f8f8f8/ffffff/ge |

call append(123,["",
"echo -ne '\\e]12;#5d6b70\\a'"]) |

if @% =~ 'dark' | 125s/5d6b70/999999/ | endif
```
