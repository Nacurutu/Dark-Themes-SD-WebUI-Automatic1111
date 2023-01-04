# Dark-Themes-SD-WebUI-Automatic1111-
Custom user.css files for Automatic1111 Stable Diffusion WebUI
#
**Compatible with sd-web-ui-quickcss Extension**

How to use with the extension:

Just clone this repository to the sd-web-ui-quickcss extension root folder.
#
**For more information regarding the extension, please visit this repository:**

https://github.com/Gerschel/sd-web-ui-quickcss

**Thank you very much [Gerschel](https://github.com/Gerschel)**

---

Old method - Not using [Gerschel](https://github.com/Gerschel) sd-web-ui-quickcss Extension:
---
**Custom Dark theme for Stable Diffusion WebUI** 

What you can get with this?

- Changes the dark theme color scheme of your Stable Diffusion WebUI 
- Purely aesthetic changes

```
- Color Scheme: Use predefined styles or Make your own
- Stable Diffusion WebUI Logo
- Stable Diffusion WebUI favicon
- Button backgounds change on Hover
- Button animations on hover
- Focus last interaction
- "Source code pro" text font on inputs
- Change sliders colors
```
-- Custom Dark theme example for Stable Diffusion WebUI screenshot --

**Alani.css**

<img src="https://user-images.githubusercontent.com/18109442/210555304-91405012-d81a-4a42-b9e6-5b20ce9826aa.png" width="75%">


**How to install**

Steps:

- Activate dark mode on the webui-user.bat ->
set COMMANDLINE_ARGS= --theme=dark

- Download and Save the user.css in your Stable Diffusion WebUI's root folder or on \extensions\sd-web-ui-quickcss\style_choices if you are going to use the extension.

   user.css -> https://pastebin.com/frSUF2xN  -_UPDATED -- 01/05/2023_-

- Click on the next image (should open in a new tab)

<img src="https://user-images.githubusercontent.com/18109442/208246354-e80714ab-71e9-48dd-a233-7012bf87335f.png" width="40%">

- Right click on the image 
- Save the image as logo.png in your Stable Diffusion WebUI's root folder

Done. 

---
**Fav Icon**

If you want to change the favicon, you will need to do the following steps:

- Click on the next image (should open in a new tab)

<img src="https://user-images.githubusercontent.com/36368048/196555507-ca0df84e-5fe3-4dbf-9a72-11e8081f16bb.svg" width="10%">

- Right click on the image 
- Save the image as favicon.svg in your Stable Diffusion WebUI's root folder
- If you are going to use the extension, save the logo.png on: extensions/sd-web-ui-quickcss/favicons/
 - Add the favicon updating the webui.py file on line 134 with the following code:

`favicon_path="favicon.svg",`

Example:

```
app, local_url, share_url = demo.launch(
            share=cmd_opts.share,
            server_name="0.0.0.0" if cmd_opts.listen else None,
            server_port=cmd_opts.port,
            debug=cmd_opts.gradio_debug,
            auth=[tuple(cred.split(':')) for cred in cmd_opts.gradio_auth.strip('"').split(',')] if cmd_opts.gradio_auth else None,
            inbrowser=cmd_opts.autolaunch,
            favicon_path="favicon.svg",
            prevent_thread_lock=True
        )
```
---
**Change font:**

Change the font of user inputs and buttons. 
(Didnt change the UI fonts because I prefer to keep the UI and the user inputs with different fonts).

Steps: 

- Download the "Source Code Pro" Family font from here: https://www.fontsquirrel.com/fonts/download/source-code-pro
- Extract SourceCodePro-Regular.otf into your Stable Diffusion WebUI's root folder.
(just in case, install the font -> Right click on the font, then click install)

Done.

---
**Make your own color palette:**

Steps:

Change the color variables on the user.css for the ones you want.

```
*THEME VARIABLES*/
:root, * , quickcss_target{
    
    --Primary_color: #E94822;
    --Secondary_color: #F2910A;
    --Input_text_color: #EFD510;
    --Input_text_color_focus: #ffffff;
    --App_color: #F2910A;
    --Background_color: #2C2D34;
    /*ENDCOLORPICKERS*/
    --UI_radius: 0;
    /*BREAKFILEREADER*/ 
    --logo: url('file=extensions/sd-web-ui-quickcss/logos/logo.png');
    --favicon: url('file=extensions/sd-web-ui-quickcss/favicons/favicon.svg');
 
}
```

The Variables you need to change on the user.css file are:

>  --Primary_color: #------;
>  --Secondary_color: #------;
>  --Input_text_color: #------;
>  --Input_text_color_focus: #------;
>  --App_color: #------;
>  --Background_color------: 


You can use HEX or RGB values. (HEX to be compatible with the Extension)

Note:
Logo and Favicon on Extension folder.
If you are not going to use the extension, change these values:


```
  /*BREAKFILEREADER*/ 
    --logo: url('file=extensions/sd-web-ui-quickcss/logos/logo.png');
    --favicon: url('file=extensions/sd-web-ui-quickcss/favicons/favicon.svg');

```
to these ones (and put the files on the WebUI root folder):

```
  /*BREAKFILEREADER*/ 
    --logo: url('file=logo.png');
    --favicon: url('file=favicon.svg');
```


Done.

---

TO DO:

> - Change the dropdown menu selection color from blue to a new one (it seems that this is handled by the OS and not the browser)
> - Change the Gradio logo animation with this one:

Logo Animation:
<img src="https://user-images.githubusercontent.com/36368048/198925174-eb2f8647-50f1-4a31-8f6f-c32b3e78b3d5.png" width="10%">


Anyone knows how to do anything from the TO DO list? 😉 

Done:

> - ~~Change the font from the user.css file~~ 
> - ~~Change Sliders color from blue to a new one~~

---

> UPDATE -- 12/19/2022 - alpha-v1.01
> 
> - New font for user inputs
> - Minor fixes

> UPDATE -- 12/21/2022 
> 
> - New plugin by @Gerschel - **For the steps, go and check his repository:**
> https://github.com/Gerschel/sd-web-ui-quickcss

> UPDATE -- 12/27/2022 
> 
> - New User.css file:
> - Added Sliders color change
> - user.css code cleaned a little and Variables added for an easier way to change colors (primary, secondary, text input, app borders and background).

> UPDATE -- 01/01/2023 
> 
> - Minor fixes
> - Code cleaned a bit.
> - Added Normalize.css on code:



What is Normalize.css?
A modern, HTML5-ready alternative to CSS resets
[Normalize.css](https://github.com/necolas/normalize.css/) makes browsers render all elements more consistently and in line with modern standards. It precisely targets only the styles that need normalizing.

https://necolas.github.io/normalize.css/


> UPDATE -- 01/05/2023 
> 
> - Minor fixes
> - Code cleaned a bit.

----

> - Thanks to @DarkVamprism, this was made using code from his user.css file posted here on github,
> - Thanks to @ParityError for the Logo 
> - Thanks to @ParityError for the Logo Animation inspired by @Ladypoly
> - Thanks to @masslevel for inspiring this theme color scheme, 
> - Thanks to all the comunity
> - Thanks to @Gerschel for the extension. 
> and
> - Special thanks to Automatic1111 and team members for this great UI.

:wink:

> Disclaimer: 
> I dont know anything about CSS or coding, so, this is a janky alpha version of a CSS file made by try and error that we can use to simulate a dark mode on the Stable Diffusion WebUI.
