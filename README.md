# modelrepo_dense
An example repository creating a model using the [DENSE](https://github.com/johnastratton/DENSE "DENSE github repository") framework

###To create as an independent project:

* Create header files as required for a DENSE model

* clone [DENSE](https://github.com/johnastratton/DENSE "DENSE github repository) into some directory

* execute `cmake <path-to-DENSE> && make` to build simulator using the model


###To create as a git repository with DENSE as a submodule:

* Create a git repository

* Within that repository, use the command `git submodule https://github.com/johnastratton/DENSE.git`

* Commit the repository state, which should consist of .gitmodules and the DENSE directory (but not its contents)

* Create header files as required for a DENSE model.

* execute `cmake DENSE && make` to build the simulator submodule on the model header files


###To clone a git submodularized repository (such as this one):

* `git clone <repo>` after which the base repository (but not the subrepo) is cloned and downloaded

* `cd <reponame>/DENSE`

* `git submodule init`

* `git submodule update` after which the subrepo is fully downloaded


Alternatively, the quick-and-easy one-line command to do all of the above is `git clone --recurse-submodules <model_repo>`
