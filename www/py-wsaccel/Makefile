PORTNAME=	wsaccel
DISTVERSION=	0.6.7
CATEGORIES=	www python
MASTER_SITES=	PYPI
PKGNAMEPREFIX=	${PYTHON_PKGNAMEPREFIX}

MAINTAINER=	bofh@FreeBSD.org
COMMENT=	WebSocket Accelerator for ws4py and AutobahnPython
WWW=		https://github.com/methane/wsaccel

LICENSE=	APACHE20
LICENSE_FILE=	${WRKSRC}/LICENSE

DEPRECATED=	Upstream ceased development

USES=		python
USE_PYTHON=	autoplist distutils pytest

post-install:
	${STRIP_CMD} ${STAGEDIR}${PYTHON_SITELIBDIR}/${PORTNAME}/utf8validator*.so
	${STRIP_CMD} ${STAGEDIR}${PYTHON_SITELIBDIR}/${PORTNAME}/xormask*.so

.include <bsd.port.mk>
