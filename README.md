#Who are we?

* Ely Flores
    * Software Engineer @ [Nearsoft](http://nearsoft.com/)
    * UABC / ENSEIRB
    * Code. Java. Web. Star Wars. Books. Coffee. Wine. Love.

* Fernando Montes
    * Senior Software Engineer @ [Nearsoft](http://nearsoft.com/)
    * ITESM - CEM
    * Code. Web. Videogames. Books. Coffee. Wine. Love

#Agenda
1. Intro
2. The tools
3. Setup
4. Coding time
    * Create base site
    * Personalize!
5. Publish to Github pages
6. What is next?
    

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
3. Create a new repo where your site will be published (`username.github.io`)
4. Clone that repo in a separate folder (different from `my-profile-com-mx`)
5. cd `my-profile-com-mx/mysite`
6. hugo -t "academic"
7. cd ..
8. mv mysite/public/* ../username.github.io/
9. cd `username.github.io`
10. git add -A
11. git commit -m "Publish site"
12. git push
13. Repeat steps from 5 to 12 to update / re-publish your site. 

## What is next?

* This is the start of a new path for you. Use your power wisely. 
* We recommend you to visit: https://gohugo.io/ to learn more about Hugo. 
* We used the _Academic_ theme for the purposes of this workshop, go ahead
 and visit http://themes.gohugo.io/ to see more sites or even better, create your own theme!
* Continue adding content, keep your site updated! Anything you learn, 
go ahead and publish it! You never know who will read it and find it useful!
* Be Happy & keep learning new things :-)

## References
* http://gohugo.io/tutorials/github-pages-blog/
* https://pages.github.com/
* http://themes.gohugo.io/academic/
* https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet
* http://codethejason.github.io/blog/setupghpages/

## Want know more about Nearsoft?

* Visit http://nearsoft.com/about/
* http://nearsoft.com/join-us/
* Nearsoft Jobs: https://github.com/Nearsoft/jobs
* Looking for a Nearsoftian? Visit [this map](https://www.google.com/maps/d/u/0/viewer?mid=163yqvS6x2ZPFca0FJyMCwrVlnKY)

## Contact us:

* Ely:
    * [Personal site](http://lapetiteensenadoise.com)
    * [Github](https://github.com/elifloresch)
    * [Twitter](https://twitter.com/elysauriax)
    * [Email me](eflores@nearsoft.com)
    
* Fernando:
    * [Github](https://github.com/ferzerkerx)
    * [Twitter](https://twitter.com/ferzerkerx)
    * [Email me](fmontes@nearsoft.com)