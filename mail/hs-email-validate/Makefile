# $FreeBSD$

PORTNAME=	email-validate
PORTVERSION=	2.3.2.9
PORTREVISION=	1
CATEGORIES=	mail haskell

MAINTAINER=	haskell@FreeBSD.org
COMMENT=	Validating an email address string against RFC 5322

LICENSE=	BSD3CLAUSE

DEPRECATED=		Haskell libraries are getting pushed out of the ports tree. If you are using this port for development, consider switching to cabal sandboxes (old way), cabal new-build (new way), or use devel/stack. If you believe this port shouldn't be removed, contact haskell@FreeBSD.org
EXPIRATION_DATE=	2019-04-14

USE_CABAL=	attoparsec>=0.10.0

.include "${.CURDIR}/../../lang/ghc/bsd.cabal.mk"
.include <bsd.port.mk>
