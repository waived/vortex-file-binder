  ///////////////////////////////
 ///// VORTEX FILE BINDER  /////
///////////////////////////////

Version: 1.1

Lanuage: Visual Basic (.NET Framework 4.8.1)

Purpose: Simple file-binding utility which aids in laundering a payload silently onto a system.

Packing method: Vortex uses XOR encryption (boolean-logic cipher) to encrypt each payload attached
                to the initial stub; additionally, the encrypted payloads are also wrapped in BASE-64
                encoding.

USG (Unique Stub Generation):
                Each stub comes packaged with unique checksums. This is in part because the XOR
                encryption key is randomly generated per each build and appended directly into
                the stub. This not only allows each stub to beat checksum tests from anti-viral
                software but ensures that each XOR encryption remains strong and less profilable.
                Each randomly generates XOR key is between 10 to 15 characters long, using alpha-
                numerical characters. The length and/or the character pool (to include special
                characters or unicode characters) can be manually expanded for increased
                security.

Please use responsibly!



