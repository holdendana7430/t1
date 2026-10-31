代发 wailian999

[B01] 条件判断 if / else
来源：http://ae.yuexingan06.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://aa.shxzskj.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://zg.szxytkj.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ay.newstarts.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://jt.yuntaijiaju.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ii.yuntaijiaju.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://de.521024.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://fk.shtwfgs.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ct.nszjky.cn

[B02] 多分支 else if / elif
来源：http://nb.9csxet.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://fh.newstarts.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hy.szsharing.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ht.muxihuayi.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pn.shxzukj.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gg.bjjhwx.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://dl.jctech888.com.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://st.huixiangedu.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mw.colortex.cn

[B03] switch / match / case
来源：http://gv.gzmigu.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ya.asd995.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://jk.jctech888.com.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://jg.hahajie.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://yi.hahajie.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://pn.gzmigu.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ar.szsharing.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://jk.nszjky.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://dx.jctech888.com.cn

[B04] for 计数循环
来源：http://eq.huixinmuqiang.cn

Py:   for i in range(10): print(i)
来源：http://pf.9csxet.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://tj.newstarts.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://yu.wgjwhj.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://jq.shxzukj.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ir.gzmigu.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://af.jctech888.com.cn

Ruby: 10.times { |i| puts i }
来源：http://cu.panjiajie.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://tv.hahajie.cn

[B05] 遍历数组 / 列表
来源：http://kl.jianghongdianzi.cn

Py:   for item in arr: print(item)
来源：http://ho.wgjwhj.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://zj.nicolike.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://zg.muxihuayi.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://rw.yuexingan06.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://lj.huixiangedu.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://on.chemitech.net.cn

Ruby: arr.each { |item| puts item }
来源：http://nd.nszjky.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://zv.bjjhwx.cn

[B06] 遍历字典 / 对象
来源：http://gk.colortex.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://gv.yuntaijiaju.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://vu.nszjky.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://tt.521024.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ej.9csxet.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ev.nicolike.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ki.szsharing.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://sr.shxzukj.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://xc.huixinmuqiang.cn

[B07] while 循环
来源：http://se.huixinmuqiang.cn

Py:   while i < 10: i += 1
来源：http://zv.lnxyls.cn

PHP:  while ($i < 10) { $i++; }
来源：http://qf.szxytkj.cn

JS:   while (i < 10) { i++; }
来源：http://ll.nszjky.cn

TS:   while (i < 10) { i++; }
来源：http://dc.shxzskj.cn

Java: while (i < 10) { i++; }
来源：http://jk.chemitech.net.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ia.huixinmuqiang.cn

Ruby: while i < 10; i += 1; end
来源：http://mt.wgjwhj.cn

C#:   while (i < 10) { i++; }
来源：http://ew.shxzukj.cn

[B08] do-while（至少执行一次）
来源：http://ew.shxzskj.cn

Py:   # 无 do-while：用 while True + break
来源：http://he.gzmigu.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ll.gzmigu.cn

JS:   do { i++; } while (i < 10);
来源：http://qk.asd995.cn

TS:   do { i++; } while (i < 10);
来源：http://vx.wgjwhj.cn

Java: do { i++; } while (i < 10);
来源：http://uh.bjjhwx.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://zl.chemitech.net.cn

Ruby: begin; i += 1; end while i < 10
来源：http://kp.szxytkj.cn

C#:   do { i++; } while (i < 10);
来源：http://sb.gzmigu.cn

[B09] break 与 continue
来源：http://ps.colortex.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://se.colortex.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://pj.nicolike.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ts.huixinmuqiang.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hc.hahajie.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nt.hnjuh.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ll.jctech888.com.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://uy.szsharing.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dv.nicolike.cn

[B10] 遍历同时拿索引
来源：http://fi.521024.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ld.jctech888.com.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://dq.9csxet.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://gz.jctech888.com.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ya.haigaiapp.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://bi.nszjky.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://om.lnxyls.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://pt.hahajie.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://co.nicolike.cn

[B11] 生成数字序列 / 区间
来源：http://sn.haigaiapp.cn

Py:   list(range(0, 10, 2))
来源：http://wl.colortex.cn

PHP:  range(0, 10, 2);
来源：http://kp.nszjky.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://gn.colortex.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wk.nszjky.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ut.nszjky.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://nh.muxihuayi.cn

Ruby: (0...10).step(2).to_a
来源：http://lr.huixiangedu.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://zk.bjjhwx.cn

[B12] 跳出多层循环
来源：http://va.panjiajie.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://yi.bookmarksfly.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://kl.shxzskj.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://bm.panjiajie.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://vt.yuntaijiaju.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://iy.jctech888.com.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mz.hnjuh.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://km.muxihuayi.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ek.asd995.cn

[B13] 判断是否为数字
来源：http://pz.panjiajie.cn

Py:   isinstance(x, (int, float))
来源：http://xz.lnxyls.cn

PHP:  is_numeric($x)
来源：http://yy.hahajie.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ql.panjiajie.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wf.9csxet.cn

Java: x instanceof Number
来源：http://jl.szsharing.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://cw.haigaiapp.cn

Ruby: x.is_a?(Numeric)
来源：http://qb.jianghongdianzi.cn

C#:   x is int or double or decimal
来源：http://ol.bookmarksfly.cn

[B14] 判断值是否在集合内
来源：http://ta.nicolike.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://pl.9csxet.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://vl.colortex.cn

JS:   [1, 2, 3].includes(x)
来源：http://qf.nszjky.cn

TS:   [1, 2, 3].includes(x)
来源：http://ri.yuntaijiaju.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://le.wgjwhj.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hx.shxzskj.cn

Ruby: [1, 2, 3].include?(x)
来源：http://sq.szxytkj.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ms.huanxung.cn

[B15] 布尔运算与取反
来源：http://xf.bjjhwx.cn

Py:   a and b or not c
来源：http://mq.huixiangedu.cn

PHP:  $a && $b || !$c
来源：http://iz.huixiangedu.cn

JS:   a && b || !c
来源：http://rn.yuntaijiaju.cn

TS:   a && b || !c
来源：http://az.huanxung.cn

Java: a && b || !c
来源：http://pi.shxzukj.cn

Go:   a && b || !c
来源：http://ct.yuexingan06.cn

Ruby: a && b || !c
来源：http://kb.yuexingan06.cn

C#:   a && b || !c
来源：http://rn.huixiangedu.cn

[B16] 卫语句：不满足条件提前返回
来源：http://xc.nszjky.cn

Py:   if not data: return
来源：http://qd.muxihuayi.cn

PHP:  if (!$data) { return; }
来源：http://rj.colortex.cn

JS:   if (!data) return;
来源：http://si.9csxet.cn

TS:   if (!data) return;
来源：http://di.muxihuayi.cn

Java: if (data == null) return;
来源：http://hi.521024.cn

Go:   if data == nil { return }
来源：http://yp.9csxet.cn

Ruby: return if data.nil?
来源：http://vt.hnjuh.cn

C#:   if (data == null) return;
来源：http://ut.shxzukj.cn

================================================================================
来源：http://tt.shtwfgs.cn

C. 函数与作用域
来源：http://cu.gzmigu.cn

================================================================================
来源：http://ba.wgjwhj.cn

[C01] 定义函数
来源：http://lk.hahajie.cn

Py:   def add(a, b): return a + b
来源：http://fu.chemitech.net.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://gf.panjiajie.cn

JS:   function add(a, b) { return a + b; }
来源：http://ez.muxihuayi.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://vp.bjjhwx.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://tp.521024.cn

Go:   func add(a, b int) int { return a + b }
来源：http://zq.huixinmuqiang.cn

Ruby: def add(a, b); a + b; end
来源：http://er.shxzukj.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ho.wgjwhj.cn

[C02] 默认参数
来源：http://pa.nszjky.cn

Py:   def greet(name="World"): return name
来源：http://dx.9csxet.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://ns.szxytkj.cn

JS:   function greet(name = "World") { return name; }
来源：http://mv.asd995.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://cu.lnxyls.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://df.jianghongdianzi.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://de.hnjuh.cn

Ruby: def greet(name = "World") = name
来源：http://ii.nicolike.cn

C#:   string Greet(string name = "World") => name;
来源：http://hu.wgjwhj.cn

[C03] 可变参数
来源：http://do.panjiajie.cn

Py:   def total(*args): return sum(args)
来源：http://ng.szsharing.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ik.521024.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://sc.panjiajie.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://so.lnxyls.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://cb.huanxung.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ye.bjjhwx.cn

Ruby: def total(*nums); nums.sum; end
来源：http://oa.yuntaijiaju.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://vd.lnxyls.cn

[C04] 命名参数 / 关键字参数
来源：http://sz.shxzukj.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://pv.panjiajie.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://rd.szxytkj.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wz.haigaiapp.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://cy.hnjuh.cn

Java: // 无：用 Builder 模式或 record
来源：http://qh.muxihuayi.cn

Go:   // 无：用配置结构体参数
来源：http://kh.nicolike.cn

Ruby: f(a: 1, b: 2)
来源：http://rs.shxzukj.cn

C#:   f(a: 1, b: 2)
来源：http://lt.colortex.cn

[C05] 返回多个值
来源：http://qj.yuexingan06.cn

Py:   return a, b
来源：http://ts.bookmarksfly.cn

PHP:  return [$a, $b];
来源：http://nk.nszjky.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://gp.muxihuayi.cn

TS:   return { a, b };
来源：http://vh.bjjhwx.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://vu.asd995.cn

Go:   return a, b
来源：http://kf.szxytkj.cn

Ruby: return a, b
来源：http://au.muxihuayi.cn

C#:   return (a, b);              // ValueTuple
来源：http://pw.521024.cn

[C06] 匿名函数 / lambda
来源：http://by.newstarts.cn

Py:   square = lambda x: x * x
来源：http://zw.bjjhwx.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://cv.panjiajie.cn

JS:   const square = x => x * x;
来源：http://sf.asd995.cn

TS:   const square = (x: number): number => x * x;
来源：http://gp.szsharing.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mq.szsharing.cn

Go:   sq := func(x int) int { return x * x }
来源：http://jq.nszjky.cn

Ruby: square = ->(x) { x * x }
来源：http://bp.9csxet.cn

C#:   Func<int, int> square = x => x * x;
来源：http://pq.wgjwhj.cn

[C07] 把函数作为参数传入
来源：http://zi.bjjhwx.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ka.szxytkj.cn

PHP:  array_map("strtoupper", $arr);
来源：http://by.wgjwhj.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://it.gzmigu.cn

TS:   arr.map(String)
来源：http://ns.jctech888.com.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://av.wgjwhj.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hc.gzmigu.cn

Ruby: arr.map(&:upcase)
来源：http://jv.521024.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://dm.yuexingan06.cn

[C08] 闭包
来源：http://sf.newstarts.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://nu.szxytkj.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://cz.nszjky.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ii.hnjuh.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://dg.shxzukj.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://oz.gzmigu.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ob.huanxung.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://za.haigaiapp.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://kd.huixinmuqiang.cn

[C09] 递归
来源：http://ig.521024.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://sb.chemitech.net.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://bw.nszjky.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://en.muxihuayi.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://lu.shxzskj.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ff.bjjhwx.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://oj.bjjhwx.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://in.9csxet.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://yo.shtwfgs.cn

[C10] 变量作用域
来源：http://qe.yuexingan06.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://dg.gzmigu.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://gu.muxihuayi.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://dw.jianghongdianzi.cn

TS:   同 JS
来源：http://gw.asd995.cn

Java: 方法内为块级作用域
来源：http://qk.newstarts.cn

Go:   花括号块级作用域
来源：http://yb.newstarts.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://jw.hahajie.cn

C#:   块级作用域
来源：http://xd.huanxung.cn

[C11] 模块导入与导出
来源：http://qq.szsharing.cn

Py:   from module import func
来源：http://so.chemitech.net.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://tw.jianghongdianzi.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://to.shtwfgs.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://pg.colortex.cn

Java: import java.util.List;
来源：http://vd.bookmarksfly.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://bx.shtwfgs.cn

Ruby: require "json"; require_relative "./util"
来源：http://yv.hnjuh.cn

C#:   using System.Text;
来源：http://xe.bjjhwx.cn

[C12] 立即执行函数 IIFE
来源：http://hc.hahajie.cn

Py:   (lambda: print("run"))()
来源：http://sx.nszjky.cn

PHP:  (function () { echo "run"; })();
来源：http://yv.shtwfgs.cn

JS:   (() => { console.log("run"); })();
来源：http://kw.huixiangedu.cn

TS:   (() => { console.log("run"); })();
来源：http://sy.bjjhwx.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://bl.yuexingan06.cn

Go:   func() { fmt.Println("run") }()
来源：http://ib.hahajie.cn

Ruby: -> { puts "run" }.call
来源：http://br.yuexingan06.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://da.shtwfgs.cn

[C13] 类型声明 / 类型注解
来源：http://gr.hahajie.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://av.panjiajie.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://nc.yuexingan06.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://os.asd995.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hi.huixinmuqiang.cn

Java: int add(int a, int b) { return a + b; }
来源：http://et.newstarts.cn

Go:   func add(a, b int) int
来源：http://cr.gzmigu.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://bn.yuntaijiaju.cn

C#:   int Add(int a, int b) => a + b;
来源：http://gy.shtwfgs.cn

[C14] 泛型函数
来源：http://mq.gzmigu.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ny.521024.cn

PHP:  // 无泛型
来源：http://wh.panjiajie.cn

JS:   // 无泛型
来源：http://ku.newstarts.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://sz.9csxet.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://zg.huanxung.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://qj.colortex.cn

Ruby: # 无泛型
来源：http://on.bjjhwx.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://db.szsharing.cn

[C15] 解构 / 展开参数
来源：http://ix.nicolike.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://qv.nszjky.cn

PHP:  [$a, $b] = $pair;
来源：http://up.asd995.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://gj.szsharing.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://yy.nicolike.cn

Java: // 无解构
来源：http://za.hnjuh.cn

Go:   // 无解构
来源：http://co.szxytkj.cn

Ruby: a, b = pair
来源：http://fg.bjjhwx.cn

C#:   var (a, b) = pair;
来源：http://qh.nicolike.cn

[C16] 函数 / 方法重载
来源：http://vu.shtwfgs.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://sl.huixiangedu.cn

PHP:  // 无重载
来源：http://pp.newstarts.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ud.jctech888.com.cn

TS:   // 用联合类型或重载签名声明
来源：http://ws.jianghongdianzi.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://sw.yuntaijiaju.cn

Go:   // 无重载：用不同函数名
来源：http://wj.yuntaijiaju.cn

Ruby: # 无重载：靠动态参数
来源：http://vb.gzmigu.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://dt.wgjwhj.cn

================================================================================
来源：http://vd.hahajie.cn

D. 数组 / 列表 / 集合
来源：http://ey.bookmarksfly.cn

================================================================================
来源：http://ci.nicolike.cn

[D01] 创建数组 / 列表
来源：http://gh.nicolike.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://yc.jctech888.com.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://sb.hahajie.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://rc.huixinmuqiang.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://yb.haigaiapp.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hq.haigaiapp.cn


<!-- 参考信息 -->