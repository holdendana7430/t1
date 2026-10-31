代发 wailian999

TS:   const r = x > 0 ? "正" : "非正";
来源：http://oi.bookmarksfly.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://zo.jianghongdianzi.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://rd.shxzskj.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://oe.shxzukj.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ho.yuexingan06.cn

[B02] 多分支 else if / elif
来源：http://fi.huixinmuqiang.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://uz.szxytkj.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://dt.huanxung.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yo.chemitech.net.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tu.wgjwhj.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://km.521024.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://xu.hahajie.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://fe.asd995.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://uo.bookmarksfly.cn

[B03] switch / match / case
来源：http://os.shxzskj.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://nd.muxihuayi.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://sc.huixiangedu.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ac.gzmigu.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://er.nszjky.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ly.521024.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ti.panjiajie.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://dt.szxytkj.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ir.panjiajie.cn

[B04] for 计数循环
来源：http://oa.haigaiapp.cn

Py:   for i in range(10): print(i)
来源：http://kq.szxytkj.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://mp.yuexingan06.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mt.jctech888.com.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://gw.gzmigu.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://tn.haigaiapp.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://rk.szsharing.cn

Ruby: 10.times { |i| puts i }
来源：http://qz.shxzukj.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://bj.shtwfgs.cn

[B05] 遍历数组 / 列表
来源：http://iq.yuexingan06.cn

Py:   for item in arr: print(item)
来源：http://sg.newstarts.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://qb.shxzukj.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://zx.gzmigu.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://tf.hahajie.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://ym.newstarts.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://go.jianghongdianzi.cn

Ruby: arr.each { |item| puts item }
来源：http://ym.haigaiapp.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://iz.asd995.cn

[B06] 遍历字典 / 对象
来源：http://rh.huixinmuqiang.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://gd.jianghongdianzi.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://xz.huanxung.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://pu.nicolike.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://lq.muxihuayi.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://yp.nszjky.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ro.chemitech.net.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://cd.colortex.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://jo.jianghongdianzi.cn

[B07] while 循环
来源：http://ih.shxzukj.cn

Py:   while i < 10: i += 1
来源：http://ly.521024.cn

PHP:  while ($i < 10) { $i++; }
来源：http://jh.shxzskj.cn

JS:   while (i < 10) { i++; }
来源：http://jd.521024.cn

TS:   while (i < 10) { i++; }
来源：http://cb.huanxung.cn

Java: while (i < 10) { i++; }
来源：http://tn.shtwfgs.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://qe.521024.cn

Ruby: while i < 10; i += 1; end
来源：http://jt.yuntaijiaju.cn

C#:   while (i < 10) { i++; }
来源：http://mg.szsharing.cn

[B08] do-while（至少执行一次）
来源：http://bo.shxzukj.cn

Py:   # 无 do-while：用 while True + break
来源：http://er.nicolike.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://qn.shxzskj.cn

JS:   do { i++; } while (i < 10);
来源：http://ey.szsharing.cn

TS:   do { i++; } while (i < 10);
来源：http://hk.jianghongdianzi.cn

Java: do { i++; } while (i < 10);
来源：http://qi.gzmigu.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://mb.gzmigu.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ag.hahajie.cn

C#:   do { i++; } while (i < 10);
来源：http://we.nicolike.cn

[B09] break 与 continue
来源：http://eo.huanxung.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://lh.yuntaijiaju.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://pw.szxytkj.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mr.huixinmuqiang.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://iw.colortex.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qq.lnxyls.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wc.9csxet.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://xr.newstarts.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rs.haigaiapp.cn

[B10] 遍历同时拿索引
来源：http://na.jianghongdianzi.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://kh.yuexingan06.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://bz.shxzskj.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ea.szsharing.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://to.bookmarksfly.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://tv.jianghongdianzi.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://he.panjiajie.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://fk.muxihuayi.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://bv.yuexingan06.cn

[B11] 生成数字序列 / 区间
来源：http://jg.bookmarksfly.cn

Py:   list(range(0, 10, 2))
来源：http://fv.szxytkj.cn

PHP:  range(0, 10, 2);
来源：http://vz.shxzskj.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wj.newstarts.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://bi.nszjky.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hv.huixiangedu.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hp.shxzskj.cn

Ruby: (0...10).step(2).to_a
来源：http://dv.muxihuayi.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ml.yuntaijiaju.cn

[B12] 跳出多层循环
来源：http://qe.asd995.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://tw.521024.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://uu.nicolike.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://pb.huanxung.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://vb.yuexingan06.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ta.lnxyls.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://eo.yuntaijiaju.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://eu.asd995.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ge.muxihuayi.cn

[B13] 判断是否为数字
来源：http://jr.asd995.cn

Py:   isinstance(x, (int, float))
来源：http://qx.lnxyls.cn

PHP:  is_numeric($x)
来源：http://tn.gzmigu.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://lo.nszjky.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://fr.newstarts.cn

Java: x instanceof Number
来源：http://bh.chemitech.net.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://pp.asd995.cn

Ruby: x.is_a?(Numeric)
来源：http://mc.panjiajie.cn

C#:   x is int or double or decimal
来源：http://ew.bjjhwx.cn

[B14] 判断值是否在集合内
来源：http://th.shtwfgs.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://zk.panjiajie.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wv.colortex.cn

JS:   [1, 2, 3].includes(x)
来源：http://hv.asd995.cn

TS:   [1, 2, 3].includes(x)
来源：http://il.yuntaijiaju.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://id.shxzskj.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://nf.szsharing.cn

Ruby: [1, 2, 3].include?(x)
来源：http://sp.shxzukj.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://cn.521024.cn

[B15] 布尔运算与取反
来源：http://da.nszjky.cn

Py:   a and b or not c
来源：http://so.szsharing.cn

PHP:  $a && $b || !$c
来源：http://pe.gzmigu.cn

JS:   a && b || !c
来源：http://wl.huanxung.cn

TS:   a && b || !c
来源：http://oo.huixinmuqiang.cn

Java: a && b || !c
来源：http://gy.hahajie.cn

Go:   a && b || !c
来源：http://zy.haigaiapp.cn

Ruby: a && b || !c
来源：http://tj.shtwfgs.cn

C#:   a && b || !c
来源：http://ms.huixiangedu.cn

[B16] 卫语句：不满足条件提前返回
来源：http://jd.shxzskj.cn

Py:   if not data: return
来源：http://tc.szxytkj.cn

PHP:  if (!$data) { return; }
来源：http://go.shtwfgs.cn

JS:   if (!data) return;
来源：http://vd.huanxung.cn

TS:   if (!data) return;
来源：http://wi.lnxyls.cn

Java: if (data == null) return;
来源：http://uu.gzmigu.cn

Go:   if data == nil { return }
来源：http://xb.shtwfgs.cn

Ruby: return if data.nil?
来源：http://th.shxzukj.cn

C#:   if (data == null) return;
来源：http://rt.chemitech.net.cn

================================================================================
来源：http://il.chemitech.net.cn

C. 函数与作用域
来源：http://ag.nicolike.cn

================================================================================
来源：http://yl.hahajie.cn

[C01] 定义函数
来源：http://vz.nszjky.cn

Py:   def add(a, b): return a + b
来源：http://wp.colortex.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://gf.szsharing.cn

JS:   function add(a, b) { return a + b; }
来源：http://yd.jianghongdianzi.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://yh.gzmigu.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://me.newstarts.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ny.hahajie.cn

Ruby: def add(a, b); a + b; end
来源：http://tu.bjjhwx.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://zo.hnjuh.cn

[C02] 默认参数
来源：http://nj.jianghongdianzi.cn

Py:   def greet(name="World"): return name
来源：http://yh.521024.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://qq.gzmigu.cn

JS:   function greet(name = "World") { return name; }
来源：http://fs.521024.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://mj.jctech888.com.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://cl.bookmarksfly.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://kj.yuexingan06.cn

Ruby: def greet(name = "World") = name
来源：http://sc.yuntaijiaju.cn

C#:   string Greet(string name = "World") => name;
来源：http://wk.gzmigu.cn

[C03] 可变参数
来源：http://au.szxytkj.cn

Py:   def total(*args): return sum(args)
来源：http://ty.colortex.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://rf.huixiangedu.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://pg.shxzskj.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://pc.huixiangedu.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://sp.nszjky.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://jx.jctech888.com.cn

Ruby: def total(*nums); nums.sum; end
来源：http://xw.huanxung.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://zw.colortex.cn

[C04] 命名参数 / 关键字参数
来源：http://pj.shxzukj.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://zx.huixiangedu.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://bk.haigaiapp.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://nn.nszjky.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://al.huixinmuqiang.cn

Java: // 无：用 Builder 模式或 record
来源：http://rh.newstarts.cn

Go:   // 无：用配置结构体参数
来源：http://xp.shxzskj.cn

Ruby: f(a: 1, b: 2)
来源：http://tn.jctech888.com.cn

C#:   f(a: 1, b: 2)
来源：http://as.wgjwhj.cn

[C05] 返回多个值
来源：http://qi.szxytkj.cn

Py:   return a, b
来源：http://bk.muxihuayi.cn

PHP:  return [$a, $b];
来源：http://pv.gzmigu.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://xh.hnjuh.cn

TS:   return { a, b };
来源：http://ne.bookmarksfly.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://qf.shxzskj.cn

Go:   return a, b
来源：http://fg.shtwfgs.cn

Ruby: return a, b
来源：http://rj.szxytkj.cn

C#:   return (a, b);              // ValueTuple
来源：http://vc.szsharing.cn

[C06] 匿名函数 / lambda
来源：http://xb.bookmarksfly.cn

Py:   square = lambda x: x * x
来源：http://ig.9csxet.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://kj.panjiajie.cn

JS:   const square = x => x * x;
来源：http://hc.hnjuh.cn

TS:   const square = (x: number): number => x * x;
来源：http://lo.shtwfgs.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://bt.szsharing.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ga.shtwfgs.cn

Ruby: square = ->(x) { x * x }
来源：http://hf.9csxet.cn

C#:   Func<int, int> square = x => x * x;
来源：http://fl.muxihuayi.cn

[C07] 把函数作为参数传入
来源：http://pp.huanxung.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://tp.wgjwhj.cn

PHP:  array_map("strtoupper", $arr);
来源：http://xn.colortex.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://if.gzmigu.cn

TS:   arr.map(String)
来源：http://ay.shtwfgs.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ef.lnxyls.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://bm.hahajie.cn

Ruby: arr.map(&:upcase)
来源：http://jf.nicolike.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://se.haigaiapp.cn

[C08] 闭包
来源：http://xn.hnjuh.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ch.hnjuh.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://li.shtwfgs.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ju.panjiajie.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://zq.hahajie.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://iu.yuexingan06.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://cg.asd995.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://px.huanxung.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://od.huixiangedu.cn

[C09] 递归
来源：http://pq.huixiangedu.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://os.chemitech.net.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://tp.bjjhwx.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://zt.bookmarksfly.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://yx.521024.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wb.9csxet.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wj.bjjhwx.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ob.nicolike.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://az.yuexingan06.cn

[C10] 变量作用域
来源：http://iw.lnxyls.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://zx.chemitech.net.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://jm.huixinmuqiang.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wi.huanxung.cn

TS:   同 JS
来源：http://rt.huanxung.cn

Java: 方法内为块级作用域
来源：http://ws.shtwfgs.cn

Go:   花括号块级作用域
来源：http://nx.huixiangedu.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://pp.nszjky.cn

C#:   块级作用域
来源：http://hu.jianghongdianzi.cn

[C11] 模块导入与导出
来源：http://xp.huixiangedu.cn

Py:   from module import func
来源：http://sy.chemitech.net.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://cz.shxzskj.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://tx.muxihuayi.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://sy.521024.cn

Java: import java.util.List;
来源：http://jf.jianghongdianzi.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://dm.newstarts.cn

Ruby: require "json"; require_relative "./util"
来源：http://pd.szsharing.cn

C#:   using System.Text;
来源：http://ij.shtwfgs.cn

[C12] 立即执行函数 IIFE
来源：http://jw.shxzskj.cn

Py:   (lambda: print("run"))()
来源：http://ap.shxzskj.cn

PHP:  (function () { echo "run"; })();
来源：http://ww.521024.cn

JS:   (() => { console.log("run"); })();
来源：http://md.jctech888.com.cn

TS:   (() => { console.log("run"); })();
来源：http://wg.shxzskj.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://yd.gzmigu.cn

Go:   func() { fmt.Println("run") }()
来源：http://yl.asd995.cn

Ruby: -> { puts "run" }.call
来源：http://ku.bjjhwx.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ga.bjjhwx.cn

[C13] 类型声明 / 类型注解
来源：http://mg.yuntaijiaju.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hm.hahajie.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://jt.nicolike.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://sb.huixiangedu.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ta.panjiajie.cn

Java: int add(int a, int b) { return a + b; }
来源：http://cb.colortex.cn

Go:   func add(a, b int) int
来源：http://go.jianghongdianzi.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://rv.bjjhwx.cn

C#:   int Add(int a, int b) => a + b;
来源：http://zz.jianghongdianzi.cn

[C14] 泛型函数
来源：http://zz.jianghongdianzi.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://fi.lnxyls.cn

PHP:  // 无泛型
来源：http://hn.jianghongdianzi.cn

JS:   // 无泛型
来源：http://wa.shxzukj.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://yk.chemitech.net.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://rw.521024.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://qq.yuntaijiaju.cn

Ruby: # 无泛型
来源：http://et.shxzskj.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://lc.shxzukj.cn

[C15] 解构 / 展开参数
来源：http://ah.wgjwhj.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://gx.shxzskj.cn

PHP:  [$a, $b] = $pair;
来源：http://ld.bookmarksfly.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://uh.szxytkj.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mv.jianghongdianzi.cn

Java: // 无解构
来源：http://rz.yuntaijiaju.cn

Go:   // 无解构
来源：http://tr.huixinmuqiang.cn

Ruby: a, b = pair
来源：http://ag.shxzukj.cn

C#:   var (a, b) = pair;
来源：http://vd.lnxyls.cn

[C16] 函数 / 方法重载
来源：http://qv.newstarts.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://sj.colortex.cn

PHP:  // 无重载
来源：http://ik.bjjhwx.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://if.jctech888.com.cn

TS:   // 用联合类型或重载签名声明
来源：http://lb.huixiangedu.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://hn.jianghongdianzi.cn

Go:   // 无重载：用不同函数名
来源：http://wd.jctech888.com.cn

Ruby: # 无重载：靠动态参数
来源：http://va.shxzukj.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://gw.asd995.cn

================================================================================
来源：http://td.hahajie.cn

D. 数组 / 列表 / 集合
来源：http://mu.lnxyls.cn

================================================================================
来源：http://mh.jctech888.com.cn

[D01] 创建数组 / 列表
来源：http://nl.wgjwhj.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://nw.nszjky.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wn.szsharing.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://pq.gzmigu.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ka.9csxet.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://fl.hnjuh.cn

Go:   arr := []int{1, 2, 3}
来源：http://ms.asd995.cn

Ruby: arr = [1, 2, 3]
来源：http://zv.szsharing.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://kd.shxzukj.cn

[D02] 追加元素到末尾
来源：http://ul.wgjwhj.cn


<!-- 参考信息 -->