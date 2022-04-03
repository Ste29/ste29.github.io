1. Create a github repository called <github-username>.github.io
2. Create a folder C:\Hugo\bin
3. Download the Hugo release from https://github.com/gohugoio/hugo/releases (not needed the extended version)
4. Extract the zip into the folder created before (make sure the execuable hugo is with lowercase h)
5. Open CMD, go to Hugo/bin and type 'hugo version'
6. To make executable hugo in every folder add bin folder to path variables
7. Go into your dev project folder and run 'hugo new site . --force' (if you want you can do everything first in a
dev repo)
8. Add your theme 'git submodule add --depth=1 https://github.com/adityatelange/hugo-PaperMod.git themes/PaperMod
' 'git submodule update --init --recursive # needed when you reclone your repo (submodules may not get cloned automatically)
'
9. Tell hugo to use the theme: 'echo 'theme = "PaperMod"' >> config.toml'
10. Create a new post: 'hugo new post/testpage.md', the generated posts have an header between ---, this stores information to create a render
page. It's some sort of metadata. Those metadata come from archetypes/default.md
11. Every configuration is stored inside config.toml
12. Test your dev repo with 'hugo server -D'
13. Set up config.toml (you can use instead config.yaml or config.json, as you pref) https://gohugo.io/getting-started/configuration/
put images in /static
-- 14. commit and push dev repo
-- 15. go in ste29.github.io repo and do 'git submodule add -b main https://github.com/Ste29/blog-dev/public' this will clone dev repo in
public folder

14. run deploy.sh in bash or git shell, this will set up your blog
15. copy public folder inside main repo


git submodule copy another repo in a specified folder of your repo, it manages everything through a .gitmodules file and 
modules folder inside .git