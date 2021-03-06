# transQiita
This application translates your articles on Qiita into English ones with googletrans, and 
upload them to Qiita automatically. 

## Requirements
[googletrans](https://pypi.org/project/googletrans/), Qiita access token(Set as Environment variable QIITA_ACCESS_TOKEN)
    
```
e.g.
$ pip install googletrans
$ export QIITA_ACCESS_TOKEN='YOUR QIITA ACCESS TOKEN'
```

## Example

```
$ python transQiita.py  [-h] [--gist] [--tweet] [--private] [--auto] [--token TOKEN]
```

## Optional Arguments

```
-h, --help     show this help message and exit
--gist         upload translated article to gist
--tweet        tweet about translated article
--private      set publish format to private
--auto         execute translation and upload automatically
--token TOKEN  set Qiita's access token
```

## Restrictions
1. **This application does not translate code blocks to prevent indentation from collapsing by translation process.**
2. **Decoration by markdown using symbols like ** , ~~ etc. does not work after translation process.**

## Anything Else
I wrote an article below to explain this application more in details.

https://qiita.com/speaktech/items/f1c47ab15c17d873fd03

# Author
[speaktech](https://qiita.com/speaktech)

# License
[MIT](./LICENSE)
