# N0ctOS-configs

Config bundled packages for N0ctOS Linux.

## Structure

```
n0ctos-<pkg>/
├── PKGBUILD                   # depends=(<pkg>), installs configs
├── n0ctos-<pkg>.install       # post_install / post_remove hooks
└── config/
    ├── default/               → /usr/share/N0ctOS/config/n0ctos-<pkg>/
    └── custom/                → ~/.config/<pkg>/
```

## Usage

```bash
# Create a new config package
./init-pkg

# Build all changed packages
./build-changed

# Build everything, deploy, push
./auto-all
```

## Branch

All work targets the `configs` branch.
