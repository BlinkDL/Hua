# Hua
Hua is an AI image editor with Stable Diffusion and more (Hua means paint in Chinese).

Website: https://www.PaintHua.com

Discord: https://discord.gg/y9kMYtjgFZ

Closed Alpha at this moment. The JS will be fully open-source afterwards.

## How to use

This is 100% free.

* Run LATEST (!!!) https://github.com/AUTOMATIC1111/stable-diffusion-webui with --api (will listen at 127.0.0.1:7860 by default). That is, "set COMMANDLINE_ARGS=--api" in webui-user.bat.
* Use sd-v1.5-inpainting model (https://huggingface.co/runwayml/stable-diffusion-inpainting) for best results.
* Run A1111 with --listen to allow LAN access.
* When connecting to IP other than 127.0.0.1, google "enable mixed content" and change site settings. Because the site is HTTPS but A1111 server is HTTP, so the browser is blocking HTTP requests by default.

Then you can use https://www.PaintHua.com for txt2img / img2img / inpainting / outpainting.

![](https://raw.githubusercontent.com/BlinkDL/Hua/main/Hua-Demo.gif)
