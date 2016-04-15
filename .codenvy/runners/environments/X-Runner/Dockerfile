#
# Copyright (c) 2012-2015 Codenvy, S.A.
# All rights reserved. This program and the accompanying materials
# are made available under the terms of the Eclipse Public License v1.0
# which accompanies this distribution, and is available at
# http://www.eclipse.org/legal/epl-v10.html
#
# Contributors:
#   Codenvy, S.A. - initial API and implementation
#

FROM codenvy/cpp_qt4
RUN sudo apt-get update
RUN sudo apt-get -y install \
	libfltk1.3-dev \
   libpng++-dev \
   libjpeg-dev \
   libxinerama-dev \
   libXft-dev \
   libfontconfig-dev \
   cmake vim

ADD $app$ /home/user/
RUN mkdir build && cd build && cmake .. && make