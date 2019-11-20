<img alt="image" src="https://avatars3.githubusercontent.com/u/54864194?s=460&v=4" width="75px">
Project by doOnline.

# webm-convert
webm-convert is a video-converter binary which requires ffmpeg 4.0+. Used to convert all video formats & codecs which are not compatible with HTML5 on most browsers and machines to be converted to the .webm format with the most optimal speed/quality.

## Required packages:
+ ffmpeg version 4.0 or higher.

## Install
Step 1 (Cloning git repository):
```
git clone https://github.com/DoOnlineNL/webm-convert.git;
```
Step 2 (Make executable and run):
```
chmod a+x ./webm-convert/webm-convert && ./webm-convert/webm-convert;
```
Step 3 (Create symlink as non-root/root):
```
path=$(echo "`readlink -f -- $(dirname -- $0)`/webm-convert") && cd /usr/bin && sudo mv "${path}"/webm-convert ./webm-convert && cd "${path}"/../;
```
Step 4 (Test the symlink, it should work troughout the whole server without selecting the installed sshfs-mount file)
```
webm-convert && echo -n "Successfully installed webm-convert, Cleaning download directory now..." && sudo rm -r webm-convert/ && echo -n "Finished installing webm-convert for this user. Please visit https://doonline.nl/ for more of this good stuff...";
```

## License
Project is licensed under MIT License

Copyright 2017 doOnline at https://doonline.nl

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), 
to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, 
and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF 
MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR
ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE
SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
