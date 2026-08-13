# Ответы на задание 'Инструменты Git'

## 1. Коммит с хешем, начинающимся на aefea

```
git log --oneline | findstr aefea
aefead2207 Update CHANGELOG.md

git log --format=format:"%H %s" | findstr aefead2207
aefead2207ef7e2aa5dc81a34aedf0cad4c32545 Update CHANGELOG.md
```

- Полный хеш: aefead2207ef7e2aa5dc81a34aedf0cad4c32545
- Комментарий: Update CHANGELOG.md

## 2. Тег коммита 85024d3
При выполнении команды `git tag --contains 85024d3` были получены следующие теги:
- v0.12.23
- v0.12.24
- v0.12.25
- v0.12.26
- v0.12.27
- v0.12.28
- v0.12.29
- v0.12.30
- v0.12.31
Самым ранним (первым) тегом, который включает данный коммит, является v0.12.23, что указывает на то, что коммит был сделан до выхода этой версии и вошел в неё.

## 3. Родители коммита b8d720

```
git log --pretty=%P -n 1 b8d720
56cd7859e05c36c06b56d013b55a252d0bb7e158 9ea88f22fc6269854151c571162c5bcf958bee2b
```

- Количество родителей: 2
- Хеши родителей: 56cd7859e05c36c06b56d013b55a252d0bb7e158, 9ea88f22fc6269854151c571162c5bcf958bee2b

## 4. Коммиты между v0.12.23 и v0.12.24

```
git log --oneline v0.12.23..v0.12.24
33ff1c03bb (tag: v0.12.24) v0.12.24
b14b74c493 [Website] vmc provider links
3f235065b9 Update CHANGELOG.md
6ae64e247b registry: Fix panic when server is unreachable
5c619ca1ba website: Remove links to the getting started guide's old location
06275647e2 Update CHANGELOG.md
d5f9411f51 command: Fix bug when using terraform login on Windows
4b6d06cc5d Update CHANGELOG.md
dd01a35078 Update CHANGELOG.md
225466bc3e Cleanup after v0.12.23 release
```

## 5. Коммит создания функции providerSource

```
git log -S "func providerSource" --oneline
5af1e6234a main: Honor explicit provider_installation CLI config when present
8c928e8358 main: Consult local directories as potential mirrors of providers
```

Берем самый ранний коммит:
- Хеш: 8c928e8358
- Комментарий: main: Consult local directories as potential mirrors of providers

## 6. Коммиты с изменением globalPluginDirs

```
git log -S "func globalPluginDirs" --oneline
7c4aeac5f3 stacks: load credentials from config file on startup (#35952)
8364383c35 Push plugin discovery down into command package
```

## 7. Автор synchronizedWriters

```
git log -S "func synchronizedWriters" --oneline
bdfea50cc8 remove unused
5ac311e2a9 main: synchronize writes to VT100-faker on Windows

git show --pretty="%an <%ae>" 5ac311e2a9
Martin Atkins <mart@degeneration.co.uk>
```

Берем самый ранний коммит:
- Имя: Martin Atkins
- Email: mart@degeneration.co.uk