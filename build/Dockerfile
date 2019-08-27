FROM ishubhamsinghtj/docker-android-build:1.1.0

###################
# GitHub Action description
###################
LABEL "com.github.actions.name"="Android Build"
LABEL "com.github.actions.description"="Build Android projects"
LABEL "com.github.actions.icon"="box"
LABEL "com.github.actions.color"="green"

LABEL "repository"="https://github.com/ishubhamsinghtj/android-github-actions/build"
LABEL "homepage"="https://github.com/ishubhamsinghtj/android-github-actions"
LABEL "maintainer"="Veaceslav Gaidarji <veaceslav.gaidarji@gmail.com>"

COPY entrypoint.sh /
ENTRYPOINT ["/entrypoint.sh"]
