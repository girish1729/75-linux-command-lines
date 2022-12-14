# 50 interesting Linux command lines

1. Convert CRLF terminated files to just CR

```shell
$ dos2unix file.txt
```

2. Check if JSON is valid

```shell
$ json_verify < file.json
```

3. Same as above but prints out nicely.

```shell
$ jq < file.json
```

4. Get rid of duplicate spaces occuring together

```shell
 $ tr -s ' ' < file.txt
```

5. Send mail from command line

```shell
$ mutt -s hi foo@yahoo.com < /tmp/mail.txt
```

6. Move in bulk based on patterns

```shell
$ mmv -v '*' '#1.jpg'
```

7. Use interactive file deletion DOS style
	(midnight commander DOS style UI)

```shell
$ mc
```


8. Fancy list files (show dirs with /)

```shell
$ ls -F
```

9. Show a file with line numbers

```shell
 $ cat -n file.txt
```

10. Use cut to split fields

```shell
 $ echo 1:2:3 | cut -d: -f2
```

11. Edit file in place and do search and replace

```shell
 $ perl -pi -e 's/old/new/' file.txt
```

12. Same as above but not in place

```shell
 $ sed -e 's/old/new/' file.txt > new.txt
```

13. Spidermonkey (interactive js shell)

```shell
$ js 
```

```shell
$ node
```

14. Simple video to audio conversion

```shell
 $ ffmpeg -i file.mp4 song.mp3
```
15. Download youtube video to disk

```shell
 $ youtube-dl https://youtu.be/XXXX
```

16. Same as above, faster

```shell
 $ yt-dlp https://youtu.be/XXX
```

17. Show progress bar or ETA with pipeviewer

```shell
 $ cat file.tgz | pv | tar zxpf
```

18. Play gif animation

```shell
 $ mplayer file.gif
```

19. View image

```shell
 $ qiv file.jpg
```

20. Same as above

```shell
 $ qview file.webp
```

21. Same as above

```shell
 $ xloadimage file.png
```

22.  Same as above

```shell
 $ display file.png
```


23. Nice PDF viewer

```shell
 $ mupdf file.pdf
```

24. Fire up a web server using current dir

```shell
 $ http-server
```

25. Fire up web server to interpret markdown files

```shell
 $ grip
```

26. Do a simple file upload to FTP or HTTP

```shell
 $ curl -T file.input ftp://remote/dir/A
```

27. Do a fast download breaking file into chunks and fetch 
    using multiple TCP connections

```shell
 $ axel <URL>
```

28. Figure out common lines

```shell
 $ comm file.txt file2.txt
```

29. Compare binary files

```shell
 $ diff a.bin b.bin
```

30.  Printout SHA256 fingerprint

```shell
 $ openssl dgst sha256 < file.txt
```

31. Same as above.

```shell
sha256sum < file.txt
```

32. Always import fresh into git repo

```shell
 $ find . -name .git | xargs rm -rf
```

33. Hear same song repeatedly

```shell
 $ mplayer favsong.mp3 -loop 0
```

34. Watch video with vol boost, 0,9 for +,-

```shell
 $ mplayer -softvol -softvol-max 1000 file.mp4
```

35. Listen to Internet radio on command line

```shell
 $ mplayer <shoutcast url>
```

36. Resize image with ImageMagick

```shell
 $ convert file.png -resize 500x500! small.png
```

37. Find out width and height

```shell
 $ identify favicon.ico
```

38. Tell the length of media

```shell
 $ mplayer -identify -frames 0 <media>
```

39. Nuke everthing in mp3 after 90 seconds

```shell
 $ ffmpeg  -i file.mp3 -to 90 out.mp3
```

40. Get rid of first 30 seconds.

```shell
 $ ffmpeg -i file.mp3 -ss 30 out.mp3
```

41. Convert a postscript file to PDF

```shell
 $ ps2pdf14 file.ps
```

42. Create webp from png or jpg

```shell
 $ cwebp file.png -o file.webp
```

43. Change image format

```shell
 $ convert file.jpg file.png
```

44. Copy file.txt to paste buffer

```shell
 $ cat file.txt| xsel
```

45. Take screenshot from command line

```shell
 $ import f.png
```

46.  Scour entire file system for files

```shell
 $ locate file
```

47. Look for pattern recursively and ignore case

```shell
 $ grep -ir pat dir/
```

48. Get rid of newline whilst printing

```shell
 $ echo -n text
```

49. Batch top output

```shell
 top -b
```

50. Show speed of download/upload

```shell
$ ifstat
```
51. Find directories and nuke them

```shell
$ find . -name mango -type d | xargs rm -rf
```

52. Prints random quote or cookie

```shell
$ fortune
```

53. Compress files using zstd
```shell
$ zstd file.bin
```

54. Decompress using zstd
```shell
$ unzstd compressed.zstd
```

55. Record screencast video
```shell
$ peek
```

56. Download youtube video in mp4
```shell
$ yt-dlp -f mp4 https://youtu.be/XXXXX
```

57. FTP client with superpowers
```shell
$ lftp <URL>
```

58. Show statistics and counters
```shell
$ conky
```

59. Show bandwidth usage
```shell
$ ifstat -b
```

60. Start a TCP server at port 1234
```shell
$ nc -l -p 1234
```

61. Connect to server using netcat
```shell
$ nc 127.0.0.1 1234
```

62. Generate strong password
```shell
$ pwgen
```

63. Generate lookalike domains
```shell
$ dnstwist google.com
```

64. anagram generator
```shell
$ an mango
```

65. Profile execution of a program
```shell
$ time <cmd>
```

66. Save changes to disk
```shell
$ sync
```

67. Figure out USB or SSD or HDD performance
```shell
$ iostat
```

68. Find out bandwidth between two point
```shell
$ bing host1 host2
```

69. Scan for machines in local network
```shell
$ fping -g 192.168.1.0/24
```

70. Colored less
```shell
$ most <file>
```

71. JSON power tool
```shell
$ jq
```

72. YAML power tool
```shell
$ yq
```

73. Search for man pages
```shell
$ apropos string
```

74. Indent javascript
```shell
$ js-beautify file.js
```

75. Capture screenshot
```shell
$ sleep 3; import foo.png
```


## Download this cheatsheet PDF

[Gumroad download](https://girish1729.gumroad.com/l/50-linux-command-lines)

## Tweet this to your followers


<a href="https://twitter.com/intent/tweet?text=Tweet+this&url=https%3A%2F%2Fgithub.com%2Fgirish1729%2F50-linux-command-lines&hashtags=twitter&original_referer=http%3A%2F%2Fgithub.com%2F&tw_p=tweetbutton" target="_blank">
  <img src="http://jpillora.com/github-twitter-button/img/tweet.png"
       alt="tweet button" title="Tweet this"></img>
</a>
