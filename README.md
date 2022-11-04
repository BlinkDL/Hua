# Hua
Hua is an AI image editor with Stable Diffusion and more (Hua means paint in Chinese).

Website: https://www.PaintHua.com

Discord: https://discord.gg/y9kMYtjgFZ

Closed Alpha at this moment. The frontend will be open-source after I finish all major functions and refactor the code.

Now it's full of hacks (100% vanilla JS) and very easy to bring in bugs if one don't fully understand it.

Meanwhile I will also write a clean & efficient backend for it and that will be open-source from the beginning.

## How to use

This is 100% free.

### NOTE: Latest A1111 commit breaks PaintHua: https://github.com/AUTOMATIC1111/stable-diffusion-webui/commit/5f0117154382eb0e2547c72630256681673e353b
### You can manually comment out the "app.user_middleware = xxxx" line in webui.py to solve it.

* Run https://github.com/AUTOMATIC1111/stable-diffusion-webui with --api (will listen at 127.0.0.1:7860 by default). That is, "set COMMANDLINE_ARGS=--api" in webui-user.bat.
* Use sd-v1.5-inpainting model (https://huggingface.co/runwayml/stable-diffusion-inpainting) for best results. 
* More A1111 settings: Turn off "Apply color correction to img2img results".
* Run A1111 with --listen to allow LAN access. When connecting to IP other than 127.0.0.1, google "enable mixed content" and change site settings. Because the site is HTTPS but A1111 server is HTTP, so the browser is blocking HTTP requests by default.

Then you can use https://www.PaintHua.com for txt2img / img2img / inpainting / outpainting.

![](https://raw.githubusercontent.com/BlinkDL/Hua/main/Hua-Demo.gif)

![](https://raw.githubusercontent.com/BlinkDL/Hua/main/Hua-Demo2.gif)
