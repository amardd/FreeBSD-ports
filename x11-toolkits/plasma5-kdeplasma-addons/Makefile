# $FreeBSD$

PORTNAME=	kdeplasma-addons
DISTVERSION=	${KDE_PLASMA_VERSION}
CATEGORIES=	x11-toolkits kde kde-plasma

MAINTAINER=	kde@FreeBSD.org
COMMENT=	Plasma5 addons to improve the Plasma experience

USES=		cmake compiler:c++11-lib cpe gettext \
		kde:5 pkgconfig qt:5 tar:xz
USE_KDE=	activities archive attica auth bookmarks codecs completion \
		config configwidgets coreaddons crash ecm emoticons guiaddons \
		i18n iconthemes init itemmodels itemviews jobwidgets kcmutils \
		kdelibs4support kio kross newstuff notifications package parts\
		plasma-framework plasma-workspace runner service solid \
		sonnet textwidgets unitconversion widgetsaddons windowsystem xmlgui
USE_QT=		core dbus declarative graphicaleffects gui location network \
		printsupport script webchannel widgets x11extras xml \
		buildtools_build qmake_build
# The webengine in the offical ports is too old for now. Once updated to 5.12.x r
# readd webengine.

OPTIONS_DEFINE=	PURPOSE
OPTIONS_DEFAULT=	PURPOSE

PURPOSE_DESC=	Enable 'QuickShare' applet
PURPOSE_USE=	KDE=purpose
PURPOSE_CMAKE_BOOL_OFF=	CMAKE_DISABLE_FIND_PACKAGE_KF5Purpose

.include <bsd.port.mk>
