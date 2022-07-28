# master-thesis
![GitHub last commit](https://img.shields.io/github/last-commit/Tale152/master-thesis)
![GitHub release (latest by date including pre-releases)](https://img.shields.io/github/v/release/Tale152/master-thesis?include_prereleases)
![GitHub Release Date](https://img.shields.io/github/release-date/Tale152/master-thesis)
![GitHub commits since latest release (by date)](https://img.shields.io/github/commits-since/Tale152/master-thesis/latest)

➡️ [Get latest PDF draft here](https://github.com/Tale152/master-thesis/releases/latest) ⬅️

## About the thesis
### Title:
__Integrating mobile devices into Grid Computing__

### Abstract:
TODO

## How to trigger document CD
First create a new tag, including a message that sums up the notes for the new release.  
```console
git tag -a v<VERSION> -m "<RELEASE NOTES>" 
```
Then push the new tag to the remote repository, triggering [this](https://github.com/Tale152/master-thesis/blob/master/.github/workflows/compile-and-upload-latex.yml) workflow, crating automatically a new [release](https://github.com/Tale152/master-thesis/releases/latest) with the compiled PDF document.
```console
git push origin --tags
```
 