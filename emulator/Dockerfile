FROM vgaidarji/docker-android-emulator:1.0.0

RUN echo "\n24333f8a63b6825ea9c5514f83c2829b004d1fee" > /opt/android-sdk/licenses/android-sdk-license
RUN echo 'y' | android update sdk --no-ui --all --filter "build-tools-28.0.3"
RUN echo 'y' | android update sdk --no-ui --all --filter "android-29"
RUN echo 'y' | android update sdk -a -u -t "sys-img-x86-google_apis_playstore-29"

###################
# GitHub Action description
###################
LABEL "com.github.actions.name"="Android Emulator"
LABEL "com.github.actions.description"="Run UI tests on Android emulator"
LABEL "com.github.actions.icon"="smartphone"
LABEL "com.github.actions.color"="green"

LABEL "repository"="https://github.com/vgaidarji/android-github-actions/emulator"
LABEL "homepage"="https://github.com/vgaidarji/android-github-actions"
LABEL "maintainer"="Veaceslav Gaidarji <veaceslav.gaidarji@gmail.com>"

COPY entrypoint.sh /

ENTRYPOINT ["/entrypoint.sh"]
CMD ["ui-tests-on-emulator"]
