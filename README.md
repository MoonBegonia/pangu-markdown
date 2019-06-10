# Pangu Markdown

偶然发现了这个不错的插件，但是似乎作者已经弃坑了，提 issue 没有回应，便决定 fock 一份自己动手，丰衣足食。（与原版冲突，不可同时使用）

## Function

1. Add whitespace between Chinese and English
2. Add whitespace between Chinese and `[ ]`
3. `, \ . : ; ? !` after Chinese characters to `，、。：；？！`
4. `()` around Chinese characters to `（）`
    - ``[] <> ` `` remains untouched
5. Continuous `。`(at least 3) to `......`, e.g. `。` to `......`
6. Truncate more than three continuous `？ ！` to only three ones.
7. Truncate continuous `。，；：、“”『』〖〗《》` to only one.

Note that all functions are based on Regex, it cannot do brace match, thus it lacks the ability to handle very complex cases, but it's enough for normal use. Maybe improve in the future.

## Usage

```
Ctrl+Shift+P -> Pangu Format
```

or

```
F1 -> Pangu Format
```

Or

```
Right Click in editor (when open markdown file) -> Pangu Format
```

## Setting

| Name                      | Description                     |
| :------------------------ | :------------------------------ |
| pangu.auto_format_on_save | Auto apply Pangu format on save |

## Thanks

Thanks to [pangu.vim](https://github.com/hotoo/pangu.vim), [writing4cn](https://marketplace.visualstudio.com/items?itemName=twocucao.writing4cn) and [pangu](https://marketplace.visualstudio.com/items?itemName=halfcrazy.pangu).