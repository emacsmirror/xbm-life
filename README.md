![][image]

## About

An implementation of [Conway's Game of Life] using Emacs' support for
XBM images.  Requires a graphical Emacs instance to run.

## Installation

Install from [Marmalade] or [MELPA (Stable)] via `M-x package-install
RET xbm-life RET`.

Alternatively download the `xbm-life.el` file, open it in Emacs and
execute `M-x eval-buffer`.

## Usage

Run `M-x xbm-life` for the demo.  You can run multiple (mostly)
independent demos along each other by either renaming an existing one
with `M-x rename-buffer` and running `M-x xbm-life` for an additional
one or by perusing `C-u M-x xbm-life` to give the one you launch a
different name.  The timer is global however, therefore all spawned
demos run the same speed and get paused/unpaused at the same time.

You can get an idea of the current details of the demo by taking a
closer look at the modeline where key indicators (such as grid size,
tile size, etc.) are displayed.

Below is a list of useful keybindings for playing around.

| Key bind  | Function                       |
|-----------|--------------------------------|
| l         | Load pattern                   |
| L         | Load random pattern            |
| g         | Reset                          |
| r         | Randomize                      |
| p, SPC    | Toggle play/pause              |
| .         | Advance by a single generation |
| +, -      | Speed up/down                  |
| M-+, M--  | Make tiles larger/smaller      |
| C-+, C--  | Make grid larger/smaller       |
| t         | Toggle wraparound              |
| i         | Invert colors                  |
| <mouse-1> | Toggle cell                    |
| q         | Bury buffer                    |

## Customization

Use `M-x customize-group RET xbm-life RET` for a comprehensive
overview.  Most items listed there influence defaults, such as the
colors used for rendering, the initial pattern and many more.

[image]: img/screencast.gif
[Conway's Game of Life]: https://en.wikipedia.org/wiki/Conway%27s_Game_of_Life
[Marmalade]: https://marmalade-repo.org/
[MELPA (Stable)]: http://melpa.org/
