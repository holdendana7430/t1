代发 wailian999

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://pn.szsharing.cn

================================================================================
来源：http://ci.colortex.cn

B. 流程控制
来源：http://ep.szxytkj.cn

================================================================================
来源：http://xs.hnjuh.cn

[B01] 条件判断 if / else
来源：http://al.huixinmuqiang.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://nv.gzmigu.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hb.shtwfgs.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://at.hnjuh.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://yr.huixiangedu.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://oj.huanxung.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://sk.szxytkj.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://qh.lnxyls.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://le.szsharing.cn

[B02] 多分支 else if / elif
来源：http://uu.muxihuayi.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://fr.panjiajie.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://wt.wgjwhj.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xu.shtwfgs.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yo.jctech888.com.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zq.jianghongdianzi.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://jt.gzmigu.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://jo.shtwfgs.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ad.9csxet.cn

[B03] switch / match / case
来源：http://il.lnxyls.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://qa.521024.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ig.gzmigu.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://kv.asd995.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ur.muxihuayi.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://sz.hnjuh.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://kj.shtwfgs.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://zo.huanxung.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://oh.521024.cn

[B04] for 计数循环
来源：http://fv.9csxet.cn

Py:   for i in range(10): print(i)
来源：http://jv.panjiajie.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ps.jctech888.com.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://zi.shxzskj.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://kn.shxzukj.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://jo.lnxyls.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://fo.bookmarksfly.cn

Ruby: 10.times { |i| puts i }
来源：http://ou.huixiangedu.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://cx.nszjky.cn

[B05] 遍历数组 / 列表
来源：http://yc.yuntaijiaju.cn

Py:   for item in arr: print(item)
来源：http://na.asd995.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ap.asd995.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://am.9csxet.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://lz.9csxet.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://nk.huixinmuqiang.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://as.shxzukj.cn

Ruby: arr.each { |item| puts item }
来源：http://ez.521024.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ag.jctech888.com.cn

[B06] 遍历字典 / 对象
来源：http://zw.nicolike.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://bn.shtwfgs.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://vj.521024.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wy.bookmarksfly.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://qs.huixiangedu.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ae.chemitech.net.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://fr.huanxung.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ak.newstarts.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://yk.9csxet.cn

[B07] while 循环
来源：http://ns.bjjhwx.cn

Py:   while i < 10: i += 1
来源：http://ri.szsharing.cn

PHP:  while ($i < 10) { $i++; }
来源：http://md.hahajie.cn

JS:   while (i < 10) { i++; }
来源：http://an.muxihuayi.cn

TS:   while (i < 10) { i++; }
来源：http://rh.gzmigu.cn

Java: while (i < 10) { i++; }
来源：http://wz.jctech888.com.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://dz.yuntaijiaju.cn

Ruby: while i < 10; i += 1; end
来源：http://jw.asd995.cn

C#:   while (i < 10) { i++; }
来源：http://dt.huixinmuqiang.cn

[B08] do-while（至少执行一次）
来源：http://ht.jianghongdianzi.cn

Py:   # 无 do-while：用 while True + break
来源：http://nh.asd995.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://bd.lnxyls.cn

JS:   do { i++; } while (i < 10);
来源：http://kx.hahajie.cn

TS:   do { i++; } while (i < 10);
来源：http://jl.haigaiapp.cn

Java: do { i++; } while (i < 10);
来源：http://qm.gzmigu.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://iy.shtwfgs.cn

Ruby: begin; i += 1; end while i < 10
来源：http://av.muxihuayi.cn

C#:   do { i++; } while (i < 10);
来源：http://xj.shxzskj.cn

[B09] break 与 continue
来源：http://if.asd995.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://pv.muxihuayi.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://oz.muxihuayi.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lc.huixinmuqiang.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://es.bjjhwx.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hj.hnjuh.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://or.hnjuh.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ec.jctech888.com.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fe.hnjuh.cn

[B10] 遍历同时拿索引
来源：http://rl.shtwfgs.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://cg.wgjwhj.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://kl.lnxyls.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ha.wgjwhj.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://un.521024.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://te.hahajie.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://sv.colortex.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://gp.colortex.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hf.huanxung.cn

[B11] 生成数字序列 / 区间
来源：http://oj.szsharing.cn

Py:   list(range(0, 10, 2))
来源：http://tm.huixinmuqiang.cn

PHP:  range(0, 10, 2);
来源：http://ml.shtwfgs.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ve.jianghongdianzi.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ru.lnxyls.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://yp.huanxung.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ur.huanxung.cn

Ruby: (0...10).step(2).to_a
来源：http://mr.newstarts.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://uj.colortex.cn

[B12] 跳出多层循环
来源：http://cj.521024.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://hr.shxzukj.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://jq.asd995.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ds.newstarts.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://pm.shxzukj.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://xl.521024.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://uw.hahajie.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wl.muxihuayi.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://jf.gzmigu.cn

[B13] 判断是否为数字
来源：http://sz.9csxet.cn

Py:   isinstance(x, (int, float))
来源：http://xa.szxytkj.cn

PHP:  is_numeric($x)
来源：http://dq.szxytkj.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://na.lnxyls.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://dc.9csxet.cn

Java: x instanceof Number
来源：http://mk.gzmigu.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://do.huanxung.cn

Ruby: x.is_a?(Numeric)
来源：http://kw.colortex.cn

C#:   x is int or double or decimal
来源：http://vx.bjjhwx.cn

[B14] 判断值是否在集合内
来源：http://au.bookmarksfly.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://za.jctech888.com.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ml.szsharing.cn

JS:   [1, 2, 3].includes(x)
来源：http://qu.yuexingan06.cn

TS:   [1, 2, 3].includes(x)
来源：http://ak.hnjuh.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://tc.bjjhwx.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://lk.521024.cn

Ruby: [1, 2, 3].include?(x)
来源：http://iy.lnxyls.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://nu.hnjuh.cn

[B15] 布尔运算与取反
来源：http://yd.hahajie.cn

Py:   a and b or not c
来源：http://gv.9csxet.cn

PHP:  $a && $b || !$c
来源：http://ny.shxzskj.cn

JS:   a && b || !c
来源：http://vg.bookmarksfly.cn

TS:   a && b || !c
来源：http://la.shxzskj.cn

Java: a && b || !c
来源：http://gu.panjiajie.cn

Go:   a && b || !c
来源：http://rd.haigaiapp.cn

Ruby: a && b || !c
来源：http://jt.newstarts.cn

C#:   a && b || !c
来源：http://la.haigaiapp.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ec.yuntaijiaju.cn

Py:   if not data: return
来源：http://xx.szxytkj.cn

PHP:  if (!$data) { return; }
来源：http://ab.panjiajie.cn

JS:   if (!data) return;
来源：http://fk.nszjky.cn

TS:   if (!data) return;
来源：http://vn.haigaiapp.cn

Java: if (data == null) return;
来源：http://iz.gzmigu.cn

Go:   if data == nil { return }
来源：http://yn.wgjwhj.cn

Ruby: return if data.nil?
来源：http://tw.colortex.cn

C#:   if (data == null) return;
来源：http://al.lnxyls.cn

================================================================================
来源：http://eu.hnjuh.cn

C. 函数与作用域
来源：http://my.hnjuh.cn

================================================================================
来源：http://bw.huixiangedu.cn

[C01] 定义函数
来源：http://zz.jctech888.com.cn

Py:   def add(a, b): return a + b
来源：http://el.lnxyls.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://tj.chemitech.net.cn

JS:   function add(a, b) { return a + b; }
来源：http://nv.shxzskj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://fp.9csxet.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://uz.szsharing.cn

Go:   func add(a, b int) int { return a + b }
来源：http://zi.szsharing.cn

Ruby: def add(a, b); a + b; end
来源：http://ur.hahajie.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://sq.hahajie.cn

[C02] 默认参数
来源：http://kw.hnjuh.cn

Py:   def greet(name="World"): return name
来源：http://ku.asd995.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://dy.asd995.cn

JS:   function greet(name = "World") { return name; }
来源：http://bo.hnjuh.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://rk.colortex.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://cm.hahajie.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://gk.hnjuh.cn

Ruby: def greet(name = "World") = name
来源：http://hb.panjiajie.cn

C#:   string Greet(string name = "World") => name;
来源：http://xt.szsharing.cn

[C03] 可变参数
来源：http://oq.panjiajie.cn

Py:   def total(*args): return sum(args)
来源：http://zk.hnjuh.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://yw.lnxyls.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wb.szxytkj.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://sb.gzmigu.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mp.jianghongdianzi.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ye.newstarts.cn

Ruby: def total(*nums); nums.sum; end
来源：http://he.shtwfgs.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://cs.haigaiapp.cn

[C04] 命名参数 / 关键字参数
来源：http://ce.chemitech.net.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://rf.szsharing.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wl.panjiajie.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://eg.huixiangedu.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mk.huixinmuqiang.cn

Java: // 无：用 Builder 模式或 record
来源：http://lc.jianghongdianzi.cn

Go:   // 无：用配置结构体参数
来源：http://vg.asd995.cn

Ruby: f(a: 1, b: 2)
来源：http://fr.521024.cn

C#:   f(a: 1, b: 2)
来源：http://ay.bookmarksfly.cn

[C05] 返回多个值
来源：http://ab.nszjky.cn

Py:   return a, b
来源：http://nr.bookmarksfly.cn

PHP:  return [$a, $b];
来源：http://lh.jctech888.com.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://al.huixinmuqiang.cn

TS:   return { a, b };
来源：http://zs.shxzukj.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://tj.szxytkj.cn

Go:   return a, b
来源：http://fb.panjiajie.cn

Ruby: return a, b
来源：http://id.huixinmuqiang.cn

C#:   return (a, b);              // ValueTuple
来源：http://jo.chemitech.net.cn

[C06] 匿名函数 / lambda
来源：http://or.haigaiapp.cn

Py:   square = lambda x: x * x
来源：http://zx.shtwfgs.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://jx.nszjky.cn

JS:   const square = x => x * x;
来源：http://hk.szsharing.cn

TS:   const square = (x: number): number => x * x;
来源：http://no.lnxyls.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://gx.asd995.cn

Go:   sq := func(x int) int { return x * x }
来源：http://is.shtwfgs.cn

Ruby: square = ->(x) { x * x }
来源：http://nd.szsharing.cn

C#:   Func<int, int> square = x => x * x;
来源：http://bq.shxzskj.cn

[C07] 把函数作为参数传入
来源：http://wj.huanxung.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ds.jctech888.com.cn

PHP:  array_map("strtoupper", $arr);
来源：http://to.yuexingan06.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://qi.gzmigu.cn

TS:   arr.map(String)
来源：http://en.bookmarksfly.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://kb.yuexingan06.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://qu.521024.cn

Ruby: arr.map(&:upcase)
来源：http://ln.shxzukj.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ah.shxzskj.cn

[C08] 闭包
来源：http://ci.hahajie.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://eh.asd995.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://nv.asd995.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mm.huixinmuqiang.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://vf.newstarts.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://kl.yuexingan06.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://iw.asd995.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://km.gzmigu.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://kr.bjjhwx.cn

[C09] 递归
来源：http://fp.bjjhwx.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://xb.nicolike.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://su.muxihuayi.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://jf.haigaiapp.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://si.yuntaijiaju.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://xd.yuexingan06.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://th.colortex.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://bv.panjiajie.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ee.nicolike.cn

[C10] 变量作用域
来源：http://yw.jctech888.com.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://fp.yuexingan06.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://rm.yuntaijiaju.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wj.bjjhwx.cn

TS:   同 JS
来源：http://do.hnjuh.cn

Java: 方法内为块级作用域
来源：http://vh.yuexingan06.cn

Go:   花括号块级作用域
来源：http://no.haigaiapp.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://xf.gzmigu.cn

C#:   块级作用域
来源：http://ki.jianghongdianzi.cn

[C11] 模块导入与导出
来源：http://rs.chemitech.net.cn

Py:   from module import func
来源：http://dj.bookmarksfly.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://sv.hahajie.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://mk.newstarts.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://st.haigaiapp.cn

Java: import java.util.List;
来源：http://dz.colortex.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://gf.yuntaijiaju.cn

Ruby: require "json"; require_relative "./util"
来源：http://qq.521024.cn

C#:   using System.Text;
来源：http://js.yuntaijiaju.cn

[C12] 立即执行函数 IIFE
来源：http://zp.asd995.cn

Py:   (lambda: print("run"))()
来源：http://ka.shxzskj.cn

PHP:  (function () { echo "run"; })();
来源：http://ka.shtwfgs.cn

JS:   (() => { console.log("run"); })();
来源：http://lz.shxzukj.cn

TS:   (() => { console.log("run"); })();
来源：http://lc.chemitech.net.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://we.nszjky.cn

Go:   func() { fmt.Println("run") }()
来源：http://ak.haigaiapp.cn

Ruby: -> { puts "run" }.call
来源：http://dg.szsharing.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://jc.jianghongdianzi.cn

[C13] 类型声明 / 类型注解
来源：http://av.huixinmuqiang.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://an.szsharing.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://kh.yuexingan06.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://xl.hahajie.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://tz.shxzskj.cn

Java: int add(int a, int b) { return a + b; }
来源：http://ka.panjiajie.cn

Go:   func add(a, b int) int
来源：http://jd.hnjuh.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://rc.9csxet.cn

C#:   int Add(int a, int b) => a + b;
来源：http://tl.haigaiapp.cn

[C14] 泛型函数
来源：http://zh.yuntaijiaju.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://zu.panjiajie.cn

PHP:  // 无泛型
来源：http://km.haigaiapp.cn

JS:   // 无泛型
来源：http://we.nszjky.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://lt.haigaiapp.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://br.bookmarksfly.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://nc.newstarts.cn

Ruby: # 无泛型
来源：http://el.hnjuh.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://fd.chemitech.net.cn

[C15] 解构 / 展开参数
来源：http://ux.asd995.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://vc.szxytkj.cn

PHP:  [$a, $b] = $pair;
来源：http://gj.bookmarksfly.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://is.newstarts.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://dz.jctech888.com.cn

Java: // 无解构
来源：http://nn.muxihuayi.cn

Go:   // 无解构
来源：http://iz.nicolike.cn

Ruby: a, b = pair
来源：http://op.asd995.cn

C#:   var (a, b) = pair;
来源：http://ao.nszjky.cn

[C16] 函数 / 方法重载
来源：http://kr.shxzukj.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://fl.chemitech.net.cn

PHP:  // 无重载
来源：http://vz.bookmarksfly.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://os.yuntaijiaju.cn

TS:   // 用联合类型或重载签名声明
来源：http://zr.jianghongdianzi.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://lc.newstarts.cn

Go:   // 无重载：用不同函数名
来源：http://hj.huanxung.cn

Ruby: # 无重载：靠动态参数
来源：http://bz.bjjhwx.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://kc.lnxyls.cn

================================================================================
来源：http://st.szsharing.cn

D. 数组 / 列表 / 集合
来源：http://ih.jianghongdianzi.cn

================================================================================
来源：http://ea.asd995.cn

[D01] 创建数组 / 列表
来源：http://sf.nszjky.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://op.huixinmuqiang.cn


<!-- 参考信息 -->