PORTNAME=	git-absorb
DISTVERSION=	0.6.17
PORTREVISION=	2
CATEGORIES=	devel

MAINTAINER=	eduardo@FreeBSD.org
COMMENT=	Git command for automating fixup/autosquash commits
WWW=		https://github.com/tummychow/git-absorb

LICENSE=	BSD3CLAUSE
LICENSE_FILE=	${WRKSRC}/LICENSE.md

USES=		cargo
USE_GITHUB=	yes
GH_ACCOUNT=	tummychow

PLIST_FILES=	bin/${PORTNAME} \
		share/man/man1/${PORTNAME}.1.gz

post-install:
	${INSTALL_MAN} ${WRKSRC}/Documentation/${PORTNAME}.1 \
		${STAGEDIR}${PREFIX}/share/man/man1

.include <bsd.port.mk>
