FROM postgres:14.1
# Time Zone
ENV TZ Asia/Tokyo
# Language
ARG DB_LANG=ja_JP
RUN localedef -i $DB_LANG -c -f UTF-8 -A /usr/share/locale/locale.alias $DB_LANG.UTF-8
ENV LANG $DB_LANG.utf8
ENV LANGUAGE $DB_LANG:ja
ENV LC_ALL $DB_LANG.UTF-8