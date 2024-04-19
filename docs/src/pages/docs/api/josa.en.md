---
title: josa
---

# josa

Attaches particles to a Hangul string such as '이/가', '을/를', '은/는', '으로/로', '와/과', '이나/나', 이란/란, 아/야, '이랑/랑', '이에요/예요', '으로서/로서', '으로써/로써', '으로부터/로부터'.

```typescript
function josa(
  // The Hangul string to attach the particle to
  word: string,
  // The particle to attach
  josa:
    | '이/가'
    | '을/를'
    | '은/는'
    | '으로/로'
    | '와/과'
    | '이나/나'
    | '이에/에'
    | '이란/란'
    | '아/야'
    | '이랑/랑'
    | '이에요/예요'
    | '으로서/로서'
    | '으로써/로써'
    | '으로부터/로부터'
): string;
```

## Examples

```typescript
josa('샴푸', '이/가'); // '샴푸가'
josa('칫솔', '이/가'); // '칫솔이'
josa('바깥', '으로/로'); // '바깥으로'
josa('내부', '으로/로'); // '내부로'
```