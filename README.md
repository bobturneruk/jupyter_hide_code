# Jupyter served via Binder with hide_code extension

[![Binder](https://mybinder.org/badge_logo.svg)](https://beta.mybinder.org/v2/gh/fomightez/jupyter_hide_code/master?filepath=index.ipynb) 

Jupyter notebook environment with the [hide_code extension](https://github.com/kirbs-/hide_code) active upon session launch. **No installation needed**.

Click a `launch binder` badge anywhere on this page to begin.

-----

## Technical details:

This was a rather tricky extension to get working in sessions served from MyBinder.org/Binder. Solution based mainly on [here](https://stackoverflow.com/a/39169844/8508004) and [here](https://github.com/binder-examples/jupyter-extension/blob/1fecbd818ef84980ec1043e4b57edebf7053d1f9/postBuild).

serverproxy wasn't necessary for noteboook with hidden code to HTML when using the hide code menu on the toolbar. Is it necessary to go to pdf which looks like it uses URL as part of process? I 'll need to explore that next after realizing all this time I probably wasn't installing wkhtmltopdf because had not added to commit `apt.txt` until just now. It wasn't there when I was testing pdf export earlier. Should have better luck now.  

-----

[![Binder](https://mybinder.org/badge_logo.svg)](https://beta.mybinder.org/v2/gh/fomightez/jupyter_hide_code/master?filepath=index.ipynb) 
