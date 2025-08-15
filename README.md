# mplStyles
List of my matplotlib styles (`matplotlib` is a graphics/plotting module for Python). All of these were based on the default matplotlib style. For more information on matplotlib styles see [Using style sheets](https://matplotlib.org/stable/users/explain/customizing.html#customizing-with-style-sheets) or [Style sheets reference](https://matplotlib.org/stable/gallery/style_sheets/style_sheets_reference.html).

## How to use
Download any of the .mplstyle files and put them in your matplotlib config directory in the directory with other styles, usually\
`C:\Programy\Python310\Lib\site-packages\matplotlib\mpl-data\stylelib`\
or\
`C:\Users\<user>\AppData\Roaming\Python\Python310\site-packages\matplotlib\mpl-data\stylelib`.\
You can also check your current config directory by running `matplotlib.get_configdir()` in a Python shell. Then just put the styles in a `stylelib` folder  (create one if not present).

Then just include this line in your script\
`plt.style.use("style_name_without_extension")`\
replacing the `style_name_without_extension` with the actual name of the style. For example with a style file named `jkl_thesis_djv.mplstyle` use\
`plt.style.use("jkl_thesis_djv")`.

## Small explanation/notes on my styles
( :star: - my favourite)
- `jkl_thesis_cmu` - style suitable for theses plots; uses serif Computer Modern font; requires having a given TTF file(s) (romanm italic, bold, bolditalic) with CMU Serif font in the matplotlib config directory (`...\matplotlib\mpl-data\fonts\ttf`)
- `jkl_thesis_djv` - style suitable for theses plots; uses serif DejaVu font
- `jkl_thesis_djv_farTicks` - same as `jkl_thesis_djv` but with longer ticks(?)
- `jkl_thesis_djv_sans` :star: - same as `jkl_thesis_djv` but with sans serif version of the DejaVu font
- `jkl_thesis_djv_t` - same as `jkl_thesis_djv` but with transparent background of the plots
