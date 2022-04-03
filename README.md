# SABnzbd-Linux-Build

SABnzbd - The automated Usenet download tool
============================================

SABnzbd is an Open Source Binary Newsreader written in Python.

It's totally free, easy to use, and works practically everywhere.
SABnzbd makes Usenet as simple and streamlined as possible by automating everything we can. All you have to do is add an `.nzb`. SABnzbd takes over from there, where it will be automatically downloaded, verified, repaired, extracted and filed away with zero human interaction.
SABnzbd offers an easy setup wizard and has self-analysis tools to verify your setup.

If you want to know more you can head over to our website: https://sabnzbd.org.

## Resolving Dependencies

SABnzbd has a few dependencies you'll need before you can get running. If you've previously run SABnzbd from one of the various Linux packages, then you likely already have all the needed dependencies. If not, here's what you're looking for:

- `python` (Python 3.7 and above, often called `python3`)
- Python modules listed in `requirements.txt`. Install with `python3 -m pip install -r requirements.txt -U`
- `par2` (Multi-threaded par2 installation guide can be found [here](https://sabnzbd.org/wiki/installation/multicore-par2))
- `unrar` (make sure you get the "official" non-free version of unrar)

Optional:
- See `requirements.txt`

Your package manager should supply these. If not, we've got links in our [installation guide](https://github.com/sabnzbd/sabnzbd/blob/master/INSTALL.txt).

## Running SABnzbd from source

Once you've sorted out all the dependencies, simply run:

```
git clone https://github.com/sabnzbd/sabnzbd.git
cd sabnzbd
python3 -OO SABnzbd.py
```

Or, if you want to run in the background:

```
python3 -OO SABnzbd.py -d -f /path/to/sabnzbd.ini
```

If you want multi-language support, run:

```
python3 tools/make_mo.py
```

Our many other command line options are explained in depth [here](https://sabnzbd.org/wiki/advanced/command-line-parameters).
