# 📝 Development Guide

{% hint style="info" %}
**Starkland tip:** If you're not a developer, you don't need to focus on this section.
{% endhint %}

## [Starkland](https://github.com/Starklandxyz/app#starkland) <a href="#user-content-starkland" id="user-content-starkland"></a>

#### [Steps to Execute](https://github.com/Starklandxyz/app#steps-to-execute) <a href="#user-content-steps-to-execute" id="user-content-steps-to-execute"></a>

Clone repository `git clone https://github.com/Starklandxyz/app --recursive`

Clone submodule `git submodule add https://github.com/Starklandxyz/contract contracts`

* Build contracts
* Build Frontend

Subsequently, clone this project and execute the following commands in the terminal:

```
yarn

yarn dev
```

#### [contracts](https://github.com/Starklandxyz/app#contracts) <a href="#user-content-contracts" id="user-content-contracts"></a>

### [DEV](https://github.com/Starklandxyz/app#dev) <a href="#user-content-dev" id="user-content-dev"></a>

instal dojo toolchain with `dojoup -v nightly`

go contracts folder

1. terminal\_1 `katana --disable-fee`
2. terminal\_2, comment world\_address `sozo build && sozo migrate name --test`
3. terminal\_3 uncomment world\_address `touch indexer.db` `torii -d indexer.db`

To avoid redeploying contracts, you can save the Katana state by using the following command. `katana --disable-fee --load-state ./dump-state.bin --dump-state ./dump-state.bin`

4. generate component `yarn components`
5. generate sql indexer `yarn codegen`
