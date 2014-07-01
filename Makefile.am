# configure.acでm4/以下にM4マクロを置くようにしたので
# m4/以下もパスに加える。
# また、ユーザーがACLOCAL_FLAGS環境変数でオプションを
# 渡せるようにしている。
ACLOCAL_AMFLAGS = -I m4 ${ACLOCAL_FLAGS}

# 再帰的にsample/以下もmakeする。
SUBDIRS = \
	sample
