1. Create a github repository called <github-username>.github.io
2. Create a folder C:\Hugo\bin
3. Download the Hugo release from https://github.com/gohugoio/hugo/releases (not needed the extended version)
4. Extract the zip into the folder created before (make sure the execuable hugo is with lowercase h)
5. Open CMD, go to Hugo/bin and type 'hugo version'
6. To make executable hugo in every folder add bin folder to path variables
7. Go into your project folder and run 'hugo new site . --force' (if you want you can do everything first in a
dev repo)
8. Add your theme 'git submodule add --depth=1 https://github.com/adityatelange/hugo-PaperMod.git themes/PaperMod
' 'git submodule update --init --recursive # needed when you reclone your repo (submodules may not get cloned automatically)
'
9. Tell hugo to use the theme: 'echo 'theme = "PaperMod"' >> config.toml'
10. Create a new post: 'hugo new post/testpage.md'
