## zshの`ls -l`の区切りが奇妙
### bashの場合
```
$ ls -l > test.txt
```

`less test.txt`の結果。
```
合計 76
drwxrwxr-x 3 yamaharu yamaharu 4096  8月 19 12:31 VirtualBox VMs
drwxrwxr-x 4 yamaharu yamaharu 4096 10月  5 17:17 dotfiles
drwxrwxr-x 2 yamaharu yamaharu 4096 10月  1 20:54 gpa
drwxrwxr-x 4 yamaharu yamaharu 4096  9月 18 19:22 note
-rw-rw-r-- 1 yamaharu yamaharu 2790 10月  5 13:58 parasite2.md
drwxrwxr-x 5 yamaharu yamaharu 4096 10月  4 11:23 perl5
-rw-rw-r-- 1 yamaharu yamaharu 1668 10月  5 18:57 problem.md
drwxr-xr-x 3 yamaharu yamaharu 4096  8月 19 12:14 snap
drwxrwxr-x 2 yamaharu yamaharu 4096 10月  5 18:53 study_file
-rwxrwxr-x 1 yamaharu yamaharu  309 10月  5 18:36 test.pl
-rw-rw-r-- 1 yamaharu yamaharu    0 10月  5 18:57 test.txt
drwxrwxr-x 3 yamaharu yamaharu 4096 10月  2 23:03 tools
drwxr-xr-x 2 yamaharu yamaharu 4096 10月  3 20:06 ダウンロード
drwxr-xr-x 2 yamaharu yamaharu 4096  8月 19 10:13 テンプレート
drwxr-xr-x 2 yamaharu yamaharu 4096  8月 19 10:13 デスクトップ
drwxr-xr-x 2 yamaharu yamaharu 4096  8月 19 10:13 ドキュメント
drwxr-xr-x 2 yamaharu yamaharu 4096  8月 19 10:13 ビデオ
drwxr-xr-x 2 yamaharu yamaharu 4096  9月 30 20:24 ピクチャ
drwxr-xr-x 2 yamaharu yamaharu 4096  8月 19 10:13 ミュージック
drwxr-xr-x 2 yamaharu yamaharu 4096  8月 19 10:13 公開
```
### zshの場合

```
$ ls -l > test.txt
```
`less test.txt`の結果。
```
合計 76
drwxrwxr-x 3 yamaharu yamaharu 4096  8月 19 12:31 [0m[01;34mVirtualBox VMs[0m
drwxrwxr-x 4 yamaharu yamaharu 4096 10月  5 17:17 [01;34mdotfiles[0m
drwxrwxr-x 2 yamaharu yamaharu 4096 10月  1 20:54 [01;34mgpa[0m
drwxrwxr-x 4 yamaharu yamaharu 4096  9月 18 19:22 [01;34mnote[0m
-rw-rw-r-- 1 yamaharu yamaharu 2790 10月  5 13:58 parasite2.md
drwxrwxr-x 5 yamaharu yamaharu 4096 10月  4 11:23 [01;34mperl5[0m
-rw-rw-r-- 1 yamaharu yamaharu 1269 10月  5 18:50 problem.md
drwxr-xr-x 3 yamaharu yamaharu 4096  8月 19 12:14 [01;34msnap[0m
drwxrwxr-x 2 yamaharu yamaharu 4096 10月  5 18:48 [01;34mstudy_file[0m
-rwxrwxr-x 1 yamaharu yamaharu  309 10月  5 18:36 [01;32mtest.pl[0m
-rw-rw-r-- 1 yamaharu yamaharu    0 10月  5 18:51 test.txt
drwxrwxr-x 3 yamaharu yamaharu 4096 10月  2 23:03 [01;34mtools[0m
drwxr-xr-x 2 yamaharu yamaharu 4096 10月  3 20:06 [01;34mダウンロード[0m
drwxr-xr-x 2 yamaharu yamaharu 4096  8月 19 10:13 [01;34mテンプレート[0m
drwxr-xr-x 2 yamaharu yamaharu 4096  8月 19 10:13 [01;34mデスクトップ[0m
drwxr-xr-x 2 yamaharu yamaharu 4096  8月 19 10:13 [01;34mドキュメント[0m
drwxr-xr-x 2 yamaharu yamaharu 4096  8月 19 10:13 [01;34mビデオ[0m
drwxr-xr-x 2 yamaharu yamaharu 4096  9月 30 20:24 [01;34mピクチャ[0m
drwxr-xr-x 2 yamaharu yamaharu 4096  8月 19 10:13 [01;34mミュージック[0m
drwxr-xr-x 2 yamaharu yamaharu 4096  8月 19 10:13 [01;34m公開[0m
```
