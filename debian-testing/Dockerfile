################################
# Dockerfile: thedcg/tl-debian:testing

# ベース
FROM debian:testing

################################
# Dockerfile.common

# 管理者
MAINTAINER Lemures Lemniscati <lemures.lemniscati@gmail.com>

# アップデート
RUN date --iso-8601=ns\
 && apt-get update\
 && apt-get -y upgrade\
 && apt-get -y install\
	make\
	git\
	openssh-client\
	xz-utils\
	tex-common\
	latex-cjk-all\
	texlive-lang-cjk\
	texlive-latex-extra\
	texlive-science\
	texlive-fonts-recommended\
	texlive-fonts-extra\
	texlive-metapost\
	texlive-bibtex-extra\
	texlive-publishers\
	biber\
	asymptote\
 && apt-get clean \
 && rm -rf /var/lib/apt/lists/*\
 && date --iso-8601=ns

# 終了