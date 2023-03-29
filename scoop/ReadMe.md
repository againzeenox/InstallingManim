# Install `Scoop`
#### 1. Run in powershell
````PS
Set-ExecutionPolicy RemoteSigned -Scope CurrentUser
````
#### 2. Run in powershell
````PS
irm get.scoop.sh | iex
````

# Install `python` + `ffmpeg`

#### Run:
````PS
scoop install python ffmpeg
````

# Install `ManimCE`
#### Run:
````PS
python -m pip install manim
````


# Test ManimCE:
#### 1. Save [this file](https://raw.githubusercontent.com/ManimCommunity/manim/main/example_scenes/basic.py) as `basic.py`
#### 2. Open a cmd line in the directory where `basic.py` is saved
#### 3. Run 
````PS
manim basic.py SquareToCircle -pqm
````

# Install `MikTex`(optional)
## Method 1
#### 1. Run in an administrative terminal
````PS
scoop install latex
````

## Method 2(TinyTex)[PREFERRED]
#### Run in an administrative terminal
````PS
scoop bucket add r-bucket https://github.com/cderv/r-bucket.git
````
then
````PS
scoop install tinytex
 ````
# Installing LaTeX packages
#### After installing TinyTex, Run these 5 commands one after the other
````PS
refreshenv
````
````PS
tlmgr install amsmath babel-english cbfonts-fd cm-super ctex doublestroke dvisvgm everysel
````
````PS
tlmgr install fontspec frcursive fundus-calligra gnu-freefont jknapltx latex-bin
````
````PS
tlmgr install mathastext microtype ms physics preview ragged2e relsize rsfs
````
````PS
tlmgr install setspace standalone tipa wasy wasysym xcolor xetex xkeyval
````
# Testing LaTeX
#### 1. Open a cmd terminal in the directory where `basic.py` is saved
#### 2. Run 
````PS
refreshenv 
````
````python
manim basic.py WriteStuff -pqm
````
