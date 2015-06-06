ec2 container stack
====

Ok.

use
====

    $ cd gin &&\
      docker build -t gin-ec2 . &&\
      docker run --name gin -p 9000 -d gin-ec2

    $ cd blgse &&\
      docker build -t blgse-ec2 . &&\
      docker run --name blgse -p 9000 -d blgse-ec2

    $ cd ecic &&\
      docker build -t ecic-ec2 . &&\
      docker run --name ecic -p 9000 -d ecic-ec2

    $ cd nginx &&\
      docker build -t nginx-ec2 . &&\
      docker run --name nginx \
      --link gin:gin-proxy \
      --link blgse:blgse-ec2 \
      --link ecic:ecic-ec2 \
      -p 80:80 \
      -d nginx-ec2


