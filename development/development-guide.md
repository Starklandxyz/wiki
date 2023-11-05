# 📝 Development Guide

{% hint style="info" %}
**Starkland tip:** If you're not a developer, you don't need to focus on this section.
{% endhint %}

go contracts folder

1. terminal\_1 `katana --disable-fee`
2. terminal\_2, comment world\_address `sozo build && sozo migrate --name test`
3. terminal\_3 uncomment world\_address `touch indexer.db` `torii -d indexer.db`
