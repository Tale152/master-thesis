# master-thesis
![GitHub last commit](https://img.shields.io/github/last-commit/Tale152/master-thesis)
![GitHub release (latest by date including pre-releases)](https://img.shields.io/github/v/release/Tale152/master-thesis?include_prereleases)
![GitHub Release Date](https://img.shields.io/github/release-date/Tale152/master-thesis)
![GitHub commits since latest release (by date)](https://img.shields.io/github/commits-since/Tale152/master-thesis/latest)

➡️ [Get latest PDF draft here](https://github.com/Tale152/master-thesis/releases/latest) ⬅️

## About the thesis
### Title: __Integrating mobile devices into Grid Computing__

### Presented by: [Alessandro Talmi](https://github.com/Tale152)

### Supervised by: [Alessandro Ricci](https://www.unibo.it/sitoweb/a.ricci)

### Abstract:
The idea of Grid Computing originated at the beginning of the nineties and found its concrete applications in contexts like the SETI@home project; in said project, a lot of computers (offered by volunteers) cooperated performing distributed computations in the Grid environment trying to analyze radio signals trying to find extraterrestrial life.  

The Grid was composed of traditional personal computers but, with the emergence of the first mobile devices like Personal Digital Assistants (PDAs), researchers started theorizing the inclusion of mobile devices into Grid Computing; although impressive theoretical work was done, the idea was discarded due to the limitations (mainly technological) of the mobile devices available at the time. Decades have passed and the current mobile devices are extremely more performant and numerous than before, leaving a great amount of resources available on mobile devices, like smartphones and tablets, untapped.  

Here we propose a solution for performing distributed computations over a Grid Computing environment that utilizes both desktop and mobile devices exploiting the resources from day to day mobile users that alternatively would end up unused.  

The work starts with a high-level introduction, discussing what Grid Computing is, the evolution of mobile devices, the idea of integrating such devices into the Grid and, last but not least, how to convince device owners to participate in the Grid. Following the introduction the tone gets more technical, starting with an explanation on how Grid Computing actually works, followed by the technical challenges of integrating mobile devices into the Grid. A brief explanation of the MapReduce paradigm is then provided, since it will be useful to understand the solution proposed by this work. Once all the required knowledge is presented, the model, that constitutes the solution offered by this work, is explained. Following the mode, the work continues presenting a chapter regarding the realization of a prototype that tries to prove the feasibility of distributed computations over a Grid composed by both mobile and desktop devices. To conclude, a last chapter presents future developments and ideas to improve this project.

## Requirements to Compile the Document on VSCode
### Install the recommended dependencies
Upon opening the project VSCode will ask you if you want to install the required dependencies; proceed to install them.  

Alternatively, recommended dependencies can be found under the extensions tab typing _@recommended_ in the search bar.

### Install required software (Windows)
Follow [this](https://www.youtube.com/watch?v=4lyHIQl4VM8) tutorial to install the required software on Windows (if you installed the recommended dependencies you will already have LaTeX Workshop on VSCode).

## How to trigger document CD
First create a new tag, including a message that sums up the notes for the new release.  
```console
git tag -a v<VERSION> -m "<RELEASE NOTES>" 
```
Then push the new tag to the remote repository, triggering [this](https://github.com/Tale152/master-thesis/blob/master/.github/workflows/compile-and-upload-latex.yml) workflow, crating automatically a new [release](https://github.com/Tale152/master-thesis/releases/latest) with the compiled PDF document.
```console
git push origin --tags
```
 