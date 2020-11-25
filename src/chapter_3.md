# Vimming with Coc 

Coc is perhaps the king of all Vim plugins. Because it's not *just* a plugin. It's more like a full plugin environment integrated closely to vim that adds all sorts of cool features. It's literally that plugin that turns Vim from a text editor to an IDE.

To get started with Coc, familiarize yourself again with the vim-plug system. As a refresher, vim-plug uses a special portion of your `~/.vimrc` file to manage plugins. If you've forgotten, here's how it should look like:

```vim
 
call plug#begin('~/.vim/plugged')

" put your vim plugins here 

call plug#end()
```

The code for coc is `Plug 'neoclide/coc.nvim', {'branch': 'release'}`. Just paste that in to your vim-plug code block. Like this:

```vim
 
call plug#begin('~/.vim/plugged')

" The Coc plugin 
Plug 'neoclide/coc.nvim', {'branch': 'release'}

" put your other vim plugins within this section

call plug#end()
```
Now, just do a `source ~/.vimrc` and a `:PlugInstall`. Wait for the plugin download screen to stop flashing, and you can begin using Coc.

First things first, you've got to add some basic languages to Coc. Being a web and frontend/GUI developer mostly, I usually go for the web design languages, and maybe python. That's why I recomment you to add html, css, js, and json first, as well as the word dtatbase from the makers of VSCode, like this:

```vim
:CocInstall coc-html coc-css coc-tsserver coc-json coc-word
```

Now, start writing some code! You'll see recomennded words to use within a popu menu. And just use the down and up arrow keys to choose your desired word. This can be useful in writing non-code prose as well, such as long essays with lots of long words. 

To make the plugin install process less obtrusive, I recommend downloading the `coc-marketplace` plugin, with ` :CocInstall coc-marketplace`. After sourcing the `.vimrc` and running ` :PlugInstall`, you can simply type ` :CocInstall coc-marketplace` to search through all your extensions.

Once you've downloaded them, use the command `:CocList extensions` to do your view an manager work. Press the tab key to toggle, enable, and control your extensions. `:CocUpdate` will update all extensions, if that's your style.

And my favorite part - ` :CocList commands` allows you to run any coc-supported feature and plugin subfeature with simper-simple input. It's also fuzzy searched, so no worries about bad typing!

![](images/CocList-commands.png)

In addition, the extensions often use the vim `CR` key, also known as the `\` character. Add `nmap <space>e :CocCommand explorer<CR>` to change the `CR` key to the `,` key. 


