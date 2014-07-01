# top_builddirはconfig.hを探すため
# top_srcdirはプロジェクトのヘッダーファイルを探すため
AM_CPPFLAGS = \
	-I$(top_builddir) \
	-I$(top_srcdir)

# .cからGLibを使うためのコンパイラーオプションを指定
AM_CFLAGS = \
	$(GLIB_CFLAGS)

# 作成する共有ライブラリー（libsample）を指定
lib_LTLIBRARIES = \
	libsample.la

# libsampleで使うライブラリー（GLib）を指定
libsample_la_LIBADD = \
	$(GLIB_LIBS)

# libsampleのソースファイルを指定
libsample_la_SOURCES = \
	greeter.c \
	greeter.h
