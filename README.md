# VIM / NEOVIM: The beginner's guide

## Table of Contents

- [Start, save and exit](#sse)
  - [Start Vim / Neovim](#start)
- [Move operators](#moveOperators)
  - [Save and exit Vim / Neovim](#saveAndExit)
- [Modes](#modes)
  - [Normal mode](#normalMode)
  - [Insert mode](#insertMode)
- [Move operators](#moveOperators)

### Start, save and exit<a name="sse"></a>

#### Start Vim / Neovim<a name="start"></a>

| command | action       |
| :-----: | :----:       |
| `vim`   | Start Vim    |
| `nvim`  | Start Neovim |

#### Save and exit Vim / Neovim<a name="saveAndExit"></a>  

| command    | action            |
| :-----:    | :----:            |
| `:w`       | save              |
| `:q`       | quit              |
| `:q!`      | quit without save |

### Move operators<a name="moveOperators"></a> 

| command   | action    |
| :-----:   | :----:    |
| `h`       | left      |
| `j`       | down      |
| `k`       | up        |
| `l`       | right     |
| `w`       | next word |
| `e`       | end word  |
| `b`       | back word |

### Modes<a name="modes"></a>

| command    | mode         |
| :-----:    | :----:       |
| `esc`      | normal       |
| `i`        | insert       |
| `:`        | command      |
| `v`        | visual       |
| `shift + v`| visual line  |
| `ctrl + v` | visual block |

#### Normal mode<a name="normalMode"></a>

##### Main actions

| command     | action          |
| :-----:     | :---:           |
| `%`         | go to pair      |
| `o`         | new line        |
| `shift + o` | new above line  |
| `r`         | replace char    |
| `shift + r` | replace several |
| `%`         | go to pair |
| `%`         | go to pair |
| `%`         | go to pair |

##### Numbers operations

You can combine the numbers and move operators.
For example:

| command              | action                       |
| :-----:              | :---:                        |
| `number + j`         | go to next relative line     |
| `number + k`         | go to previous relative line |
| `number + shift + g` | go to line                   |
| `number + w`         | go to word                   |
| `number + d + w`     | delete number of word        |

##### Action operations

You can combine the move and action operators.
For example:

| command      | action                       |
| :-----:      | :---:                        |
| `c + i + w`  | change word                  |
| `d + w`      | delete word                  |
| `d + b`      | delete back word             |
| `d + 0`      | delete                       |
| `shift + d`  | delete                       |

##### copy, cut and paste

**Note:** delete action don't exist in Vim, for this use the cut action

| command     | action             |
| :-----:     | :---               |
| `y`         | copy               |
| `yy`        | copy line          |
| `x`         | cut                |
| `dd`        | cut line           |
| `p`         | paste              |
| `shift + p` | paste above line   |

##### undo and redo

| Comando   | Acción      |
| :-----:   | :----:      |
| `d+w`     | delete word |
| `u`       | undo        |
| `ctrl+r`  | redo        |

##### start or end of document

| Comando   | Acción            |
| :-----:   | :----:            |
| `g+g`     | start of document |
| `shift+g` | end of document   |

##### timeline

| Comando   | Acción    |
| :-----:   | :----:    |
| `g+d`     | go to definition | d = definition
| `g+f`     | go to file       | d = definition
| `ctrl+o`  | acción anterior| o = older
| `ctrl+i`  |acción posterior |

#### Insert mode<a name="insertMode"></a>

##### Enter to insert mode

| Comando   | Acción                              |
| :-----:   | :----:                              |
| `i`       | insert to left                      |
| `I`       | insert to start of the current line |
| `a`       | insert to right                     |
| `A`       | insert to end of the current line   |

#### Command mode<a name="commandMode"></a>

##### Search 

| Comando     | Acción         |
| :-----:     | :----:         |
| `:/ + text`  | search to next |
| `:? + text`  | search to back |
| `n`         | search next    |
| `shift + n` | search next    |

#### Comand mode

:s/texto a reemplazar/texto nuevo /g -> en caso de querer reemplazar todas las concurrencias de la línea.

:%s/texto a reemplazar/texto nuevo -> reemplaza todas las concurrencias de lal archivo


### Autor

- [@isturiz](https://www.github.com/isturiz)

