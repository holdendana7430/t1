代发 wailian999

[B01] 条件判断 if / else
来源：http://jo.9csxet.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://cw.9csxet.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://jm.9csxet.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://jk.shtwfgs.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://xx.colortex.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://nf.shxzukj.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://mg.colortex.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ey.huixinmuqiang.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://iq.521024.cn

[B02] 多分支 else if / elif
来源：http://xk.hahajie.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://fc.chemitech.net.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ai.jianghongdianzi.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gz.jianghongdianzi.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hv.colortex.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://na.muxihuayi.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://kp.wgjwhj.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://wa.colortex.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nl.nszjky.cn

[B03] switch / match / case
来源：http://ea.szsharing.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ax.gzmigu.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://xo.yuexingan06.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://cm.asd995.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://na.muxihuayi.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://wp.hnjuh.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://yg.chemitech.net.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ia.newstarts.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://kv.shxzskj.cn

[B04] for 计数循环
来源：http://na.hnjuh.cn

Py:   for i in range(10): print(i)
来源：http://wx.haigaiapp.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://oz.gzmigu.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://vy.bookmarksfly.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://pc.bjjhwx.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://md.huixiangedu.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://zk.yuntaijiaju.cn

Ruby: 10.times { |i| puts i }
来源：http://mg.521024.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://zb.muxihuayi.cn

[B05] 遍历数组 / 列表
来源：http://cd.521024.cn

Py:   for item in arr: print(item)
来源：http://mk.nicolike.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ro.nicolike.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://tv.newstarts.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ln.shtwfgs.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://xp.bjjhwx.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ux.huanxung.cn

Ruby: arr.each { |item| puts item }
来源：http://sg.huanxung.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://tp.asd995.cn

[B06] 遍历字典 / 对象
来源：http://nw.bjjhwx.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ps.hnjuh.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://zs.bjjhwx.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hw.huixinmuqiang.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://pl.bjjhwx.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://om.yuntaijiaju.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://qs.colortex.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://kz.yuexingan06.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ap.shtwfgs.cn

[B07] while 循环
来源：http://ge.huixiangedu.cn

Py:   while i < 10: i += 1
来源：http://qg.newstarts.cn

PHP:  while ($i < 10) { $i++; }
来源：http://di.colortex.cn

JS:   while (i < 10) { i++; }
来源：http://zz.colortex.cn

TS:   while (i < 10) { i++; }
来源：http://qs.yuexingan06.cn

Java: while (i < 10) { i++; }
来源：http://gw.bookmarksfly.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://mu.panjiajie.cn

Ruby: while i < 10; i += 1; end
来源：http://tc.panjiajie.cn

C#:   while (i < 10) { i++; }
来源：http://bu.gzmigu.cn

[B08] do-while（至少执行一次）
来源：http://dj.huixiangedu.cn

Py:   # 无 do-while：用 while True + break
来源：http://vi.hnjuh.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ht.gzmigu.cn

JS:   do { i++; } while (i < 10);
来源：http://dl.huixinmuqiang.cn

TS:   do { i++; } while (i < 10);
来源：http://pg.shxzukj.cn

Java: do { i++; } while (i < 10);
来源：http://hz.muxihuayi.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://bt.asd995.cn

Ruby: begin; i += 1; end while i < 10
来源：http://lk.521024.cn

C#:   do { i++; } while (i < 10);
来源：http://ui.colortex.cn

[B09] break 与 continue
来源：http://di.bjjhwx.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hu.shxzskj.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://fw.shtwfgs.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fz.colortex.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://id.gzmigu.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fz.szxytkj.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ws.521024.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://he.9csxet.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tj.haigaiapp.cn

[B10] 遍历同时拿索引
来源：http://gs.shtwfgs.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://up.huixiangedu.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ty.newstarts.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://zh.shxzukj.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ps.gzmigu.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://th.haigaiapp.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://gq.colortex.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://gj.szsharing.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://jz.bjjhwx.cn

[B11] 生成数字序列 / 区间
来源：http://xb.yuntaijiaju.cn

Py:   list(range(0, 10, 2))
来源：http://xe.newstarts.cn

PHP:  range(0, 10, 2);
来源：http://ro.haigaiapp.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://xb.nszjky.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ey.panjiajie.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://fx.shtwfgs.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://oz.wgjwhj.cn

Ruby: (0...10).step(2).to_a
来源：http://oa.huanxung.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://zs.newstarts.cn

[B12] 跳出多层循环
来源：http://nc.9csxet.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://zm.panjiajie.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://pf.bjjhwx.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://zp.yuexingan06.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wu.bookmarksfly.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://nk.jianghongdianzi.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://gy.colortex.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://qe.jianghongdianzi.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://gl.panjiajie.cn

[B13] 判断是否为数字
来源：http://ni.huixinmuqiang.cn

Py:   isinstance(x, (int, float))
来源：http://nf.huanxung.cn

PHP:  is_numeric($x)
来源：http://vb.wgjwhj.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://tu.hahajie.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://am.colortex.cn

Java: x instanceof Number
来源：http://pn.hahajie.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://yu.521024.cn

Ruby: x.is_a?(Numeric)
来源：http://tz.hnjuh.cn

C#:   x is int or double or decimal
来源：http://eu.shtwfgs.cn

[B14] 判断值是否在集合内
来源：http://gx.huixinmuqiang.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://to.hnjuh.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://os.lnxyls.cn

JS:   [1, 2, 3].includes(x)
来源：http://al.hahajie.cn

TS:   [1, 2, 3].includes(x)
来源：http://ep.colortex.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ct.bjjhwx.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://bb.huixiangedu.cn

Ruby: [1, 2, 3].include?(x)
来源：http://yz.521024.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mo.asd995.cn

[B15] 布尔运算与取反
来源：http://pb.nszjky.cn

Py:   a and b or not c
来源：http://ls.asd995.cn

PHP:  $a && $b || !$c
来源：http://sf.lnxyls.cn

JS:   a && b || !c
来源：http://ha.jianghongdianzi.cn

TS:   a && b || !c
来源：http://al.521024.cn

Java: a && b || !c
来源：http://jg.nicolike.cn

Go:   a && b || !c
来源：http://th.chemitech.net.cn

Ruby: a && b || !c
来源：http://ta.jctech888.com.cn

C#:   a && b || !c
来源：http://ng.hnjuh.cn

[B16] 卫语句：不满足条件提前返回
来源：http://nt.lnxyls.cn

Py:   if not data: return
来源：http://iw.9csxet.cn

PHP:  if (!$data) { return; }
来源：http://ee.9csxet.cn

JS:   if (!data) return;
来源：http://jv.huanxung.cn

TS:   if (!data) return;
来源：http://rl.huixiangedu.cn

Java: if (data == null) return;
来源：http://bu.haigaiapp.cn

Go:   if data == nil { return }
来源：http://sf.shxzskj.cn

Ruby: return if data.nil?
来源：http://ow.9csxet.cn

C#:   if (data == null) return;
来源：http://oo.huixiangedu.cn

================================================================================
来源：http://je.shxzukj.cn

C. 函数与作用域
来源：http://gv.jianghongdianzi.cn

================================================================================
来源：http://pn.panjiajie.cn

[C01] 定义函数
来源：http://ag.muxihuayi.cn

Py:   def add(a, b): return a + b
来源：http://eh.shtwfgs.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ck.hahajie.cn

JS:   function add(a, b) { return a + b; }
来源：http://yq.9csxet.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://se.nicolike.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://nx.szxytkj.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ju.yuexingan06.cn

Ruby: def add(a, b); a + b; end
来源：http://en.nicolike.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://um.nicolike.cn

[C02] 默认参数
来源：http://nq.panjiajie.cn

Py:   def greet(name="World"): return name
来源：http://vv.nicolike.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://nn.shtwfgs.cn

JS:   function greet(name = "World") { return name; }
来源：http://qi.huanxung.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://xv.shxzskj.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://vs.hnjuh.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ui.nicolike.cn

Ruby: def greet(name = "World") = name
来源：http://em.shxzukj.cn

C#:   string Greet(string name = "World") => name;
来源：http://ly.newstarts.cn

[C03] 可变参数
来源：http://dq.huanxung.cn

Py:   def total(*args): return sum(args)
来源：http://sq.panjiajie.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ne.hahajie.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://fm.wgjwhj.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://fk.jianghongdianzi.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://uk.asd995.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://lf.panjiajie.cn

Ruby: def total(*nums); nums.sum; end
来源：http://ey.chemitech.net.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://it.9csxet.cn

[C04] 命名参数 / 关键字参数
来源：http://iu.shxzskj.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://fk.lnxyls.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ty.huixiangedu.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ax.yuntaijiaju.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ap.szxytkj.cn

Java: // 无：用 Builder 模式或 record
来源：http://bx.shtwfgs.cn

Go:   // 无：用配置结构体参数
来源：http://nr.szxytkj.cn

Ruby: f(a: 1, b: 2)
来源：http://vv.panjiajie.cn

C#:   f(a: 1, b: 2)
来源：http://sf.jianghongdianzi.cn

[C05] 返回多个值
来源：http://tr.gzmigu.cn

Py:   return a, b
来源：http://ot.muxihuayi.cn

PHP:  return [$a, $b];
来源：http://ki.colortex.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://uw.huixinmuqiang.cn

TS:   return { a, b };
来源：http://ot.wgjwhj.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wd.chemitech.net.cn

Go:   return a, b
来源：http://av.nszjky.cn

Ruby: return a, b
来源：http://ce.shtwfgs.cn

C#:   return (a, b);              // ValueTuple
来源：http://zi.huixiangedu.cn

[C06] 匿名函数 / lambda
来源：http://jj.shxzukj.cn

Py:   square = lambda x: x * x
来源：http://yx.szsharing.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://cb.jianghongdianzi.cn

JS:   const square = x => x * x;
来源：http://ul.shxzskj.cn

TS:   const square = (x: number): number => x * x;
来源：http://ev.szsharing.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://zo.9csxet.cn

Go:   sq := func(x int) int { return x * x }
来源：http://wb.yuexingan06.cn

Ruby: square = ->(x) { x * x }
来源：http://oh.bookmarksfly.cn

C#:   Func<int, int> square = x => x * x;
来源：http://hl.521024.cn

[C07] 把函数作为参数传入
来源：http://hf.huanxung.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wq.chemitech.net.cn

PHP:  array_map("strtoupper", $arr);
来源：http://vy.bjjhwx.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://kl.muxihuayi.cn

TS:   arr.map(String)
来源：http://iv.lnxyls.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://lh.hnjuh.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://lu.nicolike.cn

Ruby: arr.map(&:upcase)
来源：http://vy.chemitech.net.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ha.huixiangedu.cn

[C08] 闭包
来源：http://ss.nszjky.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://da.haigaiapp.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://lc.szsharing.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ms.huixiangedu.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://en.521024.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wc.521024.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ao.szxytkj.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ud.asd995.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://nk.shtwfgs.cn

[C09] 递归
来源：http://it.nszjky.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://er.szsharing.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://gv.yuntaijiaju.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://fd.szsharing.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://jv.yuexingan06.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://oq.muxihuayi.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mu.hnjuh.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://cd.panjiajie.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://vx.gzmigu.cn

[C10] 变量作用域
来源：http://zb.nszjky.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://or.asd995.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ci.panjiajie.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://op.szxytkj.cn

TS:   同 JS
来源：http://aw.asd995.cn

Java: 方法内为块级作用域
来源：http://oa.nszjky.cn

Go:   花括号块级作用域
来源：http://ry.gzmigu.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://tt.hnjuh.cn

C#:   块级作用域
来源：http://vt.hnjuh.cn

[C11] 模块导入与导出
来源：http://sd.shtwfgs.cn

Py:   from module import func
来源：http://cl.521024.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://ug.yuexingan06.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://kd.jctech888.com.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ek.nicolike.cn

Java: import java.util.List;
来源：http://fb.asd995.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://zn.jctech888.com.cn

Ruby: require "json"; require_relative "./util"
来源：http://ja.9csxet.cn

C#:   using System.Text;
来源：http://mp.jctech888.com.cn

[C12] 立即执行函数 IIFE
来源：http://di.shtwfgs.cn

Py:   (lambda: print("run"))()
来源：http://gc.gzmigu.cn

PHP:  (function () { echo "run"; })();
来源：http://pf.wgjwhj.cn

JS:   (() => { console.log("run"); })();
来源：http://jo.jctech888.com.cn

TS:   (() => { console.log("run"); })();
来源：http://ch.jianghongdianzi.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://fk.panjiajie.cn

Go:   func() { fmt.Println("run") }()
来源：http://qg.jctech888.com.cn

Ruby: -> { puts "run" }.call
来源：http://rh.haigaiapp.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://hu.wgjwhj.cn

[C13] 类型声明 / 类型注解
来源：http://cn.hnjuh.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://pa.yuexingan06.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ph.panjiajie.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://lj.gzmigu.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://rl.panjiajie.cn

Java: int add(int a, int b) { return a + b; }
来源：http://hp.panjiajie.cn

Go:   func add(a, b int) int
来源：http://gu.jianghongdianzi.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://tz.yuntaijiaju.cn

C#:   int Add(int a, int b) => a + b;
来源：http://ri.bjjhwx.cn

[C14] 泛型函数
来源：http://ls.nicolike.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://xf.hahajie.cn

PHP:  // 无泛型
来源：http://qr.newstarts.cn

JS:   // 无泛型
来源：http://lg.wgjwhj.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ja.shtwfgs.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://uq.asd995.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://sh.szxytkj.cn

Ruby: # 无泛型
来源：http://wl.jianghongdianzi.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://cc.colortex.cn

[C15] 解构 / 展开参数
来源：http://ug.colortex.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hh.yuntaijiaju.cn

PHP:  [$a, $b] = $pair;
来源：http://hh.asd995.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://zk.haigaiapp.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://zu.haigaiapp.cn

Java: // 无解构
来源：http://ur.muxihuayi.cn

Go:   // 无解构
来源：http://hq.szsharing.cn

Ruby: a, b = pair
来源：http://yt.shtwfgs.cn

C#:   var (a, b) = pair;
来源：http://nb.bookmarksfly.cn

[C16] 函数 / 方法重载
来源：http://wm.hahajie.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://vn.yuexingan06.cn

PHP:  // 无重载
来源：http://wp.9csxet.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://fh.jianghongdianzi.cn

TS:   // 用联合类型或重载签名声明
来源：http://cl.jctech888.com.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://dh.huanxung.cn

Go:   // 无重载：用不同函数名
来源：http://hg.jctech888.com.cn

Ruby: # 无重载：靠动态参数
来源：http://gd.newstarts.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://gf.hnjuh.cn

================================================================================
来源：http://bl.jctech888.com.cn

D. 数组 / 列表 / 集合
来源：http://gp.szsharing.cn

================================================================================
来源：http://sv.wgjwhj.cn

[D01] 创建数组 / 列表
来源：http://tm.hahajie.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://dk.huanxung.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://tr.panjiajie.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://en.nicolike.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://am.yuexingan06.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://jm.jianghongdianzi.cn


<!-- 参考信息 -->