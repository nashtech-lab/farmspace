# Git operators guidance

## Add a submodule

```
git submodule add <repository> <path>
```

Example

```
git submodule add  https://github.com/nashtech-lab/farmspace-docs.git documentation
```

## Clone repository includes submodules

```
git clone --recursive -b main https://github.com/nashtech-lab/farmspace.git
```

## Checkout all submodule to specified branch

```
git submodule foreach --recursive "git checkout <branch-name> || true"
```

Example 

```
git submodule foreach --recursive "git checkout main || true"
```