# Hua
Hua is an AI image editor with Stable Diffusion and more (Hua means paint in Chinese).

Website: https://www.PaintHua.com

Discord: https://discord.gg/y9kMYtjgFZ

B站视频: https://www.bilibili.com/video/BV16e4y1a7ne

![](https://raw.githubusercontent.com/BlinkDL/Hua/main/Hua-Demo.gif)

Closed Alpha at this moment. The frontend will be open-source after I finish all major functions and refactor the code, as now it's full of hacks (100% vanilla JS) and very easy to bring in bugs if one don't fully understand it. Meanwhile I will also write a clean & efficient backend for it and that will be open-source from the beginning. 

About me: I am working on https://github.com/BlinkDL/RWKV-LM too, whose training is sponsored by Stability. So you can be assured that Hua is safe :)

## Use Colab

https://colab.research.google.com/github/TheLastBen/fast-stable-diffusion/blob/main/fast_stable_diffusion_AUTOMATIC1111.ipynb
```
!pip install -q inflection

share='--api --cors-allow-origins=https://www.painthua.com'
```
![](https://raw.githubusercontent.com/BlinkDL/Hua/main/colab_guide.png)

## Use your local A1111 server

This is 100% free.

* Update A1111 to LATEST version with git pull.
* In webui-user.bat: 
```
set COMMANDLINE_ARGS=--api --port xxxxx --cors-allow-origins=https://www.painthua.com
```
where xxxxx is a random unoccupied port between 10000 and 60000 (for safety).
* Don't comment "app.user_middleware = ...". The new "--cors-allow-origins" is much safer.
* Open PaintHua config, change 7860 to your number xxxxx, close config to apply.
* Use sd-v1.5-inpainting model (https://huggingface.co/runwayml/stable-diffusion-inpainting) for best results. 
* More A1111 settings: Turn off "Apply color correction to img2img results".
* Run A1111 with --listen to allow LAN access. When connecting to IP other than 127.0.0.1, google "enable mixed content" and change site settings. Because the site is HTTPS but A1111 server is HTTP, so the browser is blocking HTTP requests by default.

Then you can use https://www.PaintHua.com for txt2img / img2img / inpainting / outpainting.

![](https://raw.githubusercontent.com/BlinkDL/Hua/main/Hua-Demo2.gif)

