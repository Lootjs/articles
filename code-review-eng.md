## A few advices, for improving code review process

### What is a code review?
**Before getting started, I wanna give my definintion of a code review:**
- Code review is a discussion about a new code. It's necessary to involve the team in assessing the importance of this change.
- Code review is sharing a knowledges about a project, beacause it can reduce bus factor. In cases, when a developers don't know how works some modules, code review can fix this omission.
- Code review is a refactoring, improving code quality.
- Code review is finding logical mistakes, because auto tests can miss that errors.
- Code review is a way to integrate a culture of mentoring and mutual assistance in a team.

**And..**
- Code review is not checking a code style - it can be automated with a linters.
- Code review is not checking a auto-tests is passing - it can be automated and should be automated.

### Primary steps before making Pull Request (PR):
1. Before making PR, it would be nice to look at the code as if the code was written by your colleague, not you. This will allow you to clarify points that are obvious to you, but not clear to the reviewer.
2. When it's possible, give a brief of PR: дать бриф для PR: что это за изменение, зачем он написан, на что следует обратить внимание. Это позволит дать контекст для ревьюера, которым обладает автор: автор исследовал задачу, и знает причины изменений.

### Улучшение процесса код-ревью: 
- Ваш PR не должен быть большим, желательно не более 500 строк кода и придерживаться принципа SRP - ваше изменение затрагивает только одну зону ответственности. 
- Необходимо проводить код-ревью в утреннее время, когда ревьюер менее нагружен и не торопится поскорее уйти домой.
- Создать стандартный чеклист для проверки Pull Request, например:
  - тесты написаны логично, т.к могут быть тесты, которые проходят в 100% случаев
  - отсутствует повторное использование кода: с возрастанием проекта повышается вероятность написания велосипедов.
  - документация обновлена, при необходимости
  - проверка на производительность: некоторые языковые конструкции могут работать медленнее, и можно заранее переписать на более быстрые вариант.

### Эмоциональные аспекты при обратной связи:
- избегать повелительных форм в словах; задавать наводящие вопросы, например, спрашивать “почему ты решил написать так?” и предлагать варианты решения, желательно с примерами кода;
- комментировать код, а не автора: “тут не хватает теста” вместо “ты забыл написать тест”;
