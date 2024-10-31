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
2. **Connect Google Internet**:
 ```bash
   sudo nano /etc/resolv.conf
   nameserver 8.8.8.8
   nameserver 8.8.4.4

'''
Get-ChildItem "C:\" | Where-Object { $_.PSIsContainer } | ForEach-Object {
>>     $size = (Get-ChildItem -Path $_.FullName -Recurse -File | Measure-Object -Property Length -Sum).Sum
>>     [PSCustomObject]@{
>>         FolderName = $_.Name
>>         SizeMB     = "{0:N2}" -f ($size / 1MB)
>>     }
>> } | Format-Table -AutoSize
