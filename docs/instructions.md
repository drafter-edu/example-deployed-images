Instructions for deploying a website using Drafter.

# 1. Update Your website/main.py

Replace the contents of `website/main.py` with your own website file.

You might want to make sure that you call `hide_debug_information` and other setup functions, if you want your site to be deployed without debug information.

```python
from drafter import *
# ...

hide_debug_information()
set_website_title("Your Website Title")
set_website_framed(False)

# ...
start_server()
```

# 2. Include any other files

If your website uses any other files, such as images, CSS, or JavaScript, you should include them in the `website` directory.

# 3. Deploy your website

You can deploy this website via GitHub Pages.

1. Go to the repository `Settings` tab.
2. Click the `Pages` section on the left sidebar.
3. Choose `Github Actions` from the `Source` dropdown box 
4. Wait for the deployment to finish.

You can now access your website at `https://<username>.github.io/<repository-name>`.
