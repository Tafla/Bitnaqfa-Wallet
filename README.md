**1. Clone wallet sources**

```
git clone https://github.com/Tafla/Digital-Naqfa-Core.git
```

**2. Modify `CryptoNoteWallet.cmake`**
 
```
set(CN_PROJECT_NAME "furiouscoin")
set(CN_CURRENCY_DISPLAY_NAME "FuriousCoin")
set(CN_CURRENCY_TICKER "XFC")
```

**3. Set symbolic link to coin sources at the same level as `src`. For example:**

```
ln -s ../Tafla cryptonote```

Alternative way is to create git submodule:

```
git submodule add https://github.com/Tafla/Digital-Naqfa-Core.git cryptonote
```

Replace URL with git remote repository of your coin.

**4. Build**

```
mkdir build && cd build && cmake .. && make
```
