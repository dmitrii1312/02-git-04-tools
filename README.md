# 02-git-04-tools
## 1. Полный хеш и комментарий коммита, хеш которого начинается на aefea
aefead2207ef7e2aa5dc81a34aedf0cad4c32545

Update CHANGELOG.md
	
	git log aefea -1 --pretty='format:%H%n %s %b'


## 2. Тег коммита 85024d3
tag: v0.12.23
	
	git log 85024d3 -1

commit 85024d3100126de36331c6982bfaac02cdab9e76 (tag: v0.12.23)


## 3. Родители коммита b8d720
Родителей 2:

	56cd7859e05c36c06b56d013b55a252d0bb7e158
	9ea88f22fc6269854151c571162c5bcf958bee2b
	
	git log b8d720 -1 --parents

## 4. Хеши и комментарии всех коммитов которые были сделаны между тегами v0.12.23 и v0.12.24.
	git log v0.12.23^..v0.12.24 --pretty='format:%H%n %s %b'
33ff1c03bb960b332be3af2e333462dde88b279e

v0.12.24

b14b74c4939dcab573326f4e3ee2a62e23e12f89

[Website] vmc provider links

3f235065b9347a758efadc92295b540ee0a5e26e

Update CHANGELOG.md

33ff1c03bb960b332be3af2e333462dde88b279e

v0.12.24

b14b74c4939dcab573326f4e3ee2a62e23e12f89

[Website] vmc provider links

3f235065b9347a758efadc92295b540ee0a5e26e

Update CHANGELOG.md

6ae64e247b332925b872447e9ce869657281c2bf

registry: Fix panic when server is unreachable Non-HTTP errors previously resulted in a panic due to dereferencing the

resp pointer while it was nil, as part of rendering the error message.

This commit changes the error message formatting to cope with a nil

response, and extends test coverage.



Fixes #24384



5c619ca1baf2e21a155fcdb4c264cc9e24a2a353

website: Remove links to the getting started guide's old location Since these links were in the soon-to-be-deprecated 0.11 language section, I

think we can just remove them without needing to find an equivalent link.



06275647e2b53d97d4f0a19a0fec11f6d69820b5

Update CHANGELOG.md

d5f9411f5108260320064349b757f55c09bc4b80

command: Fix bug when using terraform login on Windows

4b6d06cc5dcb78af637bbb19c198faff37a066ed

Update CHANGELOG.md

dd01a35078f040ca984cdd349f18d0b67e486c35

Update CHANGELOG.md

225466bc3e5f35baa5d07197bbc079345b77525e

Cleanup after v0.12.23 release

85024d3100126de36331c6982bfaac02cdab9e76

v0.12.23



## 5. Коммит в котором была создана функция func providerSource
8c928e83589d90a031f811fae52a81be7153e82f

	git log -S'func providerSource' --oneline
	git log -1 8c928e835


## 6. Все коммиты в которых была изменена функция globalPluginDirs


78b122055 Remove config.go and update things using its aliases

52dbf9483 keep .terraform.d/plugins for discovery

41ab0aef7 Add missing OS_ARCH dir to global plugin paths

66ebff90c move some more plugin search path logic to command

8364383c3 Push plugin discovery down into command package

	git log -L :globalPluginDirs:plugins.go

## 7. Автор функции synchronizedWriters
Author: Martin Atkins <mart@degeneration.co.uk>

	git log -S'func synchronizedWriters' --oneline
	git show 5ac311e2a







