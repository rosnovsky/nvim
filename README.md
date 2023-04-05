# NvChad Configuration

📝 My `neovim` configuration 

🛠 Includes TypeScript autocomplete, hints, prettier, and more

❤️ Based on [`nvChad`](https://nvchad.com)

![nvim](https://user-images.githubusercontent.com/2508576/230222564-9d18160a-9545-4e21-a0fb-ed89c4ba8105.gif)


## Before you begin

You need a few things installed globally on your machine before you can enjoy the entire setup:

```sh
npm i typescript typescript-language-server prettier --location=global
```

With this out of the way, back up your current `nvim` configuration:

```sh
cd ~/.config
mv nvim nvim_backup
```

Then clone this repo:

```sh
git clone @git@github.com:rosnovsky/nvim
```

## First Run

When you launch `nvim` for the first time now, a bunch of things will happen. 

- It will ask you if you want to install example configuration. Say "no", and be firm about it.
- All the plugins will be automatically installed
- A couple of errors or warnings will appear in the status line (this is normal)

After all is said and done, quit `nvim` (if it's your first time in `vim`/`nvim`, to quit, press `ESC` to ensure you are in `NORMAL` mode, then type `:qa!` and hit `Enter`. This command essentially means "QUIT ALL!" - ignore unsaved files and just follow orders!)

Now launch `nvim` again. This time, a few things will happen in the status line, and it's safe to ignore them. 

In order to make `prettier` work, type this in `NORMAL` mode (remember? `ESC` takes you there):

```vim
:call coc#util#install()
```

This command installs everything necessary for `prettier` to work. After it's all done, restart `nvim` one last time.

Enjoy!
