INCLUDES = -I. -I../swe -I../pics

AM_CPPFLAGS = $(WX_CPPFLAGS) -Wall -DSTRICT 

# Remove this when gimp writes xpm like const *char
AM_CPPFLAGS += -Wno-write-strings

noinst_LIBRARIES = libmaitreya_base.a

libmaitreya_base_a_SOURCES = Calculator.cpp Calculator.h ChartConfig.cpp ChartConfig.h \
	ChartProperties.cpp ChartProperties.h ColorConfig.cpp ColorConfig.h Commands.cpp Commands.h \
	Conf.cpp Conf.h ConfigLoader.h constants.cpp constants.h DataSet.cpp DataSet.h \
	FileConfig.cpp FileConfig.h FontConfig.cpp FontConfig.h IconProvider.cpp IconProvider.h \
	Lang.cpp Lang.h LanguageConfig.cpp LanguageConfig.h mathbase.cpp mathbase.h \
	MultipleViewConfig.cpp MultipleViewConfig.h PlanetList.cpp PlanetList.h \
	PrintoutConfig.cpp PrintoutConfig.h VedicChartConfig.cpp VedicChartConfig.h \
	ViewNode.cpp ViewNode.h WesternChartConfig.cpp WesternChartConfig.h XmlWorker.cpp XmlWorker.h

all-am: 

clean:
	rm -f lib*.a *.o core *~ *.bak
	rm -fr obj bin

EXTRA_DIST = Makefile.win base.vcproj 

