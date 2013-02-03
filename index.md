<section data-markdown>
    <script type="text/template">
        ## Page title

        A paragraph with some text and a [link](http://hakim.se).
    </script>
</section>% VIM VIM VIM
% Паршенко Дмитрий


# История

&nbsp;

### Vi
Первый релиз в 1976 году, автор &mdash; Билл Джой

&nbsp;

### Vim (Vi Improved)
Первый релиз в 1991 году, автор &mdash; Брам Мооленаар

# Что было добавлено в **Vim**

- Проверка правописания
- Скрипты (vimscript, Perl, Python, Ruby, Tcl, scheme и другие)
- Редактирование файлов в архивах (gzip, bzip2, zip, tar)
- Окна и вкладки
- Поддержка Unicode
- Встроенная система помощи
- Редактирование по SSH, FTP, HTTP
- и другое

# Tl;dr

&nbsp;

&nbsp;

&nbsp;

&nbsp;


## :q&lt;Enter&gt;


# Чем Vim отличается от обычного редактора

**Модальный**. Работает в нескольких режимах. Одна клавиша выполняет разные функции в разных режимах.

Позволяет переназначать клавиши как только угодно.

Руки не покидают основного блока клавиш.

Настройка и скрипты.

Связка с unix tools.



# Что делать?

- Быстро передвигаться по тексту
- Не повторяться
- Автоматизировать часто используемые функции
      - заметил повторение
      - автоматизировал
      - взял за привычку

# Режимы
Переход из любого режима в Normal &mdash; Esc.

Функцию клавиши (или комбинации) можно назначать отдельно для любого режима.

## Normal
Передвижение по тексту, манипуляции: удаление, копирование, вставка и другое.
Б*о*льшую часть времени вы находитесь в этом режиме.

## Insert
Непосредственное написание текста.
Из этого режима вы выходите как только написали необходимое количество текста.

#### Replace
От Insert отличается тем, что заменяет символы, а не вставляет. Аналогично нажатой клавише insert в обычном редакторе.

# Режимы

## Visual
Выделение текста. В этом режиме вы можете использовать возможности перемещения свойственные режиму Normal.
gv &mdash; последнее выделение.
% &mdash; перемещение между границами выделения.
@* &mdash; регистр, содержащий последнюю выделенную строку.

#### Visual Line
Выделение строк.

#### Visual Block
Выделение прямоугольного блока текста.

## Command
Режим для выполнения команд: открытие файла, выход, изменение настроек, вызов команд плагинов и т. д.


#

![](http://lmarburger.github.com/vim_vs_emacs/file/one/vim-cheat-sheet.png "Cheat Sheet")

# Переход в режим вставки
- i &mdash; перед курсором (insert)
- I &mdash; в начале строки
- a &mdash; за курсором (append)
- A &mdash; за строкой
- o &mdash; вставить строку ниже
- O &mdash; вставить строку выше
- s &mdash; с удалением одного символа (substitute)
- S &mdash; замена строки
 
# Text Objects и комбинации клавиш

### 1. Глагол
**d** (delete),
**c** (change),
**y** (yank),

### 2. Наречие

**i** (inner),
**a** (around / all)

### 3. Существительное

**t** (tag), 
**w** (word), 
**p** (paragraph), 
**m** (method),
**' " ( [ {** 

### 4. Действие целиком
- **ciw** &mdash; ("change inner word")
- **ya"** &mdash; yank double-quoted string (include quotes)
- **di(** &mdash; delete text between matching parentheses



#

![](http://uaix.piccy.info/i7/8a828b67ae56b0cd97918f9953d79dc0/4-55-1373/62722653/rsz_vim_shortcuts_dark_2560x1600.png)

# Плагины

- **BufExplorer** &mdash; переключение между буферами
- **CtrlP** &mdash; поиск и открытие файла по шаблону пути
- **NerdTree** &mdash; дерево файлов
- **Snipmate** &mdash; сниппеты кода (Textmate style)
- **Tagbar** &mdash; список символов текущем буфере
- **TComment** &mdash; комментирование кода
- **Vim-Surround** &mdash; обрамление текста кавычками, скобками, тегами

# Конфигурация

Множество файлов vimrc можно найти на Github. Храня свои настройки в репозитории, вы можете легким движением &laquo;приручить&raquo; Vim на любом компьютере.

**Github** &rarr; Search "**vimrc**" &rarr; **8,420** repository results

А также множество цветовых схем.

# Реализации

- Vim
- Gvim
- Macvim

# Vim mode в других программах

- NetBeans ([jvi](http://jvi.sourceforge.net/))
- Eclipse ([vrapper](http://vrapper.sourceforge.net/home/))
- VisualStudio ([ViEmu](http://www.viemu.com/))
- Crhomium ([vimium](http://vimium.github.com/))
- Firefox ([vimperator](http://www.vimperator.org/))

#

## Кстати, на **Github** тоже есть горячие клавиши

- k &mdash; следующий коммит
- j &mdash; предыдущий коммит
- o &mdash; открыть детали коммита

## И в **Gmail**

- k &mdash; к следующей беседе
- j &mdash; к предыдущей беседе
- n &mdash; к следующему сообщению
- p &mdash; к предыдущему сообщению
- o &mdash; открыть беседу


# Материалы

- Неофициальная Vim Wikia [http://vim.wikia.com/wiki/Vim_Tips_Wiki]( http://vim.wikia.com/wiki/Vim_Tips_Wiki )
- Что нужно уметь делать в Vim [https://learn.thoughtbot.com/vim]( https://learn.thoughtbot.com/vim )
- Собрание цветовых схем [http://code.google.com/p/vimcolorschemetest/]( http://code.google.com/p/vimcolorschemetest/ )
- Vim kata &mdash;  вдохновляющее видео [http://vimeo.com/8569257]( http://vimeo.com/8569257 )
- Vim cheat sheet [http://www.viemu.com/a_vi_vim_graphical_cheat_sheet_tutorial.html](http://www.viemu.com/a_vi_vim_graphical_cheat_sheet_tutorial.html)
- Vim movements cheat sheet [https://github.com/EspadaV8/vim_shortcut_wallpaper/](https://github.com/EspadaV8/vim_shortcut_wallpaper/)
- Peepcode Screencasts. Smash into Vim.

