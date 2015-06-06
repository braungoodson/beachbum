FROM silarsis/yeoman
RUN git clone https://github.com/braungoodson/ecic
WORKDIR /home/yeoman/ecic
RUN git checkout master
RUN bower install
RUN npm install
#CMD grunt build:dist &&\
CMD grunt serve:dist --force
