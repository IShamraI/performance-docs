RPC CALL fail-over test report
------------------------------

This scenario is executed with help of oslo.messaging simulator. There is
one client-server pair of simulator running in single-threaded mode. The
stats are collected from both client and server and detailed report is shown
with one second precision.


Execution Summary
^^^^^^^^^^^^^^^^^


.. list-table::
   :header-rows: 1

   *
     - attribute
     - value
   *
     - Client sent, msg
     - 27208
   *
     - Server received, msg
     - 27208
   *
     - Client received replies, msg
     - 27208
   *
     - Loss, msg
     - 0
   *
     - Errors, msg
     - 0
   *
     - Duration, sec
     - 121.1
   *
     - Throughput, msg/sec
     - 224.7
   *
     - Transfer, Mb
     - 87.1
   *
     - Bandwidth, Mb/sec
     - 0.7
   *
     - Avg. request latency, ms
     - 2.7
   *
     - Max request latency, ms
     - 47.0
   *
     - Avg. round-trip latency, ms
     - 4.3
   *
     - Max round-trip latency, ms
     - 2050.5



Message flow
^^^^^^^^^^^^

This chart shows the message flow between client and server. It includes
messages sent by the client, received by the server, replies received by
the client and errors caught by the client.

.. image:: rpc_call_message_flow.*



where:
 * ``sent`` - messages sent by the client
 * ``received`` - messages received by the server
 * ``round-trip`` - replies to messages received by the client
 * ``errors`` - errors exposed and caught by the client


Messages sent by the client
^^^^^^^^^^^^^^^^^^^^^^^^^^^

This chart shows messages sent by client and error rate.

.. image:: rpc_call_sent_messages.*


.. list-table:: RPC CALL sent messages
   :header-rows: 1

   *
     - time
     - sent, msg
     - errors, msg
   *
     - 0
     - 1
     - 0
   *
     - 1
     - 215
     - 0
   *
     - 2
     - 226
     - 0
   *
     - 3
     - 225
     - 0
   *
     - 4
     - 227
     - 0
   *
     - 5
     - 229
     - 0
   *
     - 6
     - 229
     - 0
   *
     - 7
     - 227
     - 0
   *
     - 8
     - 226
     - 0
   *
     - 9
     - 227
     - 0
   *
     - 10
     - 225
     - 0
   *
     - 11
     - 227
     - 0
   *
     - 12
     - 228
     - 0
   *
     - 13
     - 149
     - 0
   *
     - 14
     - .
     - 0
   *
     - 15
     - 59
     - 0
   *
     - 16
     - 223
     - 0
   *
     - 17
     - 240
     - 0
   *
     - 18
     - 241
     - 0
   *
     - 19
     - 256
     - 0
   *
     - 20
     - 255
     - 0
   *
     - 21
     - 249
     - 0
   *
     - 22
     - 247
     - 0
   *
     - 23
     - 192
     - 0
   *
     - 24
     - 240
     - 0
   *
     - 25
     - 222
     - 0
   *
     - 26
     - 229
     - 0
   *
     - 27
     - 227
     - 0
   *
     - 28
     - 229
     - 0
   *
     - 29
     - 225
     - 0
   *
     - 30
     - 227
     - 0
   *
     - 31
     - 219
     - 0
   *
     - 32
     - 226
     - 0
   *
     - 33
     - 218
     - 0
   *
     - 34
     - 231
     - 0
   *
     - 35
     - 229
     - 0
   *
     - 36
     - 230
     - 0
   *
     - 37
     - 227
     - 0
   *
     - 38
     - 221
     - 0
   *
     - 39
     - 233
     - 0
   *
     - 40
     - 245
     - 0
   *
     - 41
     - 240
     - 0
   *
     - 42
     - 245
     - 0
   *
     - 43
     - 241
     - 0
   *
     - 44
     - 239
     - 0
   *
     - 45
     - 242
     - 0
   *
     - 46
     - 246
     - 0
   *
     - 47
     - 232
     - 0
   *
     - 48
     - 245
     - 0
   *
     - 49
     - 236
     - 0
   *
     - 50
     - 231
     - 0
   *
     - 51
     - 229
     - 0
   *
     - 52
     - 242
     - 0
   *
     - 53
     - 238
     - 0
   *
     - 54
     - 246
     - 0
   *
     - 55
     - 241
     - 0
   *
     - 56
     - 246
     - 0
   *
     - 57
     - 239
     - 0
   *
     - 58
     - 245
     - 0
   *
     - 59
     - 155
     - 0
   *
     - 60
     - 77
     - 0
   *
     - 61
     - 240
     - 0
   *
     - 62
     - 240
     - 0
   *
     - 63
     - 243
     - 0
   *
     - 64
     - 238
     - 0
   *
     - 65
     - 229
     - 0
   *
     - 66
     - 224
     - 0
   *
     - 67
     - 236
     - 0
   *
     - 68
     - 231
     - 0
   *
     - 69
     - 235
     - 0
   *
     - 70
     - 244
     - 0
   *
     - 71
     - 250
     - 0
   *
     - 72
     - 257
     - 0
   *
     - 73
     - 250
     - 0
   *
     - 74
     - 245
     - 0
   *
     - 75
     - 237
     - 0
   *
     - 76
     - 240
     - 0
   *
     - 77
     - 234
     - 0
   *
     - 78
     - 225
     - 0
   *
     - 79
     - 228
     - 0
   *
     - 80
     - 224
     - 0
   *
     - 81
     - 230
     - 0
   *
     - 82
     - 225
     - 0
   *
     - 83
     - 230
     - 0
   *
     - 84
     - 226
     - 0
   *
     - 85
     - 222
     - 0
   *
     - 86
     - 223
     - 0
   *
     - 87
     - 224
     - 0
   *
     - 88
     - 219
     - 0
   *
     - 89
     - 227
     - 0
   *
     - 90
     - 228
     - 0
   *
     - 91
     - 229
     - 0
   *
     - 92
     - 229
     - 0
   *
     - 93
     - 228
     - 0
   *
     - 94
     - 234
     - 0
   *
     - 95
     - 235
     - 0
   *
     - 96
     - 238
     - 0
   *
     - 97
     - 236
     - 0
   *
     - 98
     - 237
     - 0
   *
     - 99
     - 238
     - 0
   *
     - 100
     - 240
     - 0
   *
     - 101
     - 230
     - 0
   *
     - 102
     - 242
     - 0
   *
     - 103
     - 234
     - 0
   *
     - 104
     - 236
     - 0
   *
     - 105
     - 241
     - 0
   *
     - 106
     - 238
     - 0
   *
     - 107
     - 238
     - 0
   *
     - 108
     - 239
     - 0
   *
     - 109
     - 231
     - 0
   *
     - 110
     - 232
     - 0
   *
     - 111
     - 231
     - 0
   *
     - 112
     - 227
     - 0
   *
     - 113
     - 224
     - 0
   *
     - 114
     - 221
     - 0
   *
     - 115
     - 219
     - 0
   *
     - 116
     - 223
     - 0
   *
     - 117
     - 224
     - 0
   *
     - 118
     - 229
     - 0
   *
     - 119
     - 232
     - 0
   *
     - 120
     - 213
     - 0


Messages received by the server
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

This chart shows messages received by the server and their latency.

.. image:: rpc_call_received_messages.*


.. list-table:: RPC CALL received messages
   :header-rows: 1

   *
     - time
     - sent, msg
     - latency, ms
   *
     - 0
     - 0
     - .
   *
     - 1
     - 0
     - .
   *
     - 2
     - 214
     - 3.0
   *
     - 3
     - 226
     - 2.8
   *
     - 4
     - 225
     - 2.8
   *
     - 5
     - 227
     - 2.8
   *
     - 6
     - 228
     - 2.8
   *
     - 7
     - 230
     - 2.7
   *
     - 8
     - 226
     - 2.8
   *
     - 9
     - 226
     - 2.8
   *
     - 10
     - 227
     - 2.8
   *
     - 11
     - 225
     - 2.8
   *
     - 12
     - 226
     - 2.8
   *
     - 13
     - 228
     - 2.8
   *
     - 14
     - 153
     - 2.8
   *
     - 15
     - 0
     - .
   *
     - 16
     - 55
     - 3.2
   *
     - 17
     - 223
     - 2.9
   *
     - 18
     - 241
     - 2.7
   *
     - 19
     - 240
     - 2.7
   *
     - 20
     - 257
     - 2.5
   *
     - 21
     - 255
     - 2.5
   *
     - 22
     - 249
     - 2.6
   *
     - 23
     - 247
     - 2.6
   *
     - 24
     - 192
     - 3.6
   *
     - 25
     - 240
     - 2.7
   *
     - 26
     - 222
     - 3.0
   *
     - 27
     - 229
     - 2.9
   *
     - 28
     - 226
     - 2.9
   *
     - 29
     - 230
     - 2.9
   *
     - 30
     - 224
     - 3.0
   *
     - 31
     - 227
     - 2.9
   *
     - 32
     - 219
     - 3.1
   *
     - 33
     - 226
     - 2.9
   *
     - 34
     - 218
     - 3.1
   *
     - 35
     - 232
     - 2.9
   *
     - 36
     - 228
     - 2.9
   *
     - 37
     - 230
     - 2.9
   *
     - 38
     - 227
     - 3.0
   *
     - 39
     - 221
     - 3.1
   *
     - 40
     - 233
     - 2.8
   *
     - 41
     - 245
     - 2.6
   *
     - 42
     - 240
     - 2.7
   *
     - 43
     - 244
     - 2.6
   *
     - 44
     - 241
     - 2.7
   *
     - 45
     - 240
     - 2.7
   *
     - 46
     - 241
     - 2.7
   *
     - 47
     - 247
     - 2.6
   *
     - 48
     - 231
     - 2.8
   *
     - 49
     - 245
     - 2.6
   *
     - 50
     - 237
     - 2.7
   *
     - 51
     - 230
     - 2.8
   *
     - 52
     - 229
     - 2.8
   *
     - 53
     - 242
     - 2.7
   *
     - 54
     - 239
     - 2.7
   *
     - 55
     - 246
     - 2.6
   *
     - 56
     - 241
     - 2.7
   *
     - 57
     - 246
     - 2.6
   *
     - 58
     - 238
     - 2.7
   *
     - 59
     - 245
     - 2.6
   *
     - 60
     - 160
     - 2.8
   *
     - 61
     - 72
     - 2.7
   *
     - 62
     - 240
     - 2.6
   *
     - 63
     - 240
     - 2.6
   *
     - 64
     - 242
     - 2.5
   *
     - 65
     - 239
     - 2.6
   *
     - 66
     - 229
     - 2.7
   *
     - 67
     - 224
     - 2.8
   *
     - 68
     - 236
     - 2.6
   *
     - 69
     - 231
     - 2.6
   *
     - 70
     - 235
     - 2.6
   *
     - 71
     - 243
     - 2.6
   *
     - 72
     - 251
     - 2.5
   *
     - 73
     - 256
     - 2.4
   *
     - 74
     - 250
     - 2.5
   *
     - 75
     - 245
     - 2.6
   *
     - 76
     - 237
     - 2.6
   *
     - 77
     - 240
     - 2.6
   *
     - 78
     - 234
     - 2.7
   *
     - 79
     - 225
     - 2.8
   *
     - 80
     - 229
     - 2.7
   *
     - 81
     - 223
     - 2.8
   *
     - 82
     - 230
     - 2.7
   *
     - 83
     - 225
     - 2.8
   *
     - 84
     - 230
     - 2.7
   *
     - 85
     - 226
     - 2.8
   *
     - 86
     - 223
     - 2.7
   *
     - 87
     - 223
     - 2.8
   *
     - 88
     - 224
     - 2.8
   *
     - 89
     - 219
     - 2.9
   *
     - 90
     - 225
     - 2.7
   *
     - 91
     - 229
     - 2.7
   *
     - 92
     - 229
     - 2.7
   *
     - 93
     - 228
     - 2.7
   *
     - 94
     - 229
     - 2.7
   *
     - 95
     - 234
     - 2.7
   *
     - 96
     - 235
     - 2.7
   *
     - 97
     - 237
     - 2.6
   *
     - 98
     - 236
     - 2.6
   *
     - 99
     - 237
     - 2.6
   *
     - 100
     - 238
     - 2.6
   *
     - 101
     - 240
     - 2.6
   *
     - 102
     - 230
     - 2.7
   *
     - 103
     - 244
     - 2.5
   *
     - 104
     - 231
     - 2.7
   *
     - 105
     - 237
     - 2.6
   *
     - 106
     - 240
     - 2.6
   *
     - 107
     - 238
     - 2.6
   *
     - 108
     - 238
     - 2.6
   *
     - 109
     - 240
     - 2.6
   *
     - 110
     - 230
     - 2.7
   *
     - 111
     - 232
     - 2.7
   *
     - 112
     - 231
     - 2.7
   *
     - 113
     - 227
     - 2.8
   *
     - 114
     - 224
     - 2.8
   *
     - 115
     - 221
     - 2.8
   *
     - 116
     - 219
     - 2.9
   *
     - 117
     - 223
     - 2.8
   *
     - 118
     - 224
     - 2.8
   *
     - 119
     - 228
     - 2.7
   *
     - 120
     - 233
     - 2.7
   *
     - 121
     - 221
     - 2.7
   *
     - 122
     - 0
     - .


Replies received by the client
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

This chart shows replies received by the client and total round-trip latency.

.. image:: rpc_call_round_trip_messages.*


.. list-table:: RPC CALL round-trip messages
   :header-rows: 1

   *
     - time
     - round-trip, msg
     - latency, ms
   *
     - 0
     - 0
     - .
   *
     - 1
     - 215
     - 4.6
   *
     - 2
     - 226
     - 4.4
   *
     - 3
     - 225
     - 4.4
   *
     - 4
     - 227
     - 4.3
   *
     - 5
     - 229
     - 4.3
   *
     - 6
     - 229
     - 4.3
   *
     - 7
     - 227
     - 4.4
   *
     - 8
     - 225
     - 4.4
   *
     - 9
     - 227
     - 4.3
   *
     - 10
     - 225
     - 4.4
   *
     - 11
     - 227
     - 4.4
   *
     - 12
     - 228
     - 4.3
   *
     - 13
     - 150
     - 4.4
   *
     - 14
     - 0
     - .
   *
     - 15
     - 58
     - 40.1
   *
     - 16
     - 223
     - 4.4
   *
     - 17
     - 241
     - 4.1
   *
     - 18
     - 240
     - 4.1
   *
     - 19
     - 257
     - 3.8
   *
     - 20
     - 255
     - 3.9
   *
     - 21
     - 249
     - 4.0
   *
     - 22
     - 247
     - 4.0
   *
     - 23
     - 191
     - 5.2
   *
     - 24
     - 241
     - 4.1
   *
     - 25
     - 221
     - 4.5
   *
     - 26
     - 230
     - 4.3
   *
     - 27
     - 226
     - 4.4
   *
     - 28
     - 230
     - 4.3
   *
     - 29
     - 224
     - 4.4
   *
     - 30
     - 227
     - 4.3
   *
     - 31
     - 219
     - 4.5
   *
     - 32
     - 226
     - 4.4
   *
     - 33
     - 218
     - 4.5
   *
     - 34
     - 232
     - 4.3
   *
     - 35
     - 228
     - 4.3
   *
     - 36
     - 230
     - 4.3
   *
     - 37
     - 227
     - 4.4
   *
     - 38
     - 222
     - 4.5
   *
     - 39
     - 232
     - 4.2
   *
     - 40
     - 245
     - 4.0
   *
     - 41
     - 241
     - 4.1
   *
     - 42
     - 244
     - 4.0
   *
     - 43
     - 241
     - 4.1
   *
     - 44
     - 239
     - 4.1
   *
     - 45
     - 242
     - 4.1
   *
     - 46
     - 247
     - 4.0
   *
     - 47
     - 232
     - 4.3
   *
     - 48
     - 244
     - 4.0
   *
     - 49
     - 237
     - 4.2
   *
     - 50
     - 230
     - 4.3
   *
     - 51
     - 229
     - 4.3
   *
     - 52
     - 242
     - 4.1
   *
     - 53
     - 239
     - 4.1
   *
     - 54
     - 245
     - 4.0
   *
     - 55
     - 242
     - 4.1
   *
     - 56
     - 246
     - 4.0
   *
     - 57
     - 239
     - 4.1
   *
     - 58
     - 244
     - 4.0
   *
     - 59
     - 156
     - 4.2
   *
     - 60
     - 77
     - 17.4
   *
     - 61
     - 239
     - 4.1
   *
     - 62
     - 240
     - 4.1
   *
     - 63
     - 243
     - 4.1
   *
     - 64
     - 239
     - 4.1
   *
     - 65
     - 228
     - 4.3
   *
     - 66
     - 225
     - 4.4
   *
     - 67
     - 235
     - 4.2
   *
     - 68
     - 232
     - 4.3
   *
     - 69
     - 235
     - 4.2
   *
     - 70
     - 243
     - 4.1
   *
     - 71
     - 251
     - 3.9
   *
     - 72
     - 256
     - 3.9
   *
     - 73
     - 250
     - 4.0
   *
     - 74
     - 245
     - 4.0
   *
     - 75
     - 237
     - 4.2
   *
     - 76
     - 240
     - 4.1
   *
     - 77
     - 234
     - 4.2
   *
     - 78
     - 225
     - 4.4
   *
     - 79
     - 229
     - 4.3
   *
     - 80
     - 223
     - 4.4
   *
     - 81
     - 230
     - 4.3
   *
     - 82
     - 225
     - 4.4
   *
     - 83
     - 230
     - 4.3
   *
     - 84
     - 226
     - 4.4
   *
     - 85
     - 223
     - 4.4
   *
     - 86
     - 223
     - 4.4
   *
     - 87
     - 224
     - 4.4
   *
     - 88
     - 219
     - 4.5
   *
     - 89
     - 226
     - 4.4
   *
     - 90
     - 229
     - 4.3
   *
     - 91
     - 229
     - 4.3
   *
     - 92
     - 228
     - 4.3
   *
     - 93
     - 229
     - 4.3
   *
     - 94
     - 234
     - 4.2
   *
     - 95
     - 235
     - 4.2
   *
     - 96
     - 238
     - 4.1
   *
     - 97
     - 236
     - 4.2
   *
     - 98
     - 237
     - 4.2
   *
     - 99
     - 238
     - 4.1
   *
     - 100
     - 240
     - 4.1
   *
     - 101
     - 230
     - 4.3
   *
     - 102
     - 242
     - 4.1
   *
     - 103
     - 233
     - 4.2
   *
     - 104
     - 237
     - 4.2
   *
     - 105
     - 240
     - 4.1
   *
     - 106
     - 239
     - 4.1
   *
     - 107
     - 237
     - 4.1
   *
     - 108
     - 240
     - 4.1
   *
     - 109
     - 230
     - 4.3
   *
     - 110
     - 233
     - 4.2
   *
     - 111
     - 230
     - 4.3
   *
     - 112
     - 227
     - 4.3
   *
     - 113
     - 224
     - 4.4
   *
     - 114
     - 221
     - 4.5
   *
     - 115
     - 219
     - 4.5
   *
     - 116
     - 223
     - 4.4
   *
     - 117
     - 224
     - 4.4
   *
     - 118
     - 229
     - 4.3
   *
     - 119
     - 232
     - 4.2
   *
     - 120
     - 215
     - 4.3
