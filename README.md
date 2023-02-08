# acvtool-py3
Android Applications code coverage tools actool(https://github.com/pilgun/acvtool) python3 rebuild

Not completed, currently reporting an error during the report generation phase


``` bash
Traceback (most recent call last):
  File "acvtool.py", line 220, in <module>
    main()
  File "acvtool.py", line 217, in main
    run_actions(parser, args)
  File "acvtool.py", line 82, in run_actions
    reporter.generate(
  File "/home/syc/Documents/acvtool-py3/smiler/reporter.py", line 37, in generate
    save_html_report(report_dir, smalitree, package, granularity)
  File "/home/syc/Documents/acvtool-py3/smiler/reporter.py", line 82, in save_html_report
    save_coverage(smalitree, templates, output_dir, app_name, granularity)
  File "/home/syc/Documents/acvtool-py3/smiler/reporter.py", line 94, in save_coverage
    (package, path, coverage_data) = save_package_indexhtml(g, templates, output_dir, app_name, granularity)
  File "/home/syc/Documents/acvtool-py3/smiler/reporter.py", line 153, in save_package_indexhtml
    row = init_row(elementlink=elementlink, type='class', elementname=elementname,
  File "/usr/local/lib/python3.8/dist-packages/chameleon/template.py", line 124, in __call__
    return self.render(**kwargs)
  File "/usr/local/lib/python3.8/dist-packages/chameleon/zpt/template.py", line 289, in render
    return super(PageTemplate, self).render(**_kw)
  File "/usr/local/lib/python3.8/dist-packages/chameleon/template.py", line 168, in render
    self.cook_check()
  File "/usr/local/lib/python3.8/dist-packages/chameleon/template.py", line 299, in cook_check
    self.cook(body)
  File "/usr/local/lib/python3.8/dist-packages/chameleon/template.py", line 146, in cook
    program = self._cook(body, digest, names)
  File "/usr/local/lib/python3.8/dist-packages/chameleon/template.py", line 219, in _cook
    source = self._make(body, builtins)
  File "/usr/local/lib/python3.8/dist-packages/chameleon/template.py", line 257, in _make
    return self._compile(module, builtins)
  File "/usr/local/lib/python3.8/dist-packages/chameleon/template.py", line 251, in _compile
    compiler = Compiler(self.engine, program, builtins, strict=self.strict)
  File "/usr/local/lib/python3.8/dist-packages/chameleon/compiler.py", line 947, in __init__
    generator = TemplateCodeGenerator(module)
  File "/usr/local/lib/python3.8/dist-packages/chameleon/codegen.py", line 130, in __init__
    super(TemplateCodeGenerator, self).__init__(tree)
  File "/usr/local/lib/python3.8/dist-packages/chameleon/astutil.py", line 220, in __init__
    self.visit(tree)
  File "/usr/local/lib/python3.8/dist-packages/chameleon/codegen.py", line 215, in visit
    super(TemplateCodeGenerator, self).visit(node)
  File "/usr/local/lib/python3.8/dist-packages/chameleon/astutil.py", line 280, in visit
    ret = visitor(node)
  File "/usr/local/lib/python3.8/dist-packages/chameleon/codegen.py", line 133, in visit_Module
    super(TemplateCodeGenerator, self).visit_Module(node)
  File "/usr/local/lib/python3.8/dist-packages/chameleon/astutil.py", line 287, in visit_Module
    self.visit(n)
  File "/usr/local/lib/python3.8/dist-packages/chameleon/codegen.py", line 215, in visit
    super(TemplateCodeGenerator, self).visit(node)
  File "/usr/local/lib/python3.8/dist-packages/chameleon/astutil.py", line 280, in visit
    ret = visitor(node)
  File "/usr/local/lib/python3.8/dist-packages/chameleon/astutil.py", line 381, in visit_Assign
    self.visit(node.value)
  File "/usr/local/lib/python3.8/dist-packages/chameleon/codegen.py", line 215, in visit
    super(TemplateCodeGenerator, self).visit(node)
  File "/usr/local/lib/python3.8/dist-packages/chameleon/astutil.py", line 280, in visit
    ret = visitor(node)
  File "/usr/local/lib/python3.8/dist-packages/chameleon/astutil.py", line 823, in visit_Call
    self.visit(arg)
  File "/usr/local/lib/python3.8/dist-packages/chameleon/codegen.py", line 215, in visit
    super(TemplateCodeGenerator, self).visit(node)
  File "/usr/local/lib/python3.8/dist-packages/chameleon/astutil.py", line 278, in visit
    raise Exception('No handler for ``%s`` (%s).' % (
Exception: No handler for ``Constant`` (<_ast.Constant object at 0x7f784143fa60>).

```