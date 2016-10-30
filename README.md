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


## References
1. http://gohugo.io/tutorials/github-pages-blog/
2. https://pages.github.com/
3. http://themes.gohugo.io/academic/
4. https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet