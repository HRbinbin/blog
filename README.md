# Ray's blog

This is Ray's blog built in Hexo + Github pages. It is published on [ruibinwong.com](https://ruibinwong.com/).

Should update using git bash.



## Create a new post

In git bash, run

```
$ hexo n 'The Blog name'
```



The `blog/source/_posts` folder would generate a markdown file and a image folder with the same name. Write the content in markdown file and put the image file into the image folder.



## Edit the blog

After editing the blog, run

```
$ hexo clean
INFO  Deleted database.
INFO  Deleted public folder.

$ hexo g
INFO  Start processing
...
```

to clean the old statics file and generate the new blogs in `blog/public` folder.



## Preview and deploy

Run 

```
$ hexo s
INFO  Start processing
INFO  Hexo is running at http://localhost:4000 . Press Ctrl+C to stop.
```

to start a local server for previewing the blog. Access it from `http://localhost:4000`.



Run

```
$ hexo d
```

to deploy the blog. Wait a few minutes for Github page updating.



## Add new static file to repository or the page

Since use the [pure theme](https://github.com/cofess/hexo-theme-pure) on the blog, the static files should be added in `blog/source` so the Hexo can generate them every time.



If there is a Markdown file adding in `blog\source` and it should not be rendered, edit `skip_render: filename.md` in `blog\_config.yml`.



The other file like `.png` can be added directly.