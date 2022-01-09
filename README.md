# aiha

**aiha** is the kesh word for _new_.

A dataflow language inspired by [Tesler](https://en.wikipedia.org/wiki/Larry_Tesler) and [Enea](https://de-m-wikipedia-org.translate.goog/wiki/Horace_Enea?_x_tr_sl=de&_x_tr_tl=en&_x_tr_hl=no)'s [Compel](https://www.reddit.com/r/ProgrammingLanguages/comments/l1m4wr/a_language_design_for_concurrent_processes/) from 1968 and [Armstrong](https://en.wikipedia.org/wiki/Joe_Armstrong_(programmer)) [et al](https://www.erlang.org/faq/academic.html#idm1175)'s [Erlang](https://www.erlang.org/) from 1986.

![](https://github.com/kesh-lang/aiha/blob/main/aiha-code.png)

```lua
-- filename: counter

count: 0

>> (sender, _increment_) ->
    count: count + 1
    sender << count
    = [count]
  
>> (sender, _decrement_) ->
    count: count - 1
    sender << count
    = [count]
```

Its syntax is a superset of [na](https://github.com/kesh-lang/na).

- [Creation myth](https://github.com/kesh-lang/aiha/wiki/Creation-myth)
- [Adventures of a new language](https://github.com/kesh-lang/aiha/wiki/Adventures-of-a-new-language)
