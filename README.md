# Website


How to manage PaperMod theme: https://github.com/adityatelange/hugo-PaperMod/wiki/Installation

https://github.com/adityatelange/hugo-PaperMod/wiki/installation#sample-configyml
https://github.com/adityatelange/hugo-PaperMod/wiki/Features#regular-mode-default-mode
https://github.com/adityatelange/hugo-PaperMod/tree/exampleSite


More specifically...

## Method 1
Inside the folder of your Hugo site, run:
``` 
git clone https://github.com/adityatelange/hugo-PaperMod themes/PaperMod --depth=1
```
Note: You may use  ```--branch v7.0``` to end of above command if you want to stick to specific release.

Updating theme with Method 1 :
```
cd themes/PaperMod
git pull
```

## Method 2
you can use as submodule with
```
git submodule add --depth=1 https://github.com/adityatelange/hugo-PaperMod.git themes/PaperMod
git submodule update --init --recursive # needed when you reclone your repo (submodules may not get cloned automatically)
```
Note: You may use  ```--branch v7.0``` to end of above command if you want to stick to specific release.

Updating theme with Method 2 :
```
git submodule update --remote --merge
```
