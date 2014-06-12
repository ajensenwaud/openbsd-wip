# $OpenBSD$

COMMENT=    functional programming language based on term rewriting

DISTNAME=   pure-0.60

CATEGORIES= lang

HOMEPAGE=   http://purelang.bitbucket.org/

SHARED_LIBS +=  pure 8.0
# License: LGPLv3
PERMIT_PACKAGE_CDROM=   Yes

WANTLIB += iconv gmp mpfr pthread readline stdc++ termcap z c m

LIB_DEPENDS=    devel/gmp devel/mpfr devel/llvm

MODULES=        converters/libiconv

MASTER_SITES=   https://bitbucket.org/purelang/pure-lang/downloads/

USE_GMAKE=	Yes

SEPARATE_BUILD= Yes

CONFIGURE_STYLE= gnu

CONFIGURE_ARGS += --with-libgmp-prefix="${LOCALBASE}"

#NO_TEST=    Yes
TEST_TARGET=	check

.include <bsd.port.mk>
