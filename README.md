# CodeMirror 6 Cairo language pack

### WIP

> Initial strategy is to use keywords from [keywords.adoc in starkware-libs/cairo](https://github.com/starkware-libs/cairo/blob/main/docs/reference/src/keywords.adoc). Pointers, suggestions and ideas very welcome!

This is an example repository containing a minimal [CodeMirror](https://codemirror.net/6/) language support package. The idea is to clone it, rename it, and edit it to create support for a new language.

Things you'll need to do (see the [language support example](https://codemirror.net/6/examples/lang-package/) for a more detailed tutorial):
- [ ] `git grep EXAMPLE` and replace all instances with your language name.
- [ ] Rewrite the grammar in `src/syntax.grammar` to cover your language. See the [Lezer system guide](https://lezer.codemirror.net/docs/guide/#writing-a-grammar) for information on this file format.
  - [ ] Start with keyword tokens for v0.1
- [ ] Adjust the metadata in `src/index.ts` to work with your new grammar.
- [ ] Rewrite this readme file.
- [ ] Optionally add a license.
- [ ] Adjust the grammar tests in `test/cases.txt`.
- [ ] Build (`npm run prepare`) and test (`npm test`).
- [ ] Publish. Put your package on npm under a name like `codemirror-lang-EXAMPLE`.
