VS_PRODUCT=xuggle_xuggler
VS_CPP_PATH=com/xuggle/xuggler
VS_CPP_PACKAGE=com.xuggle.xuggler
VS_CPP_NAMESPACE=com::xuggle::xuggler
include @top_builddir@/mk/Makefile.global

SUBDIRS=io
SUFFIXES=.i

noinst_LTLIBRARIES = libxuggle-xuggler.la

libxuggle_xuggler_la_LIBADD= $(VS_PKG_LIBRARIES)

libxuggle_xuggler_la_SOURCES= \
  AudioResampler.cpp \
  AudioSamples.cpp \
  Codec.cpp \
  Container.cpp \
  ContainerFormat.cpp \
  Error.cpp \
  VideoPicture.cpp \
  Global.cpp \
  IAudioResampler.cpp \
  IAudioSamples.cpp \
  ICodec.cpp \
  IContainer.cpp \
  IContainerFormat.cpp \
  IError.cpp \
  IVideoPicture.cpp \
  IIndexEntry.cpp \
  IndexEntry.cpp \
  IMediaData.cpp \
  IMediaDataWrapper.cpp \
  IMetaData.cpp \
  IPacket.cpp \
  IPixelFormat.cpp \
  IProperty.cpp \
  IRational.cpp \
  IStreamCoder.cpp \
  IStream.cpp \
  ITimeValue.cpp \
  IVideoResampler.cpp \
  MediaDataWrapper.cpp \
  MetaData.cpp \
  Packet.cpp \
  Property.cpp \
  Rational.cpp \
  StreamCoder.cpp \
  Stream.cpp \
  TimeValue.cpp \
  VideoResampler.cpp

nodist_libxuggle_xuggler_la_SOURCES= \
  Xuggler.cpp

#if VS_ENABLE_GPL
#libxuggle_xuggler_la_SOURCES+= \
#  VideoResampler.cpp 
#endif

libxuggle_xuggler_ladir=$(includedir)/$(VS_CPP_PATH)
libxuggle_xuggler_la_HEADERS= \
  Xuggler.h \
  config.h \
  FfmpegIncludes.h \
  Global.h \
  Global.swg \
  IAudioResampler.h \
  IAudioSamples.h \
  IAudioSamples.swg \
  ICodec.h \
  ICodec.swg \
  IContainerFormat.h \
  IContainerFormat.swg \
  IContainer.h \
  IContainer.swg \
  IError.h \
  IError.swg \
  IIndexEntry.h \
  IIndexEntry.swg \
  IVideoPicture.h \
  IVideoPicture.swg \
  IMediaData.h \
  IMediaData.swg \
  IMetaData.h \
  IMetaData.swg \
  IMediaDataWrapper.h \
  IMediaDataWrapper.swg \
  IPacket.h \
  IPacket.swg \
  IPixelFormat.h \
  IProperty.h \
  IRational.h \
  IRational.swg \
  IStreamCoder.h \
  IStreamCoder.swg \
  IStream.h \
  IStream.swg \
  ITimeValue.h \
  IVideoResampler.h \
  IVideoResampler.swg \
  Xuggler.i \
  AudioResampler.h \
  AudioSamples.h \
  Codec.h \
  ContainerFormat.h \
  Container.h \
  Error.h \
  IndexEntry.h \
  VideoPicture.h \
  MediaDataWrapper.h \
  MetaData.h \
  Packet.h \
  PixelFormat.h \
  Property.h \
  Rational.h \
  StreamCoder.h \
  Stream.h \
  TimeValue.h \
  VideoResampler.h 

BUILT_SOURCES= \
  Xuggler.cpp

Xuggler.cpp : $(libxuggle_xuggler_la_HEADERS)

clean-local:
	rm -f $(BUILT_SOURCES)
	if test -w "$(SWIGOUTTMPDIR)"; then rm -rf $(SWIGOUTTMPDIR); fi

maintainer-clean-local:
	rm -rf $(SWIGOUTDIR)/$(VS_CPP_PATH)

