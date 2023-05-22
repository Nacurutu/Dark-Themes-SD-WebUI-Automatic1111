<h1 align="center">
Project paused until further notice

<br>
<br>

#


<h1 align="center">
	<img src="https://user-images.githubusercontent.com/36368048/196555507-ca0df84e-5fe3-4dbf-9a72-11e8081f16bb.svg" width="100" alt="Logo"/><br/>
	<img src="https://user-images.githubusercontent.com/18109442/210565532-ae64cfbb-b199-48ed-b8f8-036e01a53285.png" height="30" width="0px"/>
	Dark Themes for <a href="https://github.com/AUTOMATIC1111/stable-diffusion-webui">Stable Diffusion Web UI</a>
	<img src="https://user-images.githubusercontent.com/18109442/210565532-ae64cfbb-b199-48ed-b8f8-036e01a53285.png" height="30" width="0px"/>

	
![rainbow-rainbow-bar](https://user-images.githubusercontent.com/18109442/210574757-262e24d2-3ab7-4fa5-bf64-935187bb5c6f.gif)

<p align="center">
	<a href="https://github.com/Nacurutu/Dark-Themes-SD-WebUI-Automatic1111/stargazers"><img src="https://img.shields.io/github/stars/Nacurutu/Dark-Themes-SD-WebUI-Automatic1111?colorA=363a4f&colorB=b7bdf8&style=for-the-badge"></a>
	<a href="https://github.com/Nacurutu/Dark-Themes-SD-WebUI-Automatic1111/issues"><img src="https://img.shields.io/github/issues/Nacurutu/Dark-Themes-SD-WebUI-Automatic1111?colorA=363a4f&colorB=f5a97f&style=for-the-badge"></a>
	<a href="https://github.com/Nacurutu/Dark-Themes-SD-WebUI-Automatic1111/contributors"><img src="https://img.shields.io/github/contributors/Nacurutu/Dark-Themes-SD-WebUI-Automatic1111?colorA=363a4f&colorB=a6da95&style=for-the-badge"></a>
</p>
<br>
<br>

#
<h2 align="left">
What can you get with this?

#
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

- Prefered Browser's zoom at 75% to have a better experience

```
#
Important:

If the changes does not apply properly (Style - logo - favicon), refresh your browser cache:

How to refresh your browser cache?
To force your browser to refresh take the following steps:

> **⇧ Shift-click the Refresh button.** 

While pressing the Refresh button on your browser’s address bar will only do a standard refresh, you can force a refresh from the server by pressing ⇧ Shift and clicking it instead.
<br>
<br>
#

# **Custom Dark theme examples for Stable Diffusion WebUI**

<details>
<summary>🔶 Alani</summary>
<img src="https://user-images.githubusercontent.com/18109442/214368236-c7775dac-b15c-4913-96c5-07340d405717.png"/>
</details>
<details>
<summary>🟣 Neon</summary>
<img src="https://user-images.githubusercontent.com/18109442/214368580-8a4d9d42-a74e-4c1f-87bd-4f3b1dfb7551.png"/>
</details>

#
# **Compatible with sd-web-ui-quickcss Extension**

How to use with the extension:

Just install the Extension. Theme included there.
#
**For more information regarding the extension, please visit this repository:**

https://github.com/Gerschel/sd-web-ui-quickcss

**Thank you very much [Gerschel](https://github.com/Gerschel)**
<br>
 <br>
---

Old method - Not using [Gerschel](https://github.com/Gerschel) sd-web-ui-quickcss Extension:
---

# **How to install**

Steps:

- Activate dark mode on the webui-user.bat ->
set COMMANDLINE_ARGS= --theme=dark

- Download and Save one of the .css files from the repo (style_choices folder) into your Stable Diffusion WebUI's root folder 

- Rename the file to user.css on your SD root folder


or on \extensions\sd-web-ui-quickcss\style_choices if you are going to use the extension (do not need to rename the file names).

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

```java
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

```css
/*THEME VARIABLES*/
:root, * , quickcss_target{
    --Primary_color: #E94822;
    --Secondary_color: #F2910A;
    --Input_text_color: #EFD510;
    --Input_text_color_focus: #ffffff;
    --App_color: #F2910A;
    --Background_color: #2C2D34;
    --Checked_text: #F2910A;
    /*ENDCOLORPICKERS*/
    --UI_radius: 0;
    --left_pannel_width: 40;
    --cards_size: 50;
    /*BREAKFILEREADER*/
    --logo: url('file=logo.png');
    --favicon: url('file=favicon.svg');
    --left-column: calc(20px *var(--left_pannel_width));
}

```

The Variables you need to change on the user.css file are:

-  --Primary_color: #------;
-  --Secondary_color: #------;
-  --Input_text_color: #------;
-  --Input_text_color_focus: #------;
-  --App_color: #------;
-  --Background_color #------: 


You can use HEX or RGB values. (HEX to be compatible with the Extension)

Done.

#

<h2 align="left">
-- UPDATES --

<h4 align="left">

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


> UPDATE -- 01/14/2023 
> 
> - Minor fixes
> - Code cleaned a bit.

> UPDATE -- 01/24/2023 
> 
> - Fixed errors after new webUI updates
> - Added a slider to resize new extra networks cards

----
---

TO DO:

> - Change the dropdown menu selection color from blue to a new one (it seems that this is handled by the OS and not the browser)


Anyone knows how to do anything from the TO DO list? 😉 

Done:

> - ~~Change the font from the user.css file~~ 
> - ~~Change Sliders color from blue to a new one~~

---

# 💙 Big Thanks to:

> - @DarkVamprism, @masslevel, nectar9000 and @vladmandic, this was made using some code from their user.css files posted here on github
> - @ParityError for the Logo and Logo Animation inspired by @Ladypoly
> - @masslevel for inspiring the Neon color palette 
> - All the community
> - @Gerschel for the extension. 

> - Special thanks to Automatic1111 and team members for this great UI.
 <br>
 <br>
<h3 align="center">
🌟🌟🌟🌟🌟🌟🌟🌟🌟🌟🌟🌟🌟🌟
 <br>
 <br>
 <h4 align="left">
> Disclaimer:
<br>
> I dont know anything about CSS or coding, so, this is a janky alpha version of a CSS file made by try and error that we can use to simulate a dark mode on the Stable Diffusion WebUI.

<h4 align="center">

![945617](https://user-images.githubusercontent.com/18109442/210566056-30b34c73-ed79-48d9-b04f-da781905d709.gif)

#

<h4 align="center">
<img src="https://user-images.githubusercontent.com/18109442/210567328-412e1903-5126-4ebf-a3cc-1c58a2fc30f6.png" width="100" alt="Logo"/><br/>
	
