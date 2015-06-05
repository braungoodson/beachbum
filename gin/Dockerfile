FROM silarsis/yeoman
RUN git clone https://github.com/braungoodson/gin
WORKDIR /home/yeoman/gin
RUN git checkout backyard
RUN bower install
RUN npm install
CMD grunt serve:dist --force
