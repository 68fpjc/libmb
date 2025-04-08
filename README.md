# 暫定 libmb for elf2x68k

## これはなに？

Project LIBC Group のマルチバイト文字ライブラリ libmb を [elf2x68k](https://github.com/yunkya2/elf2x68k) でビルドしたものです。

- 個人的に必要になって突貫工事で用意したものです。今後、正式なライブラリが登場したらそちらに乗り換えます。
- C++ については考慮していません。

```bash
$ m68k-xelf-ar t libmb.a | sort
_mbctype.o
_mblen.o
_mbset.o
ismbbalnum.o
ismbbalpha.o
ismbbgraph.o
ismbbkalnum.o
ismbbkana.o
ismbbkpunct.o
ismbblead.o
ismbbprint.o
ismbbpunct.o
ismbbtrail.o
ismbcalpha.o
ismbcdigit.o
ismbchira.o
ismbckata.o
ismbcl0.o
ismbcl1.o
ismbcl2.o
ismbclegal.o
ismbclower.o
ismbcprint.o
ismbcspace.o
ismbcsymbol.o
ismbcupper.o
mbbtombc.o
mbbtype.o
mbctohira.o
mbctokata.o
mbctolower.o
mbctombb.o
mbctoupper.o
mbsbtype.o
mbscat.o
mbschr.o
mbscmp.o
mbscpy.o
mbscspn.o
mbsdec.o
mbsdup.o
mbsicmp.o
mbsinc.o
mbslen.o
mbslwr.o
mbsnbcnt.o
mbsncat.o
mbsnccnt.o
mbsncmp.o
mbsncpy.o
mbsnextc.o
mbsnicmp.o
mbsninc.o
mbspbrk.o
mbsrchr.o
mbsrev.o
mbsset.o
mbsspn.o
mbsspnp.o
mbstok.o
mbsupr.o
```

## ソースコードからのビルド

[elf2x68k](https://github.com/yunkya2/elf2x68k) が必要です。 makefile のあるディレクトリで `make` してください。

## ライセンス

このディレクトリ配下のファイルは CC0 1.0 Universal でライセンスされます。

`*.h` は Project LIBC Group による原作を改変したものですが、 CC0 1.0 Universal とすることに問題ないはずです。

## 連絡先

https://github.com/68fpjc/libmb
