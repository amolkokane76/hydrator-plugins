============================================
Hive Batch Source and Sink Plugin Collection
============================================

Introduction
============

This project is a collection of Hive batch source and sink plugins. These plugins are currently available:

- Hive Batch Source
- Hive Batch Sink

Getting Started
===============

Following are instructions to build and deploy the Hydrator Hive plugins.

Prerequisites
-------------

To use the plugins, you must have CDAP version 3.2.1 or later. You can download CDAP Standalone that includes Hydrator `here <http://cdap.io/downloads>`__

Build Plugins
-------------

You get started with Hydrator plugins by building directly from the latest source code::

  git clone https://github.com/cdapio/hydrator-plugins.git
  cd hydrator-plugins
  mvn clean package -pl hive-plugins -am

After the build completes, you will have a jar for each plugin under the
``hive-plugins/target/`` directory.

Deploy Plugins
--------------

You can deploy the plugins using the CDAP CLI::

  > load artifact target/hive-plugins-<version>.jar \
         config-file target/hive-plugins-<version>.json

License and Trademarks
======================

Copyright © 2015-2019 Cask Data, Inc.

Licensed under the Apache License, Version 2.0 (the "License"); you may not use this file except
in compliance with the License. You may obtain a copy of the License at

http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software distributed under the
License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND,
either express or implied. See the License for the specific language governing permissions
and limitations under the License.

Cask is a trademark of Cask Data, Inc. All rights reserved.

Apache, Apache HBase, and HBase are trademarks of The Apache Software Foundation. Used with
permission. No endorsement by The Apache Software Foundation is implied by the use of these marks.
