PORTNAME=	kohana
PORTVERSION=	3.3.6
DISTVERSIONPREFIX=	v
CATEGORIES=	www
MASTER_SITES=	https://github.com/${PORTNAME}/${PORTNAME}/releases/download/${DISTVERSIONPREFIX}${DISTVERSION}/

MAINTAINER=	uzsolt@FreeBSD.org
COMMENT=	Elegant HMVC PHP5 framework
WWW=		https://kohanaframework.org/

LICENSE=	BSD3CLAUSE
LICENSE_FILE=	${WRKSRC}/LICENSE.md

DEPRECATED=	Supports only PHP5, abandoned upstream
EXPIRATION_DATE=	2024-12-01

USES=		cpe php zip
CPE_VENDOR=	${PORTNAME}framework

NO_BUILD=	yes
NO_ARCH=	yes
SUB_FILES=	pkg-message

post-patch:
	@${REINPLACE_CMD} "s,'system','${WWWDIR}/system', ; \
		s,'modules','${WWWDIR}/modules'," ${WRKSRC}/index.php

do-install:
	${MKDIR} ${STAGEDIR}${WWWDIR}
	cd ${WRKSRC} && ${COPYTREE_SHARE} "application example.htaccess \
		index.php install.php modules system" ${STAGEDIR}${WWWDIR}

.include <bsd.port.mk>
