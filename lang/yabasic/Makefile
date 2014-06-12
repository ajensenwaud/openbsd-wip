# $OpenBSD$

COMMENT=	yet another BASIC interpreter

DISTNAME=	yabasic-2.768

CATEGORIES=	lang

HOMEPAGE=	http://www.yabasic.de/

# Dual: Artistic/GPLv2
PERMIT_PACKAGE_CDROM=	Yes

WANTLIB += ICE SM X11 c curses m ncurses

MASTER_SITES=	http://www.yabasic.de/download/

SEPARATE_BUILD=	Yes
CONFIGURE_STYLE= gnu
CONFIGURE_ENV=	CPPFLAGS="-I${X11BASE}/include" \
		LDFLAGS="-L${X11BASE}/lib"
NO_TEST=	Yes

.include <bsd.port.mk>
