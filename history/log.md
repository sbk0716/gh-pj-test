# Install NodeJS

FYI:
https://nodejs.org/en/download/package-manager/#macos

```sh
% brew install node
Warning: node 18.9.1 is already installed and up-to-date.
To reinstall 18.9.1, run:
  brew reinstall node
% which node
/opt/homebrew/bin/node
% node -v
v18.9.1
%
% npm install --global yarn

changed 1 package, and audited 2 packages in 864ms

found 0 vulnerabilities
% yarn -v
1.22.19
%
```

# Scaffolding Your First Vite Project

FYI:
https://vitejs.dev/guide/#scaffolding-your-first-vite-project
```sh
% yarn create vite
yarn create v1.22.19
[1/4] 🔍  Resolving packages...
[2/4] 🚚  Fetching packages...
[3/4] 🔗  Linking dependencies...
[4/4] 🔨  Building fresh packages...
success Installed "create-vite@3.1.0" with binaries:
      - create-vite
      - cva
✔ Project name: … vite-project
✔ Select a framework: › React
✔ Select a variant: › TypeScript

Scaffolding project in /Users/admin/Desktop/study/gh-pj-test/vite-project...

Done. Now run:

  cd vite-project
  yarn
  yarn dev

✨  Done in 7.48s.
% 
% 
```


# Run Vite Project

```sh
% cd vite-project
% yarn 
yarn install v1.22.19
info No lockfile found.
[1/4] 🔍  Resolving packages...
[2/4] 🚚  Fetching packages...
[3/4] 🔗  Linking dependencies...
[4/4] 🔨  Building fresh packages...
success Saved lockfile.
✨  Done in 31.55s.
% yarn dev
yarn run v1.22.19
$ vite

  VITE v3.1.3  ready in 362 ms

  ➜  Local:   http://localhost:5173/
  ➜  Network: use --host to expose
...
...
```

```sh
% curl -sS http://localhost:5173/ | grep title
    <title>Vite + React + TS</title>
% 
```