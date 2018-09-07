# Ubunt Fest 
[![License](https://img.shields.io/badge/license-MIT-blue.svg)](https://opensource.org/licenses/MIT)

> This repository is introduce about Ubuntu Fest(11/10, 2018) - [[Link]](https://ubuntu-kr.github.io/ubuntu-fest)


### Contributing
Please contribute this page if you're interested in helping!

### Reference page
[[HERE]](https://meltingcon.github.io/2018/)

### How to make general repository for gh-pages - [[Link]](https://help.github.com/articles/creating-project-pages-using-the-command-line/)
```bash
$ cd repo

# Creates our branch, without any parents (it's an orphan!)
$ git checkout --orphan gh-pages

# Switched to a new branch 'gh-pages'

# Remove all files from the old working tree
$ git rm -rf .

$ rm '.gitignore'

$ echo "My GitHub Page" > index.html
$ git add .
$ git commit -a -m "First pages commit"
$ git push origin gh-pages

# After change of default branch 

# Delete master branch
$ git push origin :master
```

### Link repository to another repository - [[Link]](http://zeddios.tistory.com/5)
```bash
$ git remote -v
$ git clone --mirror [originally repository URL]
$ git remote set-url --push origin [new repository URL]
$ cd [dir]
$ git push --mirror

# verification 
$ git remote -v
```

### jekyll folder strucure
```
├── _config.yml // for liquid templating language
├── _includes // reusable HTML file with liquid tag
|   ├── btn.html // for nav_registration.md
|   ├── footer.html // footer area
|   ├── nav.html // navigation bar
|   ├── scripts.html // add bootstrap.js
|   └── sponsors.html // viewing sponsors list
├── _layouts
|   ├── frame.html // HTML head area
|   ├── home.html // contents on main page(main-header)
|   └── page.html // ?page-header
├── assets // for page styling
|   ├── css
|   ├── fonts
|   ├── imgs
|   ├── js
|   └── webfonts
├── nav_about.md // 소개
├── nav_contact.md // 문의
├── nav_history.md // 역사
├── nav_location.md // 장소
├── nav_registration.md // 등록 - not use
├── nav_schedules.md // 일정
├── nav_supporters.html // 주최
└── index.md
```
