PORTNAME=	kpublictransport
DISTVERSION=	${KDE_APPLICATIONS_VERSION}
PORTREVISION=	6
CATEGORIES=	devel kde kde-applications

MAINTAINER=	kde@FreeBSD.org
COMMENT=	Access realtime public transport data

LIB_DEPENDS=	libprotobuf.so:devel/protobuf

USES=		cmake compiler:c++11-lang kde:5 qt:5 tar:xz
USE_KDE=	ecm:build
USE_QT=		core declarative gui network \
		buildtools:build qmake:build

OPTIONS_DEFINE=	DOCS

# Override shared library version
KDE_APPLICATIONS_SHLIB_VER=	${KDE_APPLICATIONS_VERSION}

.include <bsd.port.mk>
