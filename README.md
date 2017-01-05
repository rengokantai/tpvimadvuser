# tpvimadvuser
##2. Settings and Options
###1 Working with Text Objects
```
fs //next s
vfs //visual next s
```

```
viw  //when the cousor is in the word, select the whole word
diw //deleteword
```

vaW // visulize word including whitespace




##4. More Vimscript
###1 Functions
H: firstline first char
O: insert a new line above and insert mode
^[: escape
```
function! AddHelloTop
  normal HOhello there^[A vim user^[0
  s/hello there/hi/
  return "message"
endfunction
```
call a function
```
command! Hello call AddHelloTop
```






##5. Plugins
###1 Adding Support for Other Languages
```
cd .vim
cd bundle
git clone http://github.com/..
```
###2 Surrond Plugin
```
ds(   //delete surronding parentheses
```

```
dst  //delete surronding tags
```

replace surronding char
```
cs({    //change () to {}
cs{<p>   //change {} to <p></p>
``` 
add
```
ysiw"  // aa=>"aa"
ysaw{   //aa=>{ aa }
yss"   //surrond line 
ySaw{  //indent
```
