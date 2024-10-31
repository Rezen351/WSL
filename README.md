# WSL
## Cara memindahkan filesystem wsl
'''bash
  cd D:\
  mkdir WSL
  cd WSL
  wsl --export <Distribution> ubuntu.tar
  wsl --unregister <Distribution>
  mkdir Ubuntu
  wsl --import <Distribution> <path> ubuntu.tar
  
  '''
fdf
