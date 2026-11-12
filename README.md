# nkp-bund

## Reassemble the bundle

The tarball is split into 90 MB parts (GitHub's 100 MB file limit). To restore it:

```bash
cd parts
cat 1.36.2_ubuntu_22.04_x86_64.tar.gz.part-* > ../1.36.2_ubuntu_22.04_x86_64.tar.gz
cd .. && sha256sum -c parts/1.36.2_ubuntu_22.04_x86_64.tar.gz.sha256
```
