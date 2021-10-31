Website-http://instapresent1.000webhostapp.com or http://instapresent.tech

# InstaPresent

This tool was built by Tanay and Gaurab

For more info, check out [our devpost](https://devpost.com/software/instapresent)

# How to run

This project requires two processes to run.

First, `git clone` our repository.

Then, create the virtualenv:

```bash
python3 -m pip install virtualenv
mkvirtualenv hack --python 3.6
source ~/hack/bin/activate
pip install -r ~/impromPPTX/reqs.txt
```

Then, open up tmux and run two sessions:

tmux pane 1:

```bash
cd ~/impromPPTX/data
source ~/hack/bin/activate
python3 server.py (requires restart on changes made to main_function.py)
```

tmux pane 2:

```bash
cd ~/impromPPTX/
source ~/hack/bin/activate
python3 manage.py runserver (does not require restart)
```
