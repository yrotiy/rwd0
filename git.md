
ITSC@DESKTOP-ONE4R81 MINGW64 /d/frontend_2
$ git clone
fatal: You must specify a repository to clone.

usage: git clone [<options>] [--] <repo> [<dir>]

    -v, --verbose         be more verbose
    -q, --quiet           be more quiet
    --progress            force progress reporting
    --reject-shallow      don't clone shallow repository
    -n, --no-checkout     don't create a checkout
    --bare                create a bare repository
    --mirror              create a mirror repository (implies bare)
    -l, --local           to clone from a local repository
    --no-hardlinks        don't use local hardlinks, always copy
    -s, --shared          setup as shared repository
    --recurse-submodules[=<pathspec>]
                          initialize submodules in the clone
    --recursive ...       alias of --recurse-submodules
    -j, --jobs <n>        number of submodules cloned in parallel
    --template <template-directory>
                          directory from which templates will be used
    --reference <repo>    reference repository
    --reference-if-able <repo>
                          reference repository
    --dissociate          use --reference only while cloning
    -o, --origin <name>   use <name> instead of 'origin' to track upstream
    -b, --branch <branch>
                          checkout <branch> instead of the remote's HEAD
    -u, --upload-pack <path>
                          path to git-upload-pack on the remote
    --depth <depth>       create a shallow clone of that depth
    --shallow-since <time>
                          create a shallow clone since a specific time
    --shallow-exclude <revision>
                          deepen history of shallow clone, excluding rev
    --single-branch       clone only one branch, HEAD or --branch
    --no-tags             don't clone any tags, and make later fetches not to follow them
    --shallow-submodules  any cloned submodules will be shallow
    --separate-git-dir <gitdir>
                          separate git dir from working tree
    -c, --config <key=value>
                          set config inside the new repository
    --server-option <server-specific>
                          option to transmit
    -4, --ipv4            use IPv4 addresses only
    -6, --ipv6            use IPv6 addresses only
    --filter <args>       object filtering
    --also-filter-submodules
                          apply partial clone filters to submodules
    --remote-submodules   any cloned submodules will use their remote-tracking branch
    --sparse              initialize sparse-checkout file to include only files at root
    --bundle-uri <uri>    a URI for downloading bundles before fetching from origin remote


ITSC@DESKTOP-ONE4R81 MINGW64 /d/frontend_2
$ git init
Initialized empty Git repository in D:/frontend_2/.git/

ITSC@DESKTOP-ONE4R81 MINGW64 /d/frontend_2
$ git clone https://github.com/yrotiy/rwd0.git
Cloning into 'rwd0'...
remote: Enumerating objects: 58, done.
remote: Counting objects: 100% (58/58), done.
remote: Compressing objects: 100% (53/53), done.
remote: Total 58 (delta 4), reused 58 (delta 4), pack-reused 0
Receiving objects: 100% (58/58), 1.31 MiB | 494.00 KiB/s, done.
Resolving deltas: 100% (4/4), done.
Updating files: 100% (53/53), done.

ITSC@DESKTOP-ONE4R81 MINGW64 /d/frontend_2
$ ls
day05_1117/  rwd0/

ITSC@DESKTOP-ONE4R81 MINGW64 /d/frontend_2
$ cd rwd0

ITSC@DESKTOP-ONE4R81 MINGW64 /d/frontend_2/rwd0
$ git config --list
diff.astextplain.textconv=astextplain
filter.lfs.clean=git-lfs clean -- %f
filter.lfs.smudge=git-lfs smudge -- %f
filter.lfs.process=git-lfs filter-process
filter.lfs.required=true
http.sslbackend=openssl
http.sslcainfo=C:/Program Files/Git/mingw64/ssl/certs/ca-bundle.crt
core.autocrlf=true
core.fscache=true
core.symlinks=false
core.editor="C:\\Program Files\\Notepad++\\notepad++.exe" -multiInst -notabbar -nosession -noPlugin
pull.rebase=false
credential.helper=manager-core
credential.https://dev.azure.com.usehttppath=true
init.defaultbranch=master
user.email=jeongyi0113@naver.com
user.name=jeongyi
difftool.sourcetree.cmd=''
mergetool.sourcetree.cmd=''
mergetool.sourcetree.trustexitcode=true
safe.directory=D:/FRONTEND_02/day04_1116

ITSC@DESKTOP-ONE4R81 MINGW64 /d/frontend_2/rwd0
$ git add .
fatal: detected dubious ownership in repository at 'D:/frontend_2/rwd0'
'D:/frontend_2/rwd0' is on a file system that doesnot record ownership
To add an exception for this directory, call:

        git config --global --add safe.directory D:/frontend_2/rwd0

ITSC@DESKTOP-ONE4R81 MINGW64 /d/frontend_2/rwd0
$  git config --global --add safe.directory D:/frontend_2/rwd0

ITSC@DESKTOP-ONE4R81 MINGW64 /d/frontend_2/rwd0 (main)
$ git add .

ITSC@DESKTOP-ONE4R81 MINGW64 /d/frontend_2/rwd0 (main)
$ git commit -m 'reset css add'
[main 67256a2] reset css add
 2 files changed, 20 insertions(+), 1 deletion(-)
 create mode 100644 style/reset.css

ITSC@DESKTOP-ONE4R81 MINGW64 /d/frontend_2/rwd0 (main)
$ git push .
Everything up-to-date
