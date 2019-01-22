# javaRMI-Remote-method-invocation-
include Communication in Client system (java RMI) and Communication in Server system (java RMI) //  eclipse projects

Remote method invocation

* allows a thread to invoke a method on a remote object
  Remote object) an object that resides in a different JVM on the same computer or on a remote host connected by a network
* Parameter passing and return value
  - possible to pass primitive data types as well as objects
  - Local objects are passed by copy using object serialization technique which allows the state of an object to be written to a byte stream.
   // An object must implement the java.io.Serializable interface.
  - Remote objects are passed by reference.
   passing an object by reference allows the receiver to alter the state of the remote objects as well as invoke its methods.
   
* stub, skeleton, parcel
  - stub : a client-side proxy for the remote object
  - skeleton : a server-side proxy
  //It doesn't exist at the moment.
  
* Sequence RMI
  1. 코드 작성
  2. stub 생성
  3. 서버 실행
  4. 클라이언트 실행
