# aiha

**aiha** is the kesh word for _new_.

A dataflow language inspired by Tesler and Enea's [Compel](https://www.reddit.com/r/ProgrammingLanguages/comments/l1m4wr/a_language_design_for_concurrent_processes/) from 1968 and [Erlang](https://www.erlang.org/) from 1986.

Its syntax is a superset of [na](https://github.com/kesh-lang/na).

```lua
-- file: main
counter: import 'counter'
'increment' >> counter
'decrement' >> counter
```

```lua
-- file: counter
count: 0
>> 'increment' -> [count: count + 1]
>> 'decrement' -> [count: count - 1]
```

- [Creation myth](https://github.com/kesh-lang/aiha/wiki/Creation-myth)
- [Adventures of a new language](https://github.com/kesh-lang/aiha/wiki/Adventures-of-a-new-language)
