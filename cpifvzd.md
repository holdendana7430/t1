代发 wailian999

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://oh.yuexingan06.cn

================================================================================
来源：http://hu.wgjwhj.cn

B. 流程控制
来源：http://dr.yuntaijiaju.cn

================================================================================
来源：http://ob.shxzskj.cn

[B01] 条件判断 if / else
来源：http://zb.shxzukj.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://gc.shtwfgs.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://kj.wgjwhj.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://mk.bookmarksfly.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://kr.huixiangedu.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://lv.9csxet.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://jn.huixiangedu.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://by.wgjwhj.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://fd.szxytkj.cn

[B02] 多分支 else if / elif
来源：http://vi.hnjuh.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ze.colortex.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://oo.muxihuayi.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yf.jianghongdianzi.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dz.bjjhwx.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lm.shxzskj.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ek.colortex.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://bt.haigaiapp.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ou.newstarts.cn

[B03] switch / match / case
来源：http://or.yuexingan06.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ca.521024.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://kd.szxytkj.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://le.shtwfgs.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ch.huixiangedu.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hr.gzmigu.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://qh.521024.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://wb.asd995.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://qs.colortex.cn

[B04] for 计数循环
来源：http://qn.huanxung.cn

Py:   for i in range(10): print(i)
来源：http://jz.szxytkj.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://gs.jianghongdianzi.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://sl.nicolike.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ge.nicolike.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://cy.panjiajie.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://uq.panjiajie.cn

Ruby: 10.times { |i| puts i }
来源：http://xw.hahajie.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://qj.gzmigu.cn

[B05] 遍历数组 / 列表
来源：http://xy.hahajie.cn

Py:   for item in arr: print(item)
来源：http://kf.jctech888.com.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://cf.bjjhwx.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://vy.asd995.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://xv.huanxung.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://sd.huixinmuqiang.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://lr.bjjhwx.cn

Ruby: arr.each { |item| puts item }
来源：http://py.shxzukj.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://it.gzmigu.cn

[B06] 遍历字典 / 对象
来源：http://ih.szxytkj.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://er.9csxet.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hl.colortex.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://dg.shxzukj.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mw.haigaiapp.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://dy.muxihuayi.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://qy.szsharing.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://jn.huanxung.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://so.szxytkj.cn

[B07] while 循环
来源：http://ib.colortex.cn

Py:   while i < 10: i += 1
来源：http://mc.szxytkj.cn

PHP:  while ($i < 10) { $i++; }
来源：http://vl.9csxet.cn

JS:   while (i < 10) { i++; }
来源：http://ca.szxytkj.cn

TS:   while (i < 10) { i++; }
来源：http://nx.shxzskj.cn

Java: while (i < 10) { i++; }
来源：http://sm.szsharing.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ny.szsharing.cn

Ruby: while i < 10; i += 1; end
来源：http://jm.huixiangedu.cn

C#:   while (i < 10) { i++; }
来源：http://fl.bjjhwx.cn

[B08] do-while（至少执行一次）
来源：http://ig.bookmarksfly.cn

Py:   # 无 do-while：用 while True + break
来源：http://gx.shtwfgs.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ky.shxzukj.cn

JS:   do { i++; } while (i < 10);
来源：http://mx.wgjwhj.cn

TS:   do { i++; } while (i < 10);
来源：http://lk.hnjuh.cn

Java: do { i++; } while (i < 10);
来源：http://bn.huanxung.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://de.lnxyls.cn

Ruby: begin; i += 1; end while i < 10
来源：http://et.jianghongdianzi.cn

C#:   do { i++; } while (i < 10);
来源：http://gt.wgjwhj.cn

[B09] break 与 continue
来源：http://pz.yuntaijiaju.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://tx.shxzukj.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://er.panjiajie.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qr.hnjuh.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fy.huixiangedu.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yp.jianghongdianzi.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ey.shtwfgs.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://xy.nszjky.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vx.gzmigu.cn

[B10] 遍历同时拿索引
来源：http://nk.szxytkj.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://va.bjjhwx.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://zm.shxzskj.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ze.huixiangedu.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://yd.szxytkj.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wx.bookmarksfly.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ri.yuntaijiaju.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://pm.yuexingan06.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://qg.muxihuayi.cn

[B11] 生成数字序列 / 区间
来源：http://xd.szxytkj.cn

Py:   list(range(0, 10, 2))
来源：http://dt.muxihuayi.cn

PHP:  range(0, 10, 2);
来源：http://gf.lnxyls.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://cg.hnjuh.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://su.shtwfgs.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://sk.newstarts.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://dg.shxzukj.cn

Ruby: (0...10).step(2).to_a
来源：http://rq.haigaiapp.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://vp.shxzskj.cn

[B12] 跳出多层循环
来源：http://bv.huixiangedu.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://dk.colortex.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://gj.shtwfgs.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://fk.bookmarksfly.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://oj.hnjuh.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://yg.yuntaijiaju.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ck.huixiangedu.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ju.wgjwhj.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://gr.chemitech.net.cn

[B13] 判断是否为数字
来源：http://km.huanxung.cn

Py:   isinstance(x, (int, float))
来源：http://en.bjjhwx.cn

PHP:  is_numeric($x)
来源：http://li.szxytkj.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xi.szxytkj.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ek.nicolike.cn

Java: x instanceof Number
来源：http://lb.huixinmuqiang.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://iu.haigaiapp.cn

Ruby: x.is_a?(Numeric)
来源：http://zx.hnjuh.cn

C#:   x is int or double or decimal
来源：http://mr.lnxyls.cn

[B14] 判断值是否在集合内
来源：http://gf.panjiajie.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://gw.wgjwhj.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://rm.huixiangedu.cn

JS:   [1, 2, 3].includes(x)
来源：http://ob.hnjuh.cn

TS:   [1, 2, 3].includes(x)
来源：http://kf.szxytkj.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ev.newstarts.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://pb.hahajie.cn

Ruby: [1, 2, 3].include?(x)
来源：http://oe.shxzskj.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ge.yuntaijiaju.cn

[B15] 布尔运算与取反
来源：http://ui.asd995.cn

Py:   a and b or not c
来源：http://ek.hahajie.cn

PHP:  $a && $b || !$c
来源：http://hl.521024.cn

JS:   a && b || !c
来源：http://ld.jianghongdianzi.cn

TS:   a && b || !c
来源：http://wp.hnjuh.cn

Java: a && b || !c
来源：http://eu.shxzukj.cn

Go:   a && b || !c
来源：http://bp.bjjhwx.cn

Ruby: a && b || !c
来源：http://eb.lnxyls.cn

C#:   a && b || !c
来源：http://vk.nicolike.cn

[B16] 卫语句：不满足条件提前返回
来源：http://gf.haigaiapp.cn

Py:   if not data: return
来源：http://dp.shxzukj.cn

PHP:  if (!$data) { return; }
来源：http://lx.hahajie.cn

JS:   if (!data) return;
来源：http://xc.muxihuayi.cn

TS:   if (!data) return;
来源：http://yb.shxzskj.cn

Java: if (data == null) return;
来源：http://qp.shxzukj.cn

Go:   if data == nil { return }
来源：http://py.jctech888.com.cn

Ruby: return if data.nil?
来源：http://de.521024.cn

C#:   if (data == null) return;
来源：http://uh.huanxung.cn

================================================================================
来源：http://oo.jctech888.com.cn

C. 函数与作用域
来源：http://fg.shtwfgs.cn

================================================================================
来源：http://tf.nicolike.cn

[C01] 定义函数
来源：http://ru.szxytkj.cn

Py:   def add(a, b): return a + b
来源：http://ai.nszjky.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://cb.hahajie.cn

JS:   function add(a, b) { return a + b; }
来源：http://qr.bookmarksfly.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xc.bjjhwx.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://kh.jianghongdianzi.cn

Go:   func add(a, b int) int { return a + b }
来源：http://zs.nszjky.cn

Ruby: def add(a, b); a + b; end
来源：http://jw.bjjhwx.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://yw.wgjwhj.cn

[C02] 默认参数
来源：http://sx.szsharing.cn

Py:   def greet(name="World"): return name
来源：http://jg.bookmarksfly.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://yl.521024.cn

JS:   function greet(name = "World") { return name; }
来源：http://ga.jianghongdianzi.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://tb.huixiangedu.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://af.nszjky.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wu.yuexingan06.cn

Ruby: def greet(name = "World") = name
来源：http://wo.huixinmuqiang.cn

C#:   string Greet(string name = "World") => name;
来源：http://pm.chemitech.net.cn

[C03] 可变参数
来源：http://bx.shxzukj.cn

Py:   def total(*args): return sum(args)
来源：http://er.hnjuh.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ep.huixiangedu.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://pe.yuntaijiaju.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://jm.wgjwhj.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://gf.521024.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ld.hahajie.cn

Ruby: def total(*nums); nums.sum; end
来源：http://hh.huixiangedu.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://vx.bookmarksfly.cn

[C04] 命名参数 / 关键字参数
来源：http://vj.lnxyls.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hn.newstarts.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://gc.9csxet.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://jz.nszjky.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ql.newstarts.cn

Java: // 无：用 Builder 模式或 record
来源：http://vo.huanxung.cn

Go:   // 无：用配置结构体参数
来源：http://hp.bjjhwx.cn

Ruby: f(a: 1, b: 2)
来源：http://kv.yuexingan06.cn

C#:   f(a: 1, b: 2)
来源：http://za.asd995.cn

[C05] 返回多个值
来源：http://tw.colortex.cn

Py:   return a, b
来源：http://ox.huixiangedu.cn

PHP:  return [$a, $b];
来源：http://xa.chemitech.net.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://mn.haigaiapp.cn

TS:   return { a, b };
来源：http://ih.bjjhwx.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://sz.huanxung.cn

Go:   return a, b
来源：http://ub.muxihuayi.cn

Ruby: return a, b
来源：http://lr.shtwfgs.cn

C#:   return (a, b);              // ValueTuple
来源：http://oh.lnxyls.cn

[C06] 匿名函数 / lambda
来源：http://ho.nszjky.cn

Py:   square = lambda x: x * x
来源：http://wq.szxytkj.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://yi.hahajie.cn

JS:   const square = x => x * x;
来源：http://ca.nicolike.cn

TS:   const square = (x: number): number => x * x;
来源：http://cl.colortex.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://lq.muxihuayi.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ek.shxzskj.cn

Ruby: square = ->(x) { x * x }
来源：http://of.shxzskj.cn

C#:   Func<int, int> square = x => x * x;
来源：http://yc.hahajie.cn

[C07] 把函数作为参数传入
来源：http://xx.asd995.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://rz.jianghongdianzi.cn

PHP:  array_map("strtoupper", $arr);
来源：http://hy.9csxet.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ys.jctech888.com.cn

TS:   arr.map(String)
来源：http://pt.9csxet.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://qn.nszjky.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://tw.hahajie.cn

Ruby: arr.map(&:upcase)
来源：http://yc.muxihuayi.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://sp.shxzskj.cn

[C08] 闭包
来源：http://zn.panjiajie.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ej.521024.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mv.521024.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://aq.szxytkj.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://gj.szxytkj.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://cs.bjjhwx.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://fv.jianghongdianzi.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://le.bookmarksfly.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://po.muxihuayi.cn

[C09] 递归
来源：http://tq.yuexingan06.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wp.muxihuayi.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://fq.chemitech.net.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vm.lnxyls.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://cs.wgjwhj.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ml.bjjhwx.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://dq.shxzukj.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ry.9csxet.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mb.panjiajie.cn

[C10] 变量作用域
来源：http://fy.szxytkj.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ll.lnxyls.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hx.bjjhwx.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://cf.shtwfgs.cn

TS:   同 JS
来源：http://zt.haigaiapp.cn

Java: 方法内为块级作用域
来源：http://ba.colortex.cn

Go:   花括号块级作用域
来源：http://kf.shxzukj.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://aa.huixiangedu.cn

C#:   块级作用域
来源：http://em.gzmigu.cn

[C11] 模块导入与导出
来源：http://mv.gzmigu.cn

Py:   from module import func
来源：http://yt.szsharing.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://zs.jctech888.com.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://we.nszjky.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://li.jctech888.com.cn

Java: import java.util.List;
来源：http://pp.bookmarksfly.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mn.shtwfgs.cn

Ruby: require "json"; require_relative "./util"
来源：http://ad.nszjky.cn

C#:   using System.Text;
来源：http://xh.huixiangedu.cn

[C12] 立即执行函数 IIFE
来源：http://rt.shxzskj.cn

Py:   (lambda: print("run"))()
来源：http://gt.gzmigu.cn

PHP:  (function () { echo "run"; })();
来源：http://az.hnjuh.cn

JS:   (() => { console.log("run"); })();
来源：http://ft.huixiangedu.cn

TS:   (() => { console.log("run"); })();
来源：http://hx.haigaiapp.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://xc.wgjwhj.cn

Go:   func() { fmt.Println("run") }()
来源：http://dq.shtwfgs.cn

Ruby: -> { puts "run" }.call
来源：http://by.hahajie.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://tu.hahajie.cn

[C13] 类型声明 / 类型注解
来源：http://xr.huixinmuqiang.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://qy.shxzukj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://sn.yuexingan06.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://kh.hahajie.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mn.yuntaijiaju.cn

Java: int add(int a, int b) { return a + b; }
来源：http://zc.yuexingan06.cn

Go:   func add(a, b int) int
来源：http://nq.haigaiapp.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://tm.shtwfgs.cn

C#:   int Add(int a, int b) => a + b;
来源：http://bj.chemitech.net.cn

[C14] 泛型函数
来源：http://nx.shtwfgs.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ie.huixiangedu.cn

PHP:  // 无泛型
来源：http://qc.szsharing.cn

JS:   // 无泛型
来源：http://wt.muxihuayi.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://km.chemitech.net.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ta.huixinmuqiang.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://yy.szxytkj.cn

Ruby: # 无泛型
来源：http://ui.hahajie.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://sw.haigaiapp.cn

[C15] 解构 / 展开参数
来源：http://go.shxzukj.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://du.yuntaijiaju.cn

PHP:  [$a, $b] = $pair;
来源：http://pl.szxytkj.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://tm.wgjwhj.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://rg.yuexingan06.cn

Java: // 无解构
来源：http://gd.bookmarksfly.cn

Go:   // 无解构
来源：http://uw.yuexingan06.cn

Ruby: a, b = pair
来源：http://dr.panjiajie.cn

C#:   var (a, b) = pair;
来源：http://jw.yuntaijiaju.cn

[C16] 函数 / 方法重载
来源：http://lm.9csxet.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ow.shxzskj.cn

PHP:  // 无重载
来源：http://au.yuntaijiaju.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://oo.shxzukj.cn

TS:   // 用联合类型或重载签名声明
来源：http://hh.521024.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://rn.521024.cn

Go:   // 无重载：用不同函数名
来源：http://eu.huanxung.cn

Ruby: # 无重载：靠动态参数
来源：http://ec.shxzskj.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://dx.gzmigu.cn

================================================================================
来源：http://fi.jctech888.com.cn

D. 数组 / 列表 / 集合
来源：http://ds.bookmarksfly.cn

================================================================================
来源：http://jt.hnjuh.cn

[D01] 创建数组 / 列表
来源：http://tq.huixiangedu.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://kj.yuntaijiaju.cn


<!-- 参考信息 -->