librbd_la_SOURCES = \
	librbd/librbd.cc \
	librbd/AioCompletion.cc \
	librbd/AioRequest.cc \
	librbd/ImageCtx.cc \
	librbd/internal.cc \
	librbd/LibrbdWriteback.cc \
	librbd/WatchCtx.cc
librbd_la_LIBADD = \
	$(LIBRADOS) $(LIBOSDC) \
	libcls_rbd_client.la libcls_lock_client.la \
	$(PTHREAD_LIBS) $(EXTRALIBS)
librbd_la_LDFLAGS = ${AM_LDFLAGS} -version-info 1:0:0 -export-symbols-regex '^rbd_.*'
lib_LTLIBRARIES += librbd.la

noinst_HEADERS += \
	librbd/AioCompletion.h \
	librbd/AioRequest.h \
	librbd/ImageCtx.h \
	librbd/internal.h \
	librbd/LibrbdWriteback.h \
	librbd/parent_types.h \
	librbd/SnapInfo.h \
	librbd/WatchCtx.h
