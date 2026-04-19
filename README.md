```mermaid
classDiagram
    class Subject {
        +Attach(o : Observer)
        +Detach(o : Observer)
        +Notify()
    }
    class Observer {
        <<interface>>
        +Update()
    }
    class ConcreteSubject {
        -subjectstate
        +GetState()
        +SetState(state)
    }
    class ConcreteObserver {
        -observerstate
        +Update()
    }

    Subject -- Observer
    Subject <|-- ConcreteSubject
    Observer <|-- ConcreteObserver
```

<video src="./uiDemo.mp4" width="100%" controls>
  Ваш браузер не поддерживает встроенные видео. 
  Вот [ссылка на видео](path/to/your/video.mp4).
</video>
