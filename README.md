#Who are we?

* Ely Flores



* Fernando Montes


#Agenda
1. Intro
2. The tools
3. Setup
4. Coding time
    * Create base site
    * Personalize!
5. Publish to Github pages
    

##Intro
1. What are we going to do?
2. What is the expectation?
3. What is the motivation?


##The tools
1. [Git](https://git-scm.com/)
2. [Github](https://github.com/)
3. [Hugo](http://gohugo.io/)
4. [Github Pages](https://pages.github.com/)
5. [Markdown](https://guides.github.com/features/mastering-markdown/)
6. Any text editor


##Setup
1. Install Git (https://git-scm.com/downloads)
2. Install Hugo (http://gohugo.io/overview/installing/)


##Coding Time
### Create base site
2. Create a Github repository (e.g. my-profile-com-mx)
3. git clone `github_repository_url`
3. cd `github_repository_folder`
2. hugo new site mysite 
3. cd mysite
4. git clone https://github.com/gcushen/hugo-academic.git themes/academic
5. cp -av themes/academic/exampleSite/* .
    * Copy the example site from themes/academic into current directory, this will give us our base site to work on.
6. hugo server --watch
7. Site must be accessible at this URL: http://localhost:1313/

### Personalize!
1. Personalize your name (mysite/config.toml)
2. Personalize your picture (mysite/static/img/portrait.jpg)
3. Update personal data (mysite/config.toml)
    * e.g. [[params.social]]
4. Update the sections you would like to include
    * [[menu.main]]
5. Update the content of your site

###Publish to Github Pages

1. Modify mysite/config.toml file to add the lines that will allow your site to be published.
2. Make sure all your latest changes are committed and pushed.
3. git checkout --orphan gh-pages
4. git rm --cached $(git ls-files)
5. git checkout master README.md
6. git add .
7. git commit -m "INIT: initial commit on gh-pages branch"
8. git push origin gh-pages
9. git checkout master
10. rm -rf public
11. git subtree add --prefix=public `repo_url` gh-pages --squash
12. git subtree pull --prefix=public `repo_url` gh-pages
13. cd mysite
14. hugo -t "academic"
15. cd ..
16. mv mysite/public .
17. git add -A
18. git commit -m "Updating site" && git push origin master
19. git subtree push --prefix=public `repo_url` gh-pages


## References
* http://gohugo.io/tutorials/github-pages-blog/
* https://pages.github.com/
* http://themes.gohugo.io/academic/
* https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet
* http://codethejason.github.io/blog/setupghpages/