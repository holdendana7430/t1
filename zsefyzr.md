代发 wailian999

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://cy.wgjwhj.cn

================================================================================
来源：http://lj.szsharing.cn

B. 流程控制
来源：http://ro.shxzukj.cn

================================================================================
来源：http://xr.huixinmuqiang.cn

[B01] 条件判断 if / else
来源：http://jw.yuntaijiaju.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://hi.colortex.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://xx.szxytkj.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://iw.521024.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://cp.hahajie.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ii.521024.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://iy.hnjuh.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://gp.chemitech.net.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://oa.huixinmuqiang.cn

[B02] 多分支 else if / elif
来源：http://vq.chemitech.net.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://fw.hnjuh.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://vv.newstarts.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://og.huixinmuqiang.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zv.shxzukj.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://iu.panjiajie.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://xd.shtwfgs.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://lr.521024.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ye.jianghongdianzi.cn

[B03] switch / match / case
来源：http://uu.chemitech.net.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://yt.nszjky.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ad.shxzskj.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wv.yuntaijiaju.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hq.muxihuayi.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://la.521024.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://cs.bjjhwx.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://eb.nicolike.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://qa.shtwfgs.cn

[B04] for 计数循环
来源：http://um.huixinmuqiang.cn

Py:   for i in range(10): print(i)
来源：http://xz.hnjuh.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://je.jianghongdianzi.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mz.newstarts.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://tk.jianghongdianzi.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://os.jctech888.com.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://zs.hnjuh.cn

Ruby: 10.times { |i| puts i }
来源：http://an.huixiangedu.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hn.hahajie.cn

[B05] 遍历数组 / 列表
来源：http://il.shxzukj.cn

Py:   for item in arr: print(item)
来源：http://vn.chemitech.net.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ke.szsharing.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://lv.hnjuh.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://hu.nicolike.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://kn.panjiajie.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://op.huanxung.cn

Ruby: arr.each { |item| puts item }
来源：http://ga.szxytkj.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://es.haigaiapp.cn

[B06] 遍历字典 / 对象
来源：http://fl.jctech888.com.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://jg.wgjwhj.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ck.521024.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://tg.yuexingan06.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ne.9csxet.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://yx.nszjky.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hm.jctech888.com.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://kc.521024.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://cz.haigaiapp.cn

[B07] while 循环
来源：http://ai.shxzukj.cn

Py:   while i < 10: i += 1
来源：http://em.szxytkj.cn

PHP:  while ($i < 10) { $i++; }
来源：http://wu.gzmigu.cn

JS:   while (i < 10) { i++; }
来源：http://ei.szsharing.cn

TS:   while (i < 10) { i++; }
来源：http://ra.bookmarksfly.cn

Java: while (i < 10) { i++; }
来源：http://tn.gzmigu.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://qv.yuntaijiaju.cn

Ruby: while i < 10; i += 1; end
来源：http://tt.gzmigu.cn

C#:   while (i < 10) { i++; }
来源：http://wv.asd995.cn

[B08] do-while（至少执行一次）
来源：http://pm.wgjwhj.cn

Py:   # 无 do-while：用 while True + break
来源：http://it.9csxet.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://cc.panjiajie.cn

JS:   do { i++; } while (i < 10);
来源：http://bl.9csxet.cn

TS:   do { i++; } while (i < 10);
来源：http://xb.521024.cn

Java: do { i++; } while (i < 10);
来源：http://wc.521024.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://lj.panjiajie.cn

Ruby: begin; i += 1; end while i < 10
来源：http://sm.hnjuh.cn

C#:   do { i++; } while (i < 10);
来源：http://pg.nszjky.cn

[B09] break 与 continue
来源：http://ms.nicolike.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://dl.szxytkj.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://sm.haigaiapp.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gg.chemitech.net.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rk.chemitech.net.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fp.newstarts.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ds.gzmigu.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://es.nicolike.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nr.shtwfgs.cn

[B10] 遍历同时拿索引
来源：http://zr.hnjuh.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://iz.asd995.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://vm.wgjwhj.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wx.haigaiapp.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://kp.hahajie.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://iz.yuexingan06.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wo.chemitech.net.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ko.wgjwhj.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://af.bookmarksfly.cn

[B11] 生成数字序列 / 区间
来源：http://rw.shxzukj.cn

Py:   list(range(0, 10, 2))
来源：http://wf.521024.cn

PHP:  range(0, 10, 2);
来源：http://xj.haigaiapp.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://eb.lnxyls.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wl.gzmigu.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://fd.huixiangedu.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://rk.shxzukj.cn

Ruby: (0...10).step(2).to_a
来源：http://ew.chemitech.net.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://nc.nicolike.cn

[B12] 跳出多层循环
来源：http://ts.yuntaijiaju.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://tn.shtwfgs.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://yf.nicolike.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://tl.hahajie.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://nv.hnjuh.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://tk.wgjwhj.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hq.nicolike.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://zx.nicolike.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://fr.jianghongdianzi.cn

[B13] 判断是否为数字
来源：http://ho.lnxyls.cn

Py:   isinstance(x, (int, float))
来源：http://aq.huixinmuqiang.cn

PHP:  is_numeric($x)
来源：http://vm.asd995.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xz.haigaiapp.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://da.nszjky.cn

Java: x instanceof Number
来源：http://qj.asd995.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://aw.bjjhwx.cn

Ruby: x.is_a?(Numeric)
来源：http://oz.chemitech.net.cn

C#:   x is int or double or decimal
来源：http://qx.yuntaijiaju.cn

[B14] 判断值是否在集合内
来源：http://be.colortex.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://rl.szsharing.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://eq.bjjhwx.cn

JS:   [1, 2, 3].includes(x)
来源：http://ve.bookmarksfly.cn

TS:   [1, 2, 3].includes(x)
来源：http://hz.asd995.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://wl.panjiajie.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://av.shxzukj.cn

Ruby: [1, 2, 3].include?(x)
来源：http://tt.shxzukj.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://we.nicolike.cn

[B15] 布尔运算与取反
来源：http://nw.nicolike.cn

Py:   a and b or not c
来源：http://ke.asd995.cn

PHP:  $a && $b || !$c
来源：http://ax.shtwfgs.cn

JS:   a && b || !c
来源：http://tw.hahajie.cn

TS:   a && b || !c
来源：http://li.newstarts.cn

Java: a && b || !c
来源：http://cw.muxihuayi.cn

Go:   a && b || !c
来源：http://ib.bookmarksfly.cn

Ruby: a && b || !c
来源：http://jj.wgjwhj.cn

C#:   a && b || !c
来源：http://ql.jianghongdianzi.cn

[B16] 卫语句：不满足条件提前返回
来源：http://jk.nszjky.cn

Py:   if not data: return
来源：http://ma.chemitech.net.cn

PHP:  if (!$data) { return; }
来源：http://lt.szxytkj.cn

JS:   if (!data) return;
来源：http://tp.hnjuh.cn

TS:   if (!data) return;
来源：http://vb.nicolike.cn

Java: if (data == null) return;
来源：http://qa.chemitech.net.cn

Go:   if data == nil { return }
来源：http://nw.nicolike.cn

Ruby: return if data.nil?
来源：http://va.szxytkj.cn

C#:   if (data == null) return;
来源：http://jr.jctech888.com.cn

================================================================================
来源：http://wq.shtwfgs.cn

C. 函数与作用域
来源：http://gx.panjiajie.cn

================================================================================
来源：http://eg.huanxung.cn

[C01] 定义函数
来源：http://bu.colortex.cn

Py:   def add(a, b): return a + b
来源：http://gw.shtwfgs.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://nq.521024.cn

JS:   function add(a, b) { return a + b; }
来源：http://ex.jianghongdianzi.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ux.bjjhwx.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://vb.asd995.cn

Go:   func add(a, b int) int { return a + b }
来源：http://hg.huixiangedu.cn

Ruby: def add(a, b); a + b; end
来源：http://sx.shxzukj.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://fz.szxytkj.cn

[C02] 默认参数
来源：http://pa.yuexingan06.cn

Py:   def greet(name="World"): return name
来源：http://ls.jianghongdianzi.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://ah.haigaiapp.cn

JS:   function greet(name = "World") { return name; }
来源：http://md.521024.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://er.nszjky.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://tj.shxzukj.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://qg.jctech888.com.cn

Ruby: def greet(name = "World") = name
来源：http://iq.colortex.cn

C#:   string Greet(string name = "World") => name;
来源：http://jy.colortex.cn

[C03] 可变参数
来源：http://fc.yuexingan06.cn

Py:   def total(*args): return sum(args)
来源：http://lu.shtwfgs.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://xf.panjiajie.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://qn.haigaiapp.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://nj.jctech888.com.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://jh.newstarts.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://up.shtwfgs.cn

Ruby: def total(*nums); nums.sum; end
来源：http://th.szxytkj.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://km.panjiajie.cn

[C04] 命名参数 / 关键字参数
来源：http://zr.shxzskj.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://uz.wgjwhj.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://gv.chemitech.net.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://gv.muxihuayi.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mi.haigaiapp.cn

Java: // 无：用 Builder 模式或 record
来源：http://li.huanxung.cn

Go:   // 无：用配置结构体参数
来源：http://ph.szsharing.cn

Ruby: f(a: 1, b: 2)
来源：http://ix.jctech888.com.cn

C#:   f(a: 1, b: 2)
来源：http://ic.chemitech.net.cn

[C05] 返回多个值
来源：http://ci.shxzukj.cn

Py:   return a, b
来源：http://yx.yuexingan06.cn

PHP:  return [$a, $b];
来源：http://rj.9csxet.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ps.muxihuayi.cn

TS:   return { a, b };
来源：http://ny.huanxung.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://py.chemitech.net.cn

Go:   return a, b
来源：http://ng.shxzukj.cn

Ruby: return a, b
来源：http://qq.yuexingan06.cn

C#:   return (a, b);              // ValueTuple
来源：http://dc.gzmigu.cn

[C06] 匿名函数 / lambda
来源：http://dt.haigaiapp.cn

Py:   square = lambda x: x * x
来源：http://lc.szsharing.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://op.shtwfgs.cn

JS:   const square = x => x * x;
来源：http://ae.9csxet.cn

TS:   const square = (x: number): number => x * x;
来源：http://sl.hahajie.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ml.shxzskj.cn

Go:   sq := func(x int) int { return x * x }
来源：http://yw.nicolike.cn

Ruby: square = ->(x) { x * x }
来源：http://ph.chemitech.net.cn

C#:   Func<int, int> square = x => x * x;
来源：http://kd.shxzskj.cn

[C07] 把函数作为参数传入
来源：http://tk.huixinmuqiang.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ia.shtwfgs.cn

PHP:  array_map("strtoupper", $arr);
来源：http://fg.shxzukj.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://xo.szxytkj.cn

TS:   arr.map(String)
来源：http://ga.bookmarksfly.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mu.9csxet.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://vi.yuexingan06.cn

Ruby: arr.map(&:upcase)
来源：http://bq.gzmigu.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://de.chemitech.net.cn

[C08] 闭包
来源：http://cf.9csxet.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://dw.panjiajie.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://eo.muxihuayi.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://yt.shxzskj.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://jw.newstarts.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://sx.jctech888.com.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://xy.huixiangedu.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://pn.bjjhwx.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://cj.gzmigu.cn

[C09] 递归
来源：http://yh.gzmigu.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://gp.hnjuh.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ii.jctech888.com.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ul.shtwfgs.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://yh.hnjuh.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ch.yuntaijiaju.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://iy.521024.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://bb.asd995.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hc.haigaiapp.cn

[C10] 变量作用域
来源：http://kg.yuexingan06.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://fx.yuntaijiaju.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://um.shtwfgs.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://sr.nszjky.cn

TS:   同 JS
来源：http://pw.hahajie.cn

Java: 方法内为块级作用域
来源：http://bv.521024.cn

Go:   花括号块级作用域
来源：http://eh.wgjwhj.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://bw.bookmarksfly.cn

C#:   块级作用域
来源：http://zp.chemitech.net.cn

[C11] 模块导入与导出
来源：http://fm.shxzukj.cn

Py:   from module import func
来源：http://pp.521024.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://dk.newstarts.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://hi.yuexingan06.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wz.hahajie.cn

Java: import java.util.List;
来源：http://dt.shxzukj.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://eg.521024.cn

Ruby: require "json"; require_relative "./util"
来源：http://vg.huanxung.cn

C#:   using System.Text;
来源：http://rs.wgjwhj.cn

[C12] 立即执行函数 IIFE
来源：http://xx.huixiangedu.cn

Py:   (lambda: print("run"))()
来源：http://zo.shxzukj.cn

PHP:  (function () { echo "run"; })();
来源：http://dc.bookmarksfly.cn

JS:   (() => { console.log("run"); })();
来源：http://vw.521024.cn

TS:   (() => { console.log("run"); })();
来源：http://uc.wgjwhj.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://vz.colortex.cn

Go:   func() { fmt.Println("run") }()
来源：http://qv.yuntaijiaju.cn

Ruby: -> { puts "run" }.call
来源：http://dl.bookmarksfly.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://wl.asd995.cn

[C13] 类型声明 / 类型注解
来源：http://tc.9csxet.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://jd.lnxyls.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://sl.huixiangedu.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://iz.colortex.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://vf.shtwfgs.cn

Java: int add(int a, int b) { return a + b; }
来源：http://xd.bjjhwx.cn

Go:   func add(a, b int) int
来源：http://du.asd995.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hl.haigaiapp.cn

C#:   int Add(int a, int b) => a + b;
来源：http://vx.jianghongdianzi.cn

[C14] 泛型函数
来源：http://ge.nszjky.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://pq.lnxyls.cn

PHP:  // 无泛型
来源：http://bv.szxytkj.cn

JS:   // 无泛型
来源：http://rn.huixinmuqiang.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://la.gzmigu.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://lp.panjiajie.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ux.szxytkj.cn

Ruby: # 无泛型
来源：http://mx.hahajie.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mz.wgjwhj.cn

[C15] 解构 / 展开参数
来源：http://ut.wgjwhj.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://nt.shtwfgs.cn

PHP:  [$a, $b] = $pair;
来源：http://gv.muxihuayi.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://uz.bjjhwx.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://jw.bookmarksfly.cn

Java: // 无解构
来源：http://gg.521024.cn

Go:   // 无解构
来源：http://qy.huixinmuqiang.cn

Ruby: a, b = pair
来源：http://na.muxihuayi.cn

C#:   var (a, b) = pair;
来源：http://fi.huixinmuqiang.cn

[C16] 函数 / 方法重载
来源：http://qh.shtwfgs.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mi.colortex.cn

PHP:  // 无重载
来源：http://ha.huixiangedu.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://pz.yuntaijiaju.cn

TS:   // 用联合类型或重载签名声明
来源：http://nu.bookmarksfly.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://yb.jianghongdianzi.cn

Go:   // 无重载：用不同函数名
来源：http://bw.9csxet.cn

Ruby: # 无重载：靠动态参数
来源：http://kn.muxihuayi.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ko.nicolike.cn

================================================================================
来源：http://mq.wgjwhj.cn

D. 数组 / 列表 / 集合
来源：http://fk.shtwfgs.cn

================================================================================
来源：http://sb.wgjwhj.cn

[D01] 创建数组 / 列表
来源：http://eo.panjiajie.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ti.hahajie.cn


<!-- 参考信息 -->