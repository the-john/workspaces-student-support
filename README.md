# workspaces-student-support
Miscellaneous student support files for Udacity students using Workspaces.

Every 30 minutes the remote server that the Udacity Python Notebooks run on will shut down if there is no user interaction.  To keep the CPU/GPU from automatically shutting down after 30 mintues ...

Save workspace_utils.py into your notebook's directory.

Then in your notebook run:

import workspace_utils.py

and use it to wrap your long running code, as shown below:

from workspace_utils import active_session
 
with active_session():
    # do long-running work here
You can also get workspace_utils.py directly from a Jupyter terminal like so:

curl -O https://raw.githubusercontent.com/udacity/workspaces-student-support/master/jupyter/workspace_utils.py

