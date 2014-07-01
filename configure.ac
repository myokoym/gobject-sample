# Autoconf 2.65以上を必須にする
#  これは、Antomake 1.13がAutoconf-h 2.65以上が必須だから
AC_PREREQ(2.65)

# Autoconfを初期化
AC_INIT([gtk-doc-sample], [1.0.0], [myokoym@gmail.com])
# 補助スクリプトをconfig/以下に置く
AC_CONFIG_AUX_DIR([config])
# M4マクロをm4/以下に置く
AC_CONFIG_MACRO_DIR([m4])

# ソースディレクトリーを検出するために、
# ソースディレクトリーに必ずあるファイルを指定
AC_CONFIG_SRCDIR([sample/greeter.h])
# AC_DEFINEで定義した変数を出力するヘッダーファイルを指定
AC_CONFIG_HEADERS([config.h])

# 1.13:    Antumake 1.13以降必須
# foreign: NEWSなどのファイルを必須としない
AM_INIT_AUTOMAKE([1.13 foreign])
# ビルドする時にコマンドラインではなく
# どんな役割のコマンドを実行しているかを出力するだけにする
AM_SILENT_RULES([yes])

# Cコンパイラーを検出
AC_PROG_CC
# Libtoolsを初期化
LT_INIT

# GLib 2.32.4以降必須
# GLibの中のgobjectモジュールを使う
AM_PATH_GLIB_2_0([2.32.4], [], [], [gobject])

# .inから生成するファイルを指定
AC_CONFIG_FILES([
  Makefile
  sample/Makefile
])

# AC_CONFIG_FILESで指定したファイルなどを生成
AC_OUTPUT
