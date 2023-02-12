1. как получено: git show aefea
   aefead2207ef7e2aa5dc81a34aedf0cad4c32545; комментарий: Update CHANGELOG.md


2. как получено: git show 85024d3
   tag: v0.12.23


3. как получено: 1. git show b8d720^ и  git show b8d720^2
	          2. git show -s --format=%p b8d720
2 родителя: 56cd7859e05c36c06b56d013b55a252d0bb7e158; 9ea88f22fc6269854151c571162c5bcf958bee2b


4. как получено: $ git log v0.12.23..v0.12.24
    commit 33ff1c03bb960b332be3af2e333462dde88b279e (tag: v0.12.24)
    v0.12.24

    commit b14b74c4939dcab573326f4e3ee2a62e23e12f89
    [Website] vmc provider links

    commit 3f235065b9347a758efadc92295b540ee0a5e26e
    Update CHANGELOG.md

    commit 6ae64e247b332925b872447e9ce869657281c2bf
    registry: Fix panic when server is unreachable

    Non-HTTP errors previously resulted in a panic due to dereferencing the
    resp pointer while it was nil, as part of rendering the error message.
    This commit changes the error message formatting to cope with a nil
    response, and extends test coverage.

    Fixes #24384

    commit 5c619ca1baf2e21a155fcdb4c264cc9e24a2a353
    website: Remove links to the getting started guide's old location

    Since these links were in the soon-to-be-deprecated 0.11 language section, I
    think we can just remove them without needing to find an equivalent link.

   commit 06275647e2b53d97d4f0a19a0fec11f6d69820b5
    Update CHANGELOG.md

   commit d5f9411f5108260320064349b757f55c09bc4b80
    command: Fix bug when using terraform login on Windows

5. как получено:  $ git log -S'func providerSource'
    8c928e83589d90a031f811fae52a81be7153e82f

6. как получено:  $ git grep --heading -n -i 'globalPluginDirs'
                             $ git log --oneline -L :globalPluginDirs:plugins.go
    список коммитов:
    78b1220558; 52dbf94834; 41ab0aef7a; 66ebff90cd; 8364383c35

7. как получено: $ git log -SsynchronizedWriters
    Author: Martin Atkins <mart@degeneration.co.uk>
  


	
