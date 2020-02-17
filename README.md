# Jupyter served via Binder with hide_code extension

[![Binder](https://mybinder.org/badge_logo.svg)](https://beta.mybinder.org/v2/gh/fomightez/jupyter_hide_code/master?filepath=index.ipynb) 

Jupyter notebook environment with the [hide_code extension](https://github.com/kirbs-/hide_code) active upon session launch. **No installation needed**.

hide_code is a Jupyter notebook extension to selectively hide code, prompts and outputs with PDF and HTML exporting support.

Click a `launch binder` badge anywhere on this page to begin.

-----

**Note: `Export to PDF via Latex` button on the far right side of the `hide_code` toolbar doesn't work here.** (ohhh, realized via a recent pull request [here](https://github.com/kirbs-/hide_code/pull/83) that links to [issue#65](https://github.com/kirbs-/hide_code/issues/65) that the button for that has been bugged for a while now.) All other features, such as `Export to PDF via HTML`, are working.

## Technical details:

This was a rather tricky extension to get working in sessions served from MyBinder.org/Binder. Solution based mainly on [here](https://stackoverflow.com/a/39169844/8508004) and [here](https://github.com/binder-examples/jupyter-extension/blob/1fecbd818ef84980ec1043e4b57edebf7053d1f9/postBuild). Getting export to PDF working from the `hide_code` toolbar required enabling wkhtmltopdf to work headlessly similar to had been done for Plotly Orca as I described [here](https://discourse.jupyter.org/t/using-plotlys-orca-to-generate-static-plots-in-binder-served-sessions/1232/4?u=fomightez). serverproxy wasn't necessary for noteboook with hidden code to HTML when using the hide code menu on the toolbar pr for expoer to PDF from same toolbar. 

`Export to PDF via Latex` button on the far right side of the `hide_code` toolbar doesn't work. I didn't try looking into what is necessary for that. **The `Export to PDF via HTML` button does work.** UPDATE: Realized via a recent pull request [here](https://github.com/kirbs-/hide_code/pull/83) that links to [issue#65](https://github.com/kirbs-/hide_code/issues/65) that the button for that has been bugged for a while now.

still to do:
- make better demo notebook since that was just a placeholder and while widgets do seem to render it would be nice to have a non-widgest plot there too. Do dataframes work? (if so, would be nice to point out over on dataframe2image as easier route/related route if just need to make a document with a dataframe showing). Was there a good one at the hide_code repo?  ==> YES. See [demo.ipynb](https://github.com/kirbs-/hide_code/tree/2508c28a065d99143e463837f7885c74e754dc1b)) in the development branch ([dev branch](https://github.com/kirbs-/hide_code/blob/dev/demo.ipynb)) is the one used to make the animation amd should step through that to illustrate use. Copied that one used to make the animation into rep for now as `demo.ipynb`.
- for original repo and port all this over there and make a pull request noting that the badge URL would need fixing after the pull.


-----

[![Binder](https://mybinder.org/badge_logo.svg)](https://beta.mybinder.org/v2/gh/fomightez/jupyter_hide_code/master?filepath=index.ipynb) 
