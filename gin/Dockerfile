FROM silarsis/yeoman

RUN git clone https://github.com/braungoodson/gin
WORKDIR /home/yeoman/gin
RUN git checkout backyard
RUN npm install
RUN bower install
RUN rm -rf client/components/startbootstrap-creative
#RUN git clone https://github.com/ironsummitmedia/startbootstrap-creative client/components/startbootstrap-creative
CMD grunt serve:dist --force
