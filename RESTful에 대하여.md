# RESTful에 대하여

## 20.01.02 (목) 



---

###### 참고자료

1) [RESTful API란? - 가그린민트](https://brainbackdoor.tistory.com/53)

2) [REST API 제대로 알고 사용하기 - TOAST Meetup!](https://meetup.toast.com/posts/92)

3) [REST - 위키백과](https://ko.wikipedia.org/wiki/REST)

4) [[HTTP] REST API란 -velog]([https://velog.io/@wlsdud2194/HTTP-REST-API-%EB%9E%80](https://velog.io/@wlsdud2194/HTTP-REST-API-란))

---



0. 사전적 정의

   * REST == REpresentational State Transfer<del>(대표적인 상태 전달)</del>의 줄임말
   * 웹에 존재하는 모든 자원(이미지, 동영상, DB 자원 등)에 고유한 URI를 부여해 활용하는 것
   * 자원을 정의하고 자원에 대한 주소를 지정하는 방법론을 의미
   * 소프트웨어 프로그램 아키텍쳐의 한 형식
   * 따라서, Restful API는 REST 특징을 지키면서 API를 제공하는 것을 의미
   * 일종의 Coding Convention이랄까. 설계원칙, 가이드를 지키면서 개발을 하자는 의미

   

1. Why REST? 왜 REST 개념이 나왔을까...

   * 애플리케이션 분리 및 통합 & 다양한 클라이언트의 등장
   * 애플리케이션의 복잡도가 증가하면서 애플리케이션을 어떻게 분리하고 통합하느냐가 주요 이슈가 됨
   * 참고) 자바 - [과거] EJB(Enterprise Java Beans), SOA(Service Oriented Architecture)
                          [최근] MSA(Micro Service Architecture)와 함께 REST가 떠오름
   * 모바일과 같은 다양한 클라이언트의 등장하면서 Backend 하나로 다양한 Device를 대응하기 위해 REST의 필요성이 증대

   

2. REST 구성

   * 자원(Resorce) - URL

     * ```
       {
       	id : 123,
       	...
       }
       ```

   * 행위(Verb) - HTTP Method

     * CRUD(DELETE, PUT, POST, GET)

   * 표현(Representations)

     * https://www.naver.com