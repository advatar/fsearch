# STATUS

## Security hardening (GitHub issues are disabled; details in the commit)

- [x] Data dir created owner-only (0700), socket 0600
- [x] Reject index/segment headers whose counts exceed the file (no section-math overflow into out-of-bounds mmap reads)
- [x] CLI output replaces control characters, so hostile file names or contents can't send terminal escape sequences
- [x] XML-escape paths written into the LaunchAgent plist
- [x] README: Security section (with Full Disk Access the daemon reads protected folders for any process running as you)
- [ ] Decide: restrict which clients may use the socket when the daemon has Full Disk Access
