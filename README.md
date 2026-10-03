![version badge](https://img.shields.io/github/v/release/Meikul/obsidian-thumbnails)
![downloads badge](https://img.shields.io/github/downloads/Meikul/obsidian-thumbnails/total.svg)
# Obsidian Thumbnails
This plugin lets you insert video thumbnails into your notes to help you keep track of what you're actually linking.

Works with Youtube and Vimeo.
<img src="https://raw.githubusercontent.com/Meikul/obsidian-thumbnails/master/demo_images/block_demo.gif" alt="GIF showing how to create a thumbnail with the plugin">

## Installation
### Community plugins
Search for "Thumbnails" in **Settings → Community plugins → Browse**.

### BRAT (beta / this fork)
To install this fork, which includes Insert Thumbnail on Paste, use [BRAT](https://github.com/TfTHacker/obsidian42-brat):
1. Install and enable **BRAT** from **Settings → Community plugins → Browse**.
2. Open the command palette and run **BRAT: Add a beta plugin for testing**.
3. Enter `https://github.com/coreyx/obsidian-thumbnails` and click **Add Plugin**.
4. Enable **Thumbnails** in **Settings → Community plugins**.

BRAT will keep the plugin updated with new releases from this repository. This fork uses the same plugin ID as the community version, so installing it through BRAT replaces the community version.

## Usage
Paste a YouTube or Vimeo link into a note, and the thumbnail code block is created for you

***OR***

Use the "Insert thumbnail from URL in clipboard" command

***OR***

Manually place a code block with the `vid` type, and include the link to your video:
````markdown
```vid
https://youtu.be/dQw4w9WgXcQ
```
````
## Paste to Insert
Pasting a YouTube or Vimeo link into a note automatically wraps it in a `vid` code block, just like the "Insert thumbnail from URL in clipboard" command.

Normal pasting is kept when:
- The clipboard holds anything other than a single video link
- Text is selected (so Obsidian's paste-link-over-selection still works)
- The cursor is inside a code block

If the cursor is in the middle of a line, the code block is placed on its own lines so it renders correctly. This can be turned off with the **Insert Thumbnail on Paste** setting.

## Commands
### Insert thumbnail from URL in clipboard
If you have a video URL in your clipboard, this command will create the code block for you.

### Insert video title link from URL in clipboard
If you have a video URL in your clipboard, this command will automatically create a link with the text set to the video title.

<img src="https://raw.githubusercontent.com/Meikul/obsidian-thumbnails/master/demo_images/title_link_demo.gif" alt="GIF demonstrating the insert video title link command" width="480">

## Offline Settings
### **Save Thumbnail Info**
<span style="opacity:0.65">Default: Enabled</span><br/>
When offline, thumbnails will have blank images but still show the title and channel.
### **Save Images**
<span style="opacity:0.65">Default: Disabled</span><br/>
Store your thumbnail images locally in a location you specify.

## Paste Settings
### **Insert Thumbnail on Paste**
<span style="opacity:0.65">Default: Enabled</span><br/>
Automatically insert a thumbnail code block when pasting a YouTube or Vimeo link.
