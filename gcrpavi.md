代发 wailian999

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ng.nszjky.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ys.lnxyls.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://se.lnxyls.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://lq.panjiajie.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ji.chemitech.net.cn

[B02] 多分支 else if / elif
来源：http://cv.shxzskj.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://bp.wgjwhj.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://qq.huixiangedu.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ve.colortex.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://du.lnxyls.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pq.newstarts.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://fc.9csxet.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://mc.hahajie.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ti.newstarts.cn

[B03] switch / match / case
来源：http://vo.yuntaijiaju.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://kw.chemitech.net.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ml.huanxung.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://nn.yuntaijiaju.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.wgjwhj.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://nt.jctech888.com.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hy.huixinmuqiang.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://qz.panjiajie.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://xf.9csxet.cn

[B04] for 计数循环
来源：http://jm.szxytkj.cn

Py:   for i in range(10): print(i)
来源：http://sr.huixinmuqiang.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ps.asd995.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ds.nicolike.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://sd.chemitech.net.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://vd.huixinmuqiang.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://is.colortex.cn

Ruby: 10.times { |i| puts i }
来源：http://in.jianghongdianzi.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ix.bjjhwx.cn

[B05] 遍历数组 / 列表
来源：http://he.wgjwhj.cn

Py:   for item in arr: print(item)
来源：http://dv.hahajie.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ux.chemitech.net.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://vc.szsharing.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://zf.gzmigu.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://kk.wgjwhj.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://dk.9csxet.cn

Ruby: arr.each { |item| puts item }
来源：http://uh.szsharing.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://jz.szxytkj.cn

[B06] 遍历字典 / 对象
来源：http://mj.huanxung.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://dk.asd995.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://lw.hahajie.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://fk.huanxung.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ik.jianghongdianzi.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://zw.9csxet.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://tr.hnjuh.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://cu.521024.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ms.hahajie.cn

[B07] while 循环
来源：http://wi.hahajie.cn

Py:   while i < 10: i += 1
来源：http://yb.yuntaijiaju.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ly.lnxyls.cn

JS:   while (i < 10) { i++; }
来源：http://bx.yuexingan06.cn

TS:   while (i < 10) { i++; }
来源：http://jd.szsharing.cn

Java: while (i < 10) { i++; }
来源：http://ll.gzmigu.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://yw.muxihuayi.cn

Ruby: while i < 10; i += 1; end
来源：http://dj.szsharing.cn

C#:   while (i < 10) { i++; }
来源：http://ax.szxytkj.cn

[B08] do-while（至少执行一次）
来源：http://dj.szsharing.cn

Py:   # 无 do-while：用 while True + break
来源：http://ym.hahajie.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://lr.shxzukj.cn

JS:   do { i++; } while (i < 10);
来源：http://nv.szxytkj.cn

TS:   do { i++; } while (i < 10);
来源：http://pe.muxihuayi.cn

Java: do { i++; } while (i < 10);
来源：http://kn.bjjhwx.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://ea.bookmarksfly.cn

Ruby: begin; i += 1; end while i < 10
来源：http://qz.jctech888.com.cn

C#:   do { i++; } while (i < 10);
来源：http://mv.newstarts.cn

[B09] break 与 continue
来源：http://nk.shxzukj.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://uy.yuexingan06.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://if.yuntaijiaju.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fk.hahajie.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://iq.shxzukj.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://eu.szsharing.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://gn.panjiajie.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://rs.gzmigu.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tx.szxytkj.cn

[B10] 遍历同时拿索引
来源：http://xa.asd995.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://kj.szsharing.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mb.jianghongdianzi.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ib.panjiajie.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://bs.wgjwhj.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://gp.521024.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://nm.huanxung.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ae.yuexingan06.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://kj.haigaiapp.cn

[B11] 生成数字序列 / 区间
来源：http://no.jianghongdianzi.cn

Py:   list(range(0, 10, 2))
来源：http://jn.shxzskj.cn

PHP:  range(0, 10, 2);
来源：http://ev.asd995.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://nf.nszjky.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://iu.wgjwhj.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://od.yuntaijiaju.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://il.newstarts.cn

Ruby: (0...10).step(2).to_a
来源：http://yd.shxzukj.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://kq.huixinmuqiang.cn

[B12] 跳出多层循环
来源：http://lu.521024.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://nh.hahajie.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ej.colortex.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://eb.haigaiapp.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ne.jctech888.com.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://rb.asd995.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ec.yuexingan06.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://gb.hnjuh.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://yi.lnxyls.cn

[B13] 判断是否为数字
来源：http://iq.newstarts.cn

Py:   isinstance(x, (int, float))
来源：http://ma.bjjhwx.cn

PHP:  is_numeric($x)
来源：http://su.hahajie.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hg.huixiangedu.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://oh.jctech888.com.cn

Java: x instanceof Number
来源：http://se.haigaiapp.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://bg.yuntaijiaju.cn

Ruby: x.is_a?(Numeric)
来源：http://bh.wgjwhj.cn

C#:   x is int or double or decimal
来源：http://wy.newstarts.cn

[B14] 判断值是否在集合内
来源：http://ci.panjiajie.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://nm.szsharing.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://dq.szsharing.cn

JS:   [1, 2, 3].includes(x)
来源：http://cv.newstarts.cn

TS:   [1, 2, 3].includes(x)
来源：http://ip.panjiajie.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://hx.jctech888.com.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://yx.lnxyls.cn

Ruby: [1, 2, 3].include?(x)
来源：http://id.shtwfgs.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://yh.jctech888.com.cn

[B15] 布尔运算与取反
来源：http://pd.muxihuayi.cn

Py:   a and b or not c
来源：http://si.yuntaijiaju.cn

PHP:  $a && $b || !$c
来源：http://yl.szsharing.cn

JS:   a && b || !c
来源：http://tj.nszjky.cn

TS:   a && b || !c
来源：http://jm.haigaiapp.cn

Java: a && b || !c
来源：http://sc.bookmarksfly.cn

Go:   a && b || !c
来源：http://fk.gzmigu.cn

Ruby: a && b || !c
来源：http://hk.newstarts.cn

C#:   a && b || !c
来源：http://hi.szxytkj.cn

[B16] 卫语句：不满足条件提前返回
来源：http://jh.newstarts.cn

Py:   if not data: return
来源：http://jv.colortex.cn

PHP:  if (!$data) { return; }
来源：http://ae.hahajie.cn

JS:   if (!data) return;
来源：http://sd.jianghongdianzi.cn

TS:   if (!data) return;
来源：http://kb.nszjky.cn

Java: if (data == null) return;
来源：http://bs.huixiangedu.cn

Go:   if data == nil { return }
来源：http://wm.newstarts.cn

Ruby: return if data.nil?
来源：http://hj.asd995.cn

C#:   if (data == null) return;
来源：http://vd.nszjky.cn

================================================================================
来源：http://iw.shxzukj.cn

C. 函数与作用域
来源：http://wa.muxihuayi.cn

================================================================================
来源：http://yv.jianghongdianzi.cn

[C01] 定义函数
来源：http://kc.gzmigu.cn

Py:   def add(a, b): return a + b
来源：http://ij.bookmarksfly.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ep.shxzukj.cn

JS:   function add(a, b) { return a + b; }
来源：http://xr.521024.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://sr.nicolike.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ib.colortex.cn

Go:   func add(a, b int) int { return a + b }
来源：http://oq.jianghongdianzi.cn

Ruby: def add(a, b); a + b; end
来源：http://hk.chemitech.net.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://uy.nicolike.cn

[C02] 默认参数
来源：http://tq.haigaiapp.cn

Py:   def greet(name="World"): return name
来源：http://oc.szsharing.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://dy.jianghongdianzi.cn

JS:   function greet(name = "World") { return name; }
来源：http://hi.lnxyls.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://zf.huixinmuqiang.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://uy.huixiangedu.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hp.bookmarksfly.cn

Ruby: def greet(name = "World") = name
来源：http://nf.bjjhwx.cn

C#:   string Greet(string name = "World") => name;
来源：http://ls.9csxet.cn

[C03] 可变参数
来源：http://va.newstarts.cn

Py:   def total(*args): return sum(args)
来源：http://eq.nszjky.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://xx.521024.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ag.szsharing.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://sn.9csxet.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ms.asd995.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://me.shtwfgs.cn

Ruby: def total(*nums); nums.sum; end
来源：http://qv.haigaiapp.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://iw.asd995.cn

[C04] 命名参数 / 关键字参数
来源：http://wm.521024.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mk.shxzukj.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hf.colortex.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mj.huixinmuqiang.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://oe.huixiangedu.cn

Java: // 无：用 Builder 模式或 record
来源：http://kx.colortex.cn

Go:   // 无：用配置结构体参数
来源：http://lt.szxytkj.cn

Ruby: f(a: 1, b: 2)
来源：http://pu.muxihuayi.cn

C#:   f(a: 1, b: 2)
来源：http://oe.chemitech.net.cn

[C05] 返回多个值
来源：http://jd.huixinmuqiang.cn

Py:   return a, b
来源：http://kp.wgjwhj.cn

PHP:  return [$a, $b];
来源：http://pp.yuexingan06.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://bq.jianghongdianzi.cn

TS:   return { a, b };
来源：http://ye.huixinmuqiang.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://eu.szsharing.cn

Go:   return a, b
来源：http://jb.shxzukj.cn

Ruby: return a, b
来源：http://wn.huixinmuqiang.cn

C#:   return (a, b);              // ValueTuple
来源：http://fg.shxzskj.cn

[C06] 匿名函数 / lambda
来源：http://so.haigaiapp.cn

Py:   square = lambda x: x * x
来源：http://qg.newstarts.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://cz.bookmarksfly.cn

JS:   const square = x => x * x;
来源：http://ha.bjjhwx.cn

TS:   const square = (x: number): number => x * x;
来源：http://tf.newstarts.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wm.bjjhwx.cn

Go:   sq := func(x int) int { return x * x }
来源：http://lz.haigaiapp.cn

Ruby: square = ->(x) { x * x }
来源：http://zt.szxytkj.cn

C#:   Func<int, int> square = x => x * x;
来源：http://eh.bjjhwx.cn

[C07] 把函数作为参数传入
来源：http://cj.gzmigu.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ec.szxytkj.cn

PHP:  array_map("strtoupper", $arr);
来源：http://rq.nszjky.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://jt.huixiangedu.cn

TS:   arr.map(String)
来源：http://ci.jctech888.com.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://cc.muxihuayi.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://am.wgjwhj.cn

Ruby: arr.map(&:upcase)
来源：http://or.szxytkj.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ba.hnjuh.cn

[C08] 闭包
来源：http://zp.bookmarksfly.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ya.colortex.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ql.szxytkj.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ae.chemitech.net.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://oi.haigaiapp.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ri.hnjuh.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://kr.colortex.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ju.haigaiapp.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://uk.yuntaijiaju.cn

[C09] 递归
来源：http://jx.colortex.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://pk.newstarts.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://rl.yuntaijiaju.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://yr.bjjhwx.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://xu.hnjuh.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ma.yuexingan06.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://fz.bjjhwx.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ip.521024.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://rq.nicolike.cn

[C10] 变量作用域
来源：http://bm.hnjuh.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://qv.jctech888.com.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://rq.huanxung.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hr.9csxet.cn

TS:   同 JS
来源：http://eg.jctech888.com.cn

Java: 方法内为块级作用域
来源：http://rb.gzmigu.cn

Go:   花括号块级作用域
来源：http://nx.huixinmuqiang.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://zs.szxytkj.cn

C#:   块级作用域
来源：http://oq.hahajie.cn

[C11] 模块导入与导出
来源：http://vx.shtwfgs.cn

Py:   from module import func
来源：http://tr.shtwfgs.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://ug.wgjwhj.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://xh.bjjhwx.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ly.panjiajie.cn

Java: import java.util.List;
来源：http://gl.lnxyls.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://le.jianghongdianzi.cn

Ruby: require "json"; require_relative "./util"
来源：http://ru.nszjky.cn

C#:   using System.Text;
来源：http://tc.huanxung.cn

[C12] 立即执行函数 IIFE
来源：http://hi.muxihuayi.cn

Py:   (lambda: print("run"))()
来源：http://lk.shtwfgs.cn

PHP:  (function () { echo "run"; })();
来源：http://tr.shtwfgs.cn

JS:   (() => { console.log("run"); })();
来源：http://qg.szsharing.cn

TS:   (() => { console.log("run"); })();
来源：http://qp.yuntaijiaju.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://lw.bjjhwx.cn

Go:   func() { fmt.Println("run") }()
来源：http://oz.jctech888.com.cn

Ruby: -> { puts "run" }.call
来源：http://pb.chemitech.net.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://xm.hnjuh.cn

[C13] 类型声明 / 类型注解
来源：http://si.bookmarksfly.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://rp.nszjky.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://oy.bjjhwx.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://gc.colortex.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://rt.panjiajie.cn

Java: int add(int a, int b) { return a + b; }
来源：http://ft.szsharing.cn

Go:   func add(a, b int) int
来源：http://uf.szxytkj.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ac.lnxyls.cn

C#:   int Add(int a, int b) => a + b;
来源：http://yl.wgjwhj.cn

[C14] 泛型函数
来源：http://ez.panjiajie.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://rp.nicolike.cn

PHP:  // 无泛型
来源：http://pm.shtwfgs.cn

JS:   // 无泛型
来源：http://du.muxihuayi.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://jn.newstarts.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ia.lnxyls.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mu.haigaiapp.cn

Ruby: # 无泛型
来源：http://sn.shxzskj.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://si.521024.cn

[C15] 解构 / 展开参数
来源：http://nn.jctech888.com.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://aw.nszjky.cn

PHP:  [$a, $b] = $pair;
来源：http://rs.nszjky.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ua.jctech888.com.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://lr.nicolike.cn

Java: // 无解构
来源：http://mo.bjjhwx.cn

Go:   // 无解构
来源：http://zr.nicolike.cn

Ruby: a, b = pair
来源：http://bt.muxihuayi.cn

C#:   var (a, b) = pair;
来源：http://yz.szsharing.cn

[C16] 函数 / 方法重载
来源：http://tc.haigaiapp.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://rm.muxihuayi.cn

PHP:  // 无重载
来源：http://ng.newstarts.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://gq.szsharing.cn

TS:   // 用联合类型或重载签名声明
来源：http://dl.jianghongdianzi.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://zl.colortex.cn

Go:   // 无重载：用不同函数名
来源：http://xp.shtwfgs.cn

Ruby: # 无重载：靠动态参数
来源：http://xs.lnxyls.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://md.asd995.cn

================================================================================
来源：http://hk.nszjky.cn

D. 数组 / 列表 / 集合
来源：http://uv.gzmigu.cn

================================================================================
来源：http://bk.chemitech.net.cn

[D01] 创建数组 / 列表
来源：http://zz.shtwfgs.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://xq.hnjuh.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ud.newstarts.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mo.huixiangedu.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://nk.nicolike.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://gd.yuexingan06.cn

Go:   arr := []int{1, 2, 3}
来源：http://eq.panjiajie.cn

Ruby: arr = [1, 2, 3]
来源：http://lz.gzmigu.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://cl.yuexingan06.cn

[D02] 追加元素到末尾
来源：http://wx.chemitech.net.cn


<!-- 参考信息 -->