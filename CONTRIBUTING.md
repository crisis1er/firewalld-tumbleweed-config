# Contributing

Contributions are welcome — especially from openSUSE Tumbleweed
and openSUSE Leap users.

## License agreement

By contributing, you agree that your contributions will be licensed
under **GNU GPL v3.0**.  
Attribution will reference **crisis1er** (https://github.com/crisis1er)
and **SafeITExperts** (https://safeitexperts.com).

## How to contribute

1. **Fork** this repository
2. **Create a branch** from `main`:
   ```bash
   git checkout -b fix/your-description
   ```
3. **Make your changes** — keep commits focused and atomic
4. **Test** on openSUSE Tumbleweed before submitting  
   Compatibility with openSUSE Leap and openSUSE-based distributions
   is welcome but not required
5. **Open a Pull Request** against `main`

## What to include in your PR

- What the change does and why
- Your openSUSE version:
  ```bash
  cat /etc/os-release
  ```
- firewalld version:
  ```bash
  firewall-cmd --version
  ```
- Whether you tested on a live system

## Bug reports

Open an [issue](https://github.com/crisis1er/firewalld-tumbleweed-config/issues) and include:
- File(s) concerned
- Your openSUSE version and firewalld version
- Exact error message — paste text, never screenshot
- Steps to reproduce

## Style guidelines

- Config files: keep section comments aligned with existing structure
- XML files: well-formed, indented with 2 spaces
- Markdown: one sentence per line for easier diffs

## Questions

See [SUPPORT.md](SUPPORT.md).
