# virtual thread 메모
- 카카오페이에서 vitual thread 관련으로 포스팅이 올라옴
- 이제 mysql 에서도 9.0 버전에서 pinning 이슈를 해결하고자 Synchronized 코드를 ReentrantLocks 으로 변경하여 반영됨
- 동시성 제어 관련으로 `spring.task.execution.simple.concurrency-limit` 이 설정에 대해서 좀 더 알아봐야함


## 참고
- https://tech.kakaopay.com/post/ro-spring-virtual-thread/
- https://stackoverflow.com/questions/77825075/how-to-limit-the-number-of-spring-async-tasks-with-virtual-threads-enabled/77825750
- https://dev.mysql.com/doc/relnotes/connector-j/en/news-9-0-0.html
