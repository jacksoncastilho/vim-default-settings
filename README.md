# Vim Default Settings

This repository contains a default configuration file for Vim (`.vimrc`) that can be used to enhance your editing experience. The settings provided here are recommended for those who prefer using spaces instead of tabs, automatic indentation, and persistent undo functionality.

## How to Use

1. In your home directory (`~`), create a file named `.vimrc`:

    ```bash
    touch ~/.vimrc
    ```

2. Open the newly created file in Vim:

    ```bash
    vim ~/.vimrc
    ```

3. Copy and paste the following script into the `.vimrc` file:

    ```vim
    set expandtab                    
    " Use spaces instead of tabs "
    set tabstop=4
    " Number of spaces for a tab "
    set shiftwidth=4
    " Spaces used for auto-indent operations "
    set autoindent
    " Enables automatic indentation "
    set smartindent
    " Enables smart indentation for programming languages "
    set cursorline
    " Highlights the current cursor line "
    set number
    " Enables line numbering "
    set undofile
    " Enables persistent undo functionality "
    if !isdirectory(expand("$HOME/.vim/undodir"))
        call mkdir(expand("$HOME/.vim/undodir"),"p")
    endif
    set undodir=$HOME/.vim/undodir
    ```

## Description of the Settings

- `set expandtab`: Replaces the tab character with spaces.
- `set tabstop=4`: Sets the number of spaces equivalent to a tab.
- `set shiftwidth=4`: Defines the number of spaces used for auto-indent operations.
- `set autoindent`: Maintains the indentation of the previous line when creating a new line.
- `set smartindent`: Enables automatic indentation for source code.
- `set cursorline`: Highlights the line where the cursor is located.
- `set number`: Displays line numbers.
- `set undofile`: Enables persistent undo functionality.
- `set undodir`: Configures a directory to store undo files, ensuring that the change history is kept across sessions.

## Note

If the directory `~/.vim/undodir` does not exist, it will be created automatically the first time Vim runs with these settings.

## Contribution

Feel free to suggest improvements or add new settings via pull requests.

## License

This project is under the [MIT License](LICENSE).
