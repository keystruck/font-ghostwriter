# font-ghostwriter


## Build Instructions

1. Install `node` locally.

2. Clone the Iosevka repo into a local dedicated folder. The full repo weighs in at >30GB so limit the depth of the clone.

```
git clone --depth 1 https://github.com/be5invis/Iosevka -o iosevka
```

3. Clone this repo into another local dedicated folder, then copy or symlink `private-build-plans.toml` into the iosevka repo directory.

```
git clone https://github.com/keystruck/font-ghostwriter -o font-ghostwriter
ln -s font-ghostwriter/private-build-plans.toml iosevka/private-build-plans.toml
```

4. `cd` into the iosevka directory, update the repo files, and install any required `npm` dependencies.

```
cd iosevka
git pull
npm install
```

5. Build the font.

```
npm run build ttf::GW{Code,Type,SansQuasi}{,Cond}
```

After the build completes the font files will be found in the repo `/dist` directory.


## Iosevka Resources

Customizer: [https://typeof.net/Iosevka/Customizer]
