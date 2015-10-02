## Git usage scenario

Emily is a developer for a Cincinnati based company and was recently tasked with a few updates to the company website.
The company uses git to keep track of their code changes and also allow all of their developers to work in harmony.

Being a new hire, Emily has yet to get a copy of the code, but is provided a [link](https://github.com/tcmacdonald/intro-to-git-starter-kit.git) to the existing company Github account. Since she only has read access to the company account, for now she Forks it to her own account in order to work on it. ![Fork Repo](images/fork.png "Fork repo")

She now has her own copy of the website and can finally get to work. To do that she will clone the Forked company website onto her laptop via the `git clone` command

    $ git clone https://github.com/emily/intro-to-git-starter-kit.git
      Cloning into 'intro-to-git-starter-kit'...
      remote: Counting objects: 17, done.
      remote: Compressing objects: 100% (10/10), done.
      remote: Total 17 (delta 3), reused 17 (delta 3), pack-reused 0
      Unpacking objects: 100% (17/17), done.
      Checking connectivity... done.

Git just created a new directory called `intro-to-git-starter-kit` containing all the project files. Let's inspect...

    $ cd intro-to-git-starter-kit/
    $ ls -la
      total 24
      drwxr-xr-x   7 emily  staff   238 Sep 24 23:00 .
      drwxr-xr-x  36 emily  staff  1224 Sep 24 23:00 ..
      drwxr-xr-x  13 emily  staff   442 Sep 24 23:00 .git
      -rw-r--r--   1 emily  staff    10 Sep 24 23:00 .gitignore
      -rw-r--r--   1 emily  staff   583 Sep 24 23:00 about.html
      drwxr-xr-x   3 emily  staff   102 Sep 24 23:00 images
      -rw-r--r--   1 emily  staff    13 Sep 24 23:00 index.html

She can now open the 'intro-to-git-starter-kit' folder with Sublime in order to make her changes.
