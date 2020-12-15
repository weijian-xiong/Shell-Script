# Web Crawler
 Shell script Project

## Tool installation for this project
1. Debian / Ubuntu Linux install curl, wget, lynx, and w3m
```
sudo apt-get install curl wget lynx w3m
```
2. Install Lynx on Mac with Homebrew
```
brew install lynx
```

The script uses the tool Lynx to download a web page<br>
```
lynx -dump "$target_url"
```
Change permission before compile shell script:
```
chmod 755 web_grep

chmod 755 inverted_index
```

## Project Description
<img width="580" alt="web_grep_question" src="https://user-images.githubusercontent.com/24274444/98777939-37f93b80-23b7-11eb-952f-9b8ed94438fb.png">
<img width="563" alt="Inverted_index_question" src="https://user-images.githubusercontent.com/24274444/98777951-3c255900-23b7-11eb-9c82-ad5386b601f2.png">

## Output
<img width="675" alt="web_grep_output" src="https://user-images.githubusercontent.com/24274444/98777964-40ea0d00-23b7-11eb-852d-a301e454496a.png">
<img width="619" alt="inverted_index_output" src="https://user-images.githubusercontent.com/24274444/98777985-46dfee00-23b7-11eb-8580-3e7c70d22f14.png">

### Difference between lynx and wget tool
For example, we have a html file called jukebox.html.
```
#jukebox.html
<html>
This is a JukeBox.
</html>
```

lynx -dump http://1.2.3.4/jukebox.html<br>
==> return the rendered content
```
This is a Jukebox.
```
wget http://1.2.3.4/jukebox.html<br>
==> return the source code
```
<html>
This is a JukeBox.
</html>
```
