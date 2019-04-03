# Slack dark theme injector tool
This tool writes a dark theme to mimic Discord on the Slack desktop application.

### Preview:

![Sample screenshot of dark Slack theme](TODO)

### Prerequisites

Install [python](https://www.python.org/)

You _really_ should take the css file from this site, and host it somewhere _you_ control. It's
not a great idea to have a script inject an arbitrary CSS file from a domain outside of your control,
into an application like Slack that could have sensitive data.

Don't trust me - fork the repo.

### Running

Unix
```bash
sudo python makeitdark.py
```
```bash
sudo python3 makeitdark.py
```

Windows
```bash
python makeitdark.py
```
### Sidebar

Matching Discord-themed sidebar:
```
#2C2F33,#252525,#4d4d4d,#D2D6D6,#4D4D4D,#DEDEDE,#ADBA4E,#DB6668
```
You can fiddle around with custom sidebar themes at https://slackthemes.net

### Reverting

If you want to uninstall the dark Slack theme you can run with the `makeitlight` option:
```
makeitdark.py makeitlight
```

### Slack Updates

When Slack updates it will overwrite the installed dark theme. When this happens just re-run the tool to make it dark again.

## Authors

* **James Szklarz** - *Initial work* - [LostConnection](https://github.com/LostConnection)
* **Andrew Hayworth** - *Darkreader updates* - [ahayworth](https://github.com/ahayworth)
* **devrism** - *Discord theme fork* - [devrism](https://github.com/devrism/)

See also the list of [contributors](https://github.com/LostConnection/makeitdark/contributors) who participated in this project.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details

## Acknowledgments

* Authors of js injection code used
* [Original dark css used](https://github.com/laCour/slack-night-mode)
