# Changelog

All notable changes to this configuration are documented here.

---

## [1.0] — 2026-04-04

### Added
- Initial production configuration — hardened firewalld for openSUSE Tumbleweed
- nftables backend (`FirewallBackend=nftables`)
- `zone public` (target DROP, default zone) on `br0` — whitelist-only inbound
- `zone trusted` (source 192.168.1.0/24) — monitoring stack ports (Prometheus, Grafana, Loki, exporters)
- `zone libvirt` (target ACCEPT) — KVM VM isolation with priority 32767 reject rule
- `zone libvirt-routed` — routed KVM network support
- `zone docker` — Docker bridge (ACCEPT)
- Policy `libvirt-to-host` (REJECT) — VMs blocked from host except DNS, DHCP, SSH, TFTP, ICMP
- Policy `libvirt-routed-in/out` (ACCEPT) — routed VM traffic
- Policy `allow-host-ipv6` — NDP/RA for host IPv6
- `lockdown-whitelist.xml` — D-Bus access restricted to firewall-config, root, NetworkManager, virtd
- `LogDenied=all` — all dropped/rejected packets logged to journald
- `ReloadPolicy=INPUT:DROP,FORWARD:DROP,OUTPUT:DROP` — secure reload window
- `IPv6_rpfilter=yes` + `RFC3964_IPv4=yes` — anti-spoofing
- Real terminal output examples for all documented commands (`examples/`)
- Full Mermaid architecture diagram in README
