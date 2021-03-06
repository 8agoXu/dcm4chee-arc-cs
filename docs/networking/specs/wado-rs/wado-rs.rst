WADO-RS Specifications
^^^^^^^^^^^^^^^^^^^^^^

.. _wado-rs-retrieve-study:

WADO-RS Retrieve Study
""""""""""""""""""""""

.. csv-table:: WADO-RS Retrieve Study
   :header: "Options", "Restrictions"
   :file: retrieve-study-series-instance.csv

.. _wado-rs-retrieve-series:

WADO-RS Retrieve Series
"""""""""""""""""""""""

.. csv-table:: WADO-RS Retrieve Series
   :header: "Options", "Restrictions"
   :file: retrieve-study-series-instance.csv

.. _wado-rs-retrieve-instance:

WADO-RS Retrieve Instance
"""""""""""""""""""""""""

.. csv-table:: WADO-RS Retrieve Instance
   :header: "Options", "Restrictions"
   :file: retrieve-study-series-instance.csv

.. _wado-rs-retrieve-frames:

WADO-RS Retrieve Frames
"""""""""""""""""""""""

.. csv-table:: WADO-RS Retrieve Frames
   :header: "Options", "Restrictions"
   :file: retrieve-frames.csv

.. _wado-rs-retrieve-bulkdata:

WADO-RS Retrieve Bulk Data
""""""""""""""""""""""""""

.. csv-table:: WADO-RS Retrieve Bulk Data
   :header: "Options", "Restrictions"
   :file: retrieve-bulkdata.csv

.. _wado-rs-retrieve-metadata:

WADO-RS Retrieve Metadata
"""""""""""""""""""""""""

.. csv-table:: WADO-RS Retrieve Metadata
   :header: "Options", "Restrictions"
   :file: retrieve-metadata.csv

.. _wado-rs-connection-policies:

WADO-RS Connection Policies
"""""""""""""""""""""""""""

.. _wado-rs-general:

General
'''''''
All standard RS connection policies apply. There are no extensions for RS options.

.. _wado-rs-number-of-connections:

Number Of Connections
'''''''''''''''''''''
DCM4CHEE-WADO-SERVICE limits the number of simultaneous RS requests. Additional requests will be queued after the HTTP connection is accepted. When an earlier request completes, a pending request will proceed.

.. csv-table:: Number of HTTP Requests Supported
   :file: common/qido-rs-stow-rs-wado-uri-wado-rs-number-of-connections.csv

.. _wado-rs-asynchronous-nature:

Asynchronous Nature
'''''''''''''''''''
DCM4CHEE-WADO-SERVICE does not support RS asynchronous response.