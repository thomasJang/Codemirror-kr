# 프로젝트 참여방법

- [Getting help](#getting-help-)
- [Submitting bug reports](#submitting-bug-reports-)
- [Contributing code](#contributing-code-)

## 도움말
  
Community discussion, questions, and informal bug reporting is done on the
[discuss.CodeMirror forum](http://discuss.codemirror.net).
> 토론, 질문, 비공식 버그리포팅은 다음의 URL에서 확인 할 수 있습니다. [discuss.CodeMirror forum](http://discuss.codemirror.net).

## 버그리포트 작성하기

The preferred way to report bugs is to use the
[GitHub issue tracker](http://github.com/codemirror/CodeMirror/issues). Before
reporting a bug, read these pointers.
> 우리가 좋아하는 버그 리포트를 작성하는 방법은 GitHub 이슈를 남기는 것 입니다. [GitHub issue tracker](http://github.com/codemirror/CodeMirror/issues). 버그리포트를 작성하기 전에 다음의 몇가지 사항을 확인해주십시요 

**Note:** The issue tracker is for *bugs*, not requests for help. Questions
should be asked on the
[discuss.CodeMirror forum](http://discuss.codemirror.net) instead.
> **주의:** Github 이슈는 버그를 남기는 공간입니다. 도움을 요청하는 공간이 아닙니다. 질문은 다음의 토론게시판을 이용하세요 [discuss.CodeMirror forum](http://discuss.codemirror.net)  

### 버그리포트 작성가이드

- CodeMirror is maintained by volunteers. They don't owe you anything, so be
  polite. Reports with an indignant or belligerent tone tend to be moved to the
  bottom of the pile.
> CodeMirror는 자원봉사자로 운영됩니다. 자원봉사자들은 당신에게 서비스하는 사람이 아닙니다. 그러므로 공손해야 합니다. 화난말투나 시비거는 말투를 사용하면 당신의 버그리포트는 무시될 수 있습니다.
``` 
tend to (~하는 경향이 있다)
```

- Include information about **the browser in which the problem occurred**. Even
  if (you tested several browsers, and the problem occurred in all of them,)
  mention this fact in the bug report. Also include browser version numbers and
  the operating system that you're on.
> 버그가 발생한 브라우저 정보를 포함해주세요, 여러가지 브라우저에서 모두 모두 버그가 발생하더라도 버그가 발생한 모든 브라우저 정보를 포함해주세요. OS나 브라우저 버전정보까지 포함 된다면 금상첨화겠지요
```
Even if (만약 ~하더라도)
operating system that you're on. (당신이 쓰고 있는 브라우저)
```

- Mention which release of CodeMirror you're using. Preferably, try also with
  the current development snapshot, to ensure the problem has not already been
  fixed.
> 당신이 사용중인 CodeMirror버전을 남겨주세요. 아직 고쳐지지 않은 문제라는 것을 입증하기 위해 가능하다면 최신버전 이용을 권장합니다.
```
has not already been fixed (아직 고쳐지지 않은)
수동태 be + PP
```

- Mention very precisely what went wrong. "X is broken" is not a good bug
  report. What did you expect to happen? What happened instead? Describe the exact steps A maintainer has to take
  to make the problem occur. We can not fix something( that we can not observe. )
> "X가 안된다" 식의 버그 리포트는 좋지 않습니다. 어떤 기능을 의도하였는지 어떤 결과가 발생하였는지 운영자가 문제를 재현할 수 있도록 정확한 절차를 설명해야 합니다. 당신이 수행한 절차를 설명하지 않으면 우리는 그 문제를 해결할 수 없습니다.  


- If the problem can not be reproduced in any of the demos included in the
  CodeMirror distribution, please provide an HTML document that demonstrates
  the problem. The best way to do this is to go to
  [jsbin.com](http://jsbin.com/ihunin/edit), enter it there, press save, and
  include the resulting link in your bug report.
> 만약 문제가 Codemirror에서 만들어진 데모로는 재현되지 않을 때는 문제를 재현할 수 있는 HTML 문서를 만들어 주시면 감사하겠습니다. HTML 문서를 만들수 있는 좋은 방법중에 하나로 [jsbin.com](http://jsbin.com/ihunin/edit)를 추천합니다. 
```
to 부정사 (~ 하기)
```

## 코드에 기여하기

- Make sure you have a [GitHub Account](https://github.com/signup/free)
> 깃허브에서 계정을 만들어주세요
```
Make sure ~ (~를 확실하게 해라, ~ 확인해라)
```

- Fork [CodeMirror](https://github.com/codemirror/CodeMirror/)
  ([how to fork a repo](https://help.github.com/articles/fork-a-repo))
> Codemirror를 포크해주세요

- Make your changes
> 코드를 변경하세요

- If your changes are easy to test or likely to regress, add tests.
  Tests for the core go into `test/test.js`, some modes have their own
  test suite under `mode/XXX/test.js`. Feel free to add new test
  suites to modes that don't have one yet be sure to link the new
  tests into `test/index.html`.
> 만약 당신의 코드변경내용이 테스트하기 쉽고, 원복하기 수월하면 테스트를 추가하세요 테스트코드를 'test/test.js'안에 넣어라, 모드 테스트는 각각의 모드 폴더 아래 `mode/XXX/test.js`에 테스트 코드가 있습니다. 새로운 모드는 자유롭게 추가하고 `test/index.html`에 링크를 추가해주세요 
```
Feel free to (자유롭게 ~ 해라)
```

- Follow the general code style of the rest of the project see
  below. Run `bin/lint` to verify that the linter is happy.
> 기존 프로젝트에 있는 코드의 스타일을 최대한 따라주세요. `bin/lint`의 linter로 코드를 검사하면 아주 좋습니다. 

- Make sure all tests pass. Visit `test/index.html` in your browser to
  run them.
> 코드 검사가 완료되면 당신의 브라우저에 실행시켜주세요.

- Submit a pull request
([how to create a pull request](https://help.github.com/articles/fork-a-repo)).
  Don't put more than one feature/fix in a single pull request.
> 풀 리퀘스트 상용법은 ([how to create a pull request](https://help.github.com/articles/fork-a-repo))에 있습니다. 한번에 한개의 수정사항만 풀리퀘스트 해주세요. 

By contributing code to CodeMirror you

 - agree to license the contributed code under CodeMirror's [MIT
   license](http://codemirror.net/LICENSE).

 - confirm that you have the right to contribute and license the code
   in question. (Either you hold all rights on the code, or the rights
   holder has explicitly granted the right to use it like this,
   through a compatible open source license or through a direct
   agreement with you.)
   
   > question

### Coding standards

- 2 spaces per indentation level, no tabs.
- Include semicolons after statements.
- Note that the linter (`bin/lint`) which is run after each commit
  complains about unused variables and functions. Prefix their names
  with an underscore to muffle it.

- CodeMirror does *not* follow JSHint or JSLint prescribed style.
  Patches that try to 'fix' code to pass one of these linters will be
  unceremoniously discarded.
