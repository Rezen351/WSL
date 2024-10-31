# WSL
## Cara memindahkan filesystem wsl
Langkah-langkah untuk menginstal dan menjalankan proyek:

1. **Get Started**:
   ```bash
    cd D:\
    mkdir WSL
    cd WSL
    wsl --export <Distribution> ubuntu.tar
    wsl --unregister <Distribution>
    mkdir Ubuntu
    wsl --import <Distribution> <path> ubuntu.tar

'''
