# Nautilus Annotations 
Annotate files and directories

# Details

Long time ago **GNOME Files (Nautilus)** had the ability to handle custom annotations attached to files and directories. This ability has slowly gone lost in the folds of time. Things however are rarely really unlearned, and an ability rarely goes away for good.

**Nautilus Annotations** brings back **Nautilus**' annotation capabilities. It exploits the same machinery that was used back then: that of relying on **GIO** to store custom information about a file or a directory.

Each annotation is stored as a `metadata::annotation` entry in **GIO**'s database. Annotated files are shown in the viewport with an emblem attached.

Thanks to **GIO**, when a file is moved or renamed its annotations remain synchronized with the new path.

## Dependencies

* yad
* xprop
* xdotool

## Install

Clone project:
1. `git clone git://github.com/webmastak/nautilus-annotations`
2. `cd nautilus-annotations`
3. `cp NautilusAnnotation ~/.local/share/nautilus/scripts/yourdir`
7. `cp scripts-accels ~/.config/nautilus`
8. `nautilus -q`
9. `enjoy`


## Usage

Select a file or directory, hotkey dafault `Ctrl+Alt+a` insert the annotation into the content field and save.
Hotkey can be changed to another one in the file `~/.config/nautilus/scripts-accels`
To change the annotation, just change and save. 
To erase an annotation it is sufficient to leave the content blank and save.

## Inspired by

The project [nautilus-annotations](https://github.com/madmurphy/nautilus-annotations)

## Contributing

1. Fork it (<https://github.com/webmastak/nautilus-annotations/fork>)
2. Create your feature branch (`git checkout -b my-new-feature`)
3. Commit your changes (`git commit -am 'Add some feature'`)
4. Push to the branch (`git push origin my-new-feature`)
5. Create a new Pull Request


## Contributors

- [webmastak](https://github.com/webmastak) - creator and maintainer
