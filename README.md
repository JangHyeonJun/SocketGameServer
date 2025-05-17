# SocketGameServer
소켓 게임서버 구현

TCP Socket 기반에서 Async, Multi-thread로 구동되는 서버 구현

#### Project

1. **Server** : 서버 구현부, Listener 객체는 연결된 DummyClient에 대한 세션을 생성하여 Server.SessionManager에 관리하고 송수신 패킷을 비동기 처리
2. **ServerCore** : 서버&클라이언트 공통 라이브러리
3. **DummyClient** : 서버 접속 Dummy Client. Connector 객체는 Server에 대한 세션을 생성하여 DummyClient.SessionManger에 관리하고 송수신 패킷 비동기 처리
4. **PacketGenerator** : 서버&클라이언트 통신 패킷 프로토콜을 XML을 통해 자동으로 생성

