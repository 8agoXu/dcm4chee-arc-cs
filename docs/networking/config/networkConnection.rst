Network Connection
==================
Describes one TCP/UDP port on one network device.

.. tabularcolumns:: |p{4cm}|l|p{8cm}|l|
.. csv-table:: Network Connection Attributes (LDAP Object: dcmNetworkConnection)
    :header: Name, Type, Description, LDAP Attribute
    :widths: 20, 7, 60, 13

    "Name",string,"Arbitrary/Meaningful name for the Network Connection object","
    .. _cn:

    cn_"
    "**Hostname**",string,"DNS name for this particular connection","
    .. _dicomHostname:

    dicomHostname_"
    "Port",integer,"TCP/UDP port that a service is listening on. May be missing if this network connection is only used for outbound connections","
    .. _dicomPort:

    dicomPort_"
    "TLS CipherSuites(s)",string,"The TLS CipherSuites that are supported on this particular connection. If not present TLS is disabled","
    .. _dicomTLSCipherSuite:

    dicomTLSCipherSuite_"
    "installed",boolean,"True if the Network Connection is installed on the network. If not present, information about the installed status of the Network Connection is inherited from the device","
    .. _dicomInstalled:

    dicomInstalled_"
    "Protocol",string,"Protocol of Network Connection: DICOM, HL7, SYSLOG_TLS or SYSLOG_UDP; DICOM if absent","
    .. _dcmProtocol:

    dcmProtocol_"
    "HTTP Proxy",string,"HTTP Proxy: [user:password@]host:port","
    .. _dcmHTTPProxy:

    dcmHTTPProxy_"
    "TLS Need Client Auth",boolean,"Indicates if TLS client authentication is required; required if absent","
    .. _dcmTLSNeedClientAuth:

    dcmTLSNeedClientAuth_"
    "TLS Protocol",string,"The Supported TLS Protocols; TLSv1, SSLv3 if absent","
    .. _dcmTLSProtocol:

    dcmTLSProtocol_"
    "TCP Backlog",integer,"Maximum queue length for incoming TCP connections; 50 if absent","
    .. _dcmTCPBacklog:

    dcmTCPBacklog_"
    "TCP Connect Timeout",integer,"TCP connect timeout in ms; no timeout if absent","
    .. _dcmTCPConnectTimeout:

    dcmTCPConnectTimeout_"
    "TCP Close Delay",integer,"TCP socket close delay in ms after send of A-ASSOCIATE-RJ, A-RELEASE-RP or A-ABORT PDU; 50 ms if absent","
    .. _dcmTCPCloseDelay:

    dcmTCPCloseDelay_"
    "TCP Send Buffer Size",integer,"TCP send buffer size; use system defaults if absent","
    .. _dcmTCPSendBufferSize:

    dcmTCPSendBufferSize_"
    "TCP Receive Buffer Size",string,"TCP receive buffer size; use system defaults if absent","
    .. _dcmTCPReceiveBufferSize:

    dcmTCPReceiveBufferSize_"
    "TCP No Delay",boolean,"Enable/disable TCP_NODELAY (disable/enable Nagle algorithm); disable Nagle algorithm if absent","
    .. _dcmTCPNoDelay:

    dcmTCPNoDelay_"
    "Bind Address",string,"Bind address of listening socket; use hostname of the connection if absent","
    .. _dcmBindAddress:

    dcmBindAddress_"
    "Client Bind Address",string,"Bind address of outgoing connections; use hostname of the connection if absent","
    .. _dcmClientBindAddress:

    dcmClientBindAddress_"
    "Blacklisted Hostname(s)",string,"blacklisted DNS hostnames","
    .. _dcmBlacklistedHostname:

    dcmBlacklistedHostname_"
    "Send PDU Length",integer,"Maximal length of emitted PDUs; 16378 if absent","
    .. _dcmSendPDULength:

    dcmSendPDULength_"
    "Receive PDU Length",integer,"Maximal length of received PDUs; 16378 if absent","
    .. _dcmReceivePDULength:

    dcmReceivePDULength_"
    "Max Ops Performed",integer,"Maximal number of operations to perform asynchronously; 0 = infinite; 1 (=synchronous) if absent","
    .. _dcmMaxOpsPerformed:

    dcmMaxOpsPerformed_"
    "Max Ops Invoked",integer,"Maximal number of operations to invoke asynchronously; 0 = infinite; 1 (=synchronous) if absent","
    .. _dcmMaxOpsInvoked:

    dcmMaxOpsInvoked_"
    "Pack PDV",boolean,"Enable/disable packing of command and data PDVs into one P-DATA-TF PDU; enabled if absent","
    .. _dcmPackPDV:

    dcmPackPDV_"
    "AA-RQ Timeout",integer,"Timeout in ms for receive of A-ASSOCIATE-RQ PDU after TCP connect; no timeout if absent","
    .. _dcmAARQTimeout:

    dcmAARQTimeout_"
    "AA-AC Timeout",integer,"Timeout in ms for receive of A-ASSOCIATE-AC PDU after send of A-ASSOCIATE-RQ PDU; no timeout if absent","
    .. _dcmAAACTimeout:

    dcmAAACTimeout_"
    "AR-RP Timeout",integer,"Timeout in ms for receive of A-RELEASE-RP PDU after send of A-RELEASE-RQ PDU; no timeout if absent","
    .. _dcmARRPTimeout:

    dcmARRPTimeout_"
    "Response Timeout",integer,"Timeout in ms for receive of response message; no timeout if absent","
    .. _dcmResponseTimeout:

    dcmResponseTimeout_"
    "Retrieve Timeout",integer,"Timeout in ms for receive of C-GET-RSP or C-MOVE-RSP; no timeout if absent","
    .. _dcmRetrieveTimeout:

    dcmRetrieveTimeout_"
    "Idle Timeout",integer,"Indicates aborting of idle Associations after specified timeout in ms; no timeout if absent","
    .. _dcmIdleTimeout:

    dcmIdleTimeout_"
