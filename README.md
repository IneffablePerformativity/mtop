This "mtop" will be a top module of some submodule.

-------- BLOW OFF TOP AND RE-CLONE IT!!!
Having existing github repositories, mtop and msub:
cd repo
rm -rf *
git clone git@github.com:IneffablePerformativity/msub.git
git clone git@github.com:IneffablePerformativity/mtop.git
cd mtop
git submodule add git@github.com:IneffablePerformativity/msub.git msub
Then all the appropriate git add, commit, push.

--------- FINALLY!
repo
├── msub
│   └── README.md
└── mtop
    ├── README.md
    └── msub
        └── README.md
