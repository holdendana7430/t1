代发 wailian999

[B01] 条件判断 if / else
来源：http://eh.szxytkj.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://tl.bjjhwx.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://mq.shxzskj.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://vi.haigaiapp.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://jr.bjjhwx.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://yk.colortex.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://jy.shxzskj.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://mt.panjiajie.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://wm.haigaiapp.cn

[B02] 多分支 else if / elif
来源：http://lu.bjjhwx.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://xc.shxzskj.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://oq.szsharing.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wq.muxihuayi.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wx.szsharing.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fc.shxzukj.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://bg.hnjuh.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://xz.gzmigu.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qp.haigaiapp.cn

[B03] switch / match / case
来源：http://lt.newstarts.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://qz.panjiajie.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://gr.panjiajie.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://fo.gzmigu.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://nk.bjjhwx.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://yp.shxzukj.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://au.shxzukj.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://qq.chemitech.net.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://on.hahajie.cn

[B04] for 计数循环
来源：http://zv.wgjwhj.cn

Py:   for i in range(10): print(i)
来源：http://zx.jctech888.com.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://by.huixiangedu.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ws.9csxet.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://le.gzmigu.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://kp.huixiangedu.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://vg.bookmarksfly.cn

Ruby: 10.times { |i| puts i }
来源：http://vj.nszjky.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://no.jianghongdianzi.cn

[B05] 遍历数组 / 列表
来源：http://np.chemitech.net.cn

Py:   for item in arr: print(item)
来源：http://ut.gzmigu.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://uf.nicolike.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://go.huixinmuqiang.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ur.shxzskj.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://yp.gzmigu.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://qd.shxzskj.cn

Ruby: arr.each { |item| puts item }
来源：http://fd.huanxung.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://qc.szsharing.cn

[B06] 遍历字典 / 对象
来源：http://yw.yuntaijiaju.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://tz.asd995.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hb.bookmarksfly.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ds.9csxet.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://pu.hahajie.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hn.yuexingan06.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://uf.hahajie.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ti.wgjwhj.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://fu.hnjuh.cn

[B07] while 循环
来源：http://zs.521024.cn

Py:   while i < 10: i += 1
来源：http://yz.haigaiapp.cn

PHP:  while ($i < 10) { $i++; }
来源：http://af.shxzukj.cn

JS:   while (i < 10) { i++; }
来源：http://yz.muxihuayi.cn

TS:   while (i < 10) { i++; }
来源：http://zm.hahajie.cn

Java: while (i < 10) { i++; }
来源：http://zh.lnxyls.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://xi.shtwfgs.cn

Ruby: while i < 10; i += 1; end
来源：http://ds.yuntaijiaju.cn

C#:   while (i < 10) { i++; }
来源：http://qs.szsharing.cn

[B08] do-while（至少执行一次）
来源：http://vh.shtwfgs.cn

Py:   # 无 do-while：用 while True + break
来源：http://fj.jctech888.com.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://bi.shxzskj.cn

JS:   do { i++; } while (i < 10);
来源：http://jw.9csxet.cn

TS:   do { i++; } while (i < 10);
来源：http://mp.yuexingan06.cn

Java: do { i++; } while (i < 10);
来源：http://vf.521024.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://vb.shxzukj.cn

Ruby: begin; i += 1; end while i < 10
来源：http://xz.colortex.cn

C#:   do { i++; } while (i < 10);
来源：http://rs.haigaiapp.cn

[B09] break 与 continue
来源：http://ke.shxzskj.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://qf.lnxyls.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://sb.hnjuh.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cd.jctech888.com.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mp.shxzskj.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hx.lnxyls.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://nh.newstarts.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://sm.bjjhwx.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rv.yuntaijiaju.cn

[B10] 遍历同时拿索引
来源：http://or.gzmigu.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://pv.9csxet.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://qe.panjiajie.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://zx.lnxyls.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hn.huixiangedu.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://dd.colortex.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://pf.hnjuh.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ry.chemitech.net.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://cq.shtwfgs.cn

[B11] 生成数字序列 / 区间
来源：http://rl.nicolike.cn

Py:   list(range(0, 10, 2))
来源：http://su.yuntaijiaju.cn

PHP:  range(0, 10, 2);
来源：http://uo.shxzskj.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://rt.huixinmuqiang.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://by.hnjuh.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://xj.gzmigu.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://il.szxytkj.cn

Ruby: (0...10).step(2).to_a
来源：http://nv.szsharing.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://xn.szsharing.cn

[B12] 跳出多层循环
来源：http://vr.521024.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ra.huanxung.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://fa.yuntaijiaju.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ng.9csxet.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://vb.gzmigu.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://vd.jctech888.com.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://sm.9csxet.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ch.hnjuh.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hb.szsharing.cn

[B13] 判断是否为数字
来源：http://yq.bookmarksfly.cn

Py:   isinstance(x, (int, float))
来源：http://fq.szxytkj.cn

PHP:  is_numeric($x)
来源：http://ye.newstarts.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://gn.panjiajie.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://vq.huanxung.cn

Java: x instanceof Number
来源：http://oz.szsharing.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://km.szsharing.cn

Ruby: x.is_a?(Numeric)
来源：http://ir.bjjhwx.cn

C#:   x is int or double or decimal
来源：http://gp.colortex.cn

[B14] 判断值是否在集合内
来源：http://ju.bookmarksfly.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hi.hnjuh.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ie.hnjuh.cn

JS:   [1, 2, 3].includes(x)
来源：http://yf.shxzskj.cn

TS:   [1, 2, 3].includes(x)
来源：http://bl.yuntaijiaju.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://oa.huanxung.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://sc.bjjhwx.cn

Ruby: [1, 2, 3].include?(x)
来源：http://jz.hahajie.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://zb.wgjwhj.cn

[B15] 布尔运算与取反
来源：http://vy.bjjhwx.cn

Py:   a and b or not c
来源：http://ft.jctech888.com.cn

PHP:  $a && $b || !$c
来源：http://df.colortex.cn

JS:   a && b || !c
来源：http://fe.newstarts.cn

TS:   a && b || !c
来源：http://jp.huixiangedu.cn

Java: a && b || !c
来源：http://rd.shtwfgs.cn

Go:   a && b || !c
来源：http://pe.shxzukj.cn

Ruby: a && b || !c
来源：http://kt.szxytkj.cn

C#:   a && b || !c
来源：http://bx.nszjky.cn

[B16] 卫语句：不满足条件提前返回
来源：http://xr.muxihuayi.cn

Py:   if not data: return
来源：http://ax.bookmarksfly.cn

PHP:  if (!$data) { return; }
来源：http://ow.huixinmuqiang.cn

JS:   if (!data) return;
来源：http://nv.nszjky.cn

TS:   if (!data) return;
来源：http://hn.gzmigu.cn

Java: if (data == null) return;
来源：http://wx.shtwfgs.cn

Go:   if data == nil { return }
来源：http://ng.yuexingan06.cn

Ruby: return if data.nil?
来源：http://bd.lnxyls.cn

C#:   if (data == null) return;
来源：http://vf.lnxyls.cn

================================================================================
来源：http://kq.szxytkj.cn

C. 函数与作用域
来源：http://gt.haigaiapp.cn

================================================================================
来源：http://gv.lnxyls.cn

[C01] 定义函数
来源：http://bx.bjjhwx.cn

Py:   def add(a, b): return a + b
来源：http://yh.panjiajie.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://dp.newstarts.cn

JS:   function add(a, b) { return a + b; }
来源：http://vi.jctech888.com.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://do.521024.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://sv.jianghongdianzi.cn

Go:   func add(a, b int) int { return a + b }
来源：http://kd.lnxyls.cn

Ruby: def add(a, b); a + b; end
来源：http://nd.jctech888.com.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hk.shxzukj.cn

[C02] 默认参数
来源：http://ul.yuexingan06.cn

Py:   def greet(name="World"): return name
来源：http://sp.hahajie.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://gp.haigaiapp.cn

JS:   function greet(name = "World") { return name; }
来源：http://jw.chemitech.net.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://xf.huanxung.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://cm.szxytkj.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://dr.panjiajie.cn

Ruby: def greet(name = "World") = name
来源：http://kk.colortex.cn

C#:   string Greet(string name = "World") => name;
来源：http://pl.wgjwhj.cn

[C03] 可变参数
来源：http://hi.shxzukj.cn

Py:   def total(*args): return sum(args)
来源：http://il.wgjwhj.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://xi.haigaiapp.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mj.shtwfgs.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://xx.huixinmuqiang.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ff.jianghongdianzi.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://jm.bjjhwx.cn

Ruby: def total(*nums); nums.sum; end
来源：http://io.newstarts.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://bi.hahajie.cn

[C04] 命名参数 / 关键字参数
来源：http://qc.muxihuayi.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://yi.muxihuayi.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://dc.nicolike.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mj.colortex.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://nj.nszjky.cn

Java: // 无：用 Builder 模式或 record
来源：http://zd.huixiangedu.cn

Go:   // 无：用配置结构体参数
来源：http://ie.yuntaijiaju.cn

Ruby: f(a: 1, b: 2)
来源：http://gu.colortex.cn

C#:   f(a: 1, b: 2)
来源：http://nn.jianghongdianzi.cn

[C05] 返回多个值
来源：http://wb.newstarts.cn

Py:   return a, b
来源：http://aj.hahajie.cn

PHP:  return [$a, $b];
来源：http://ik.szxytkj.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://jz.shxzskj.cn

TS:   return { a, b };
来源：http://oh.shxzukj.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ju.9csxet.cn

Go:   return a, b
来源：http://af.huanxung.cn

Ruby: return a, b
来源：http://dv.jctech888.com.cn

C#:   return (a, b);              // ValueTuple
来源：http://dy.szsharing.cn

[C06] 匿名函数 / lambda
来源：http://cp.colortex.cn

Py:   square = lambda x: x * x
来源：http://mx.szxytkj.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ux.colortex.cn

JS:   const square = x => x * x;
来源：http://fu.jianghongdianzi.cn

TS:   const square = (x: number): number => x * x;
来源：http://nq.shxzukj.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ba.lnxyls.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ha.521024.cn

Ruby: square = ->(x) { x * x }
来源：http://fe.yuntaijiaju.cn

C#:   Func<int, int> square = x => x * x;
来源：http://wv.yuntaijiaju.cn

[C07] 把函数作为参数传入
来源：http://cf.hahajie.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://gp.hahajie.cn

PHP:  array_map("strtoupper", $arr);
来源：http://gk.asd995.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://sa.nicolike.cn

TS:   arr.map(String)
来源：http://uc.shxzukj.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ic.huanxung.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ex.lnxyls.cn

Ruby: arr.map(&:upcase)
来源：http://fe.hnjuh.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://yk.bookmarksfly.cn

[C08] 闭包
来源：http://be.nszjky.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://sn.nicolike.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ub.muxihuayi.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://xp.bookmarksfly.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ee.gzmigu.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://em.wgjwhj.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wd.yuexingan06.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ul.huanxung.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mw.hahajie.cn

[C09] 递归
来源：http://xi.shtwfgs.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hr.colortex.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://qj.yuntaijiaju.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hv.lnxyls.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qv.hnjuh.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://gg.nicolike.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ml.wgjwhj.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://qd.lnxyls.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://pe.9csxet.cn

[C10] 变量作用域
来源：http://gw.shxzskj.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ph.bookmarksfly.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://qs.szsharing.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://iv.asd995.cn

TS:   同 JS
来源：http://xk.shtwfgs.cn

Java: 方法内为块级作用域
来源：http://jj.9csxet.cn

Go:   花括号块级作用域
来源：http://qk.shxzskj.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://fy.chemitech.net.cn

C#:   块级作用域
来源：http://fo.9csxet.cn

[C11] 模块导入与导出
来源：http://hc.nicolike.cn

Py:   from module import func
来源：http://no.panjiajie.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://mk.hnjuh.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://oo.yuexingan06.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://pa.jctech888.com.cn

Java: import java.util.List;
来源：http://en.chemitech.net.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://bn.9csxet.cn

Ruby: require "json"; require_relative "./util"
来源：http://qj.huixinmuqiang.cn

C#:   using System.Text;
来源：http://hi.colortex.cn

[C12] 立即执行函数 IIFE
来源：http://dg.shxzukj.cn

Py:   (lambda: print("run"))()
来源：http://pq.huixinmuqiang.cn

PHP:  (function () { echo "run"; })();
来源：http://mx.9csxet.cn

JS:   (() => { console.log("run"); })();
来源：http://fr.huixiangedu.cn

TS:   (() => { console.log("run"); })();
来源：http://pw.bookmarksfly.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://yt.yuexingan06.cn

Go:   func() { fmt.Println("run") }()
来源：http://df.bjjhwx.cn

Ruby: -> { puts "run" }.call
来源：http://xu.521024.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ri.hnjuh.cn

[C13] 类型声明 / 类型注解
来源：http://fg.yuexingan06.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://di.huixiangedu.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://gx.huanxung.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ju.haigaiapp.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ul.haigaiapp.cn

Java: int add(int a, int b) { return a + b; }
来源：http://ff.shtwfgs.cn

Go:   func add(a, b int) int
来源：http://un.huixiangedu.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://gv.bookmarksfly.cn

C#:   int Add(int a, int b) => a + b;
来源：http://vl.szsharing.cn

[C14] 泛型函数
来源：http://ks.colortex.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ed.nszjky.cn

PHP:  // 无泛型
来源：http://rs.shxzskj.cn

JS:   // 无泛型
来源：http://xn.jctech888.com.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://uf.bjjhwx.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://dz.shxzskj.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://lj.jianghongdianzi.cn

Ruby: # 无泛型
来源：http://he.shtwfgs.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://nh.9csxet.cn

[C15] 解构 / 展开参数
来源：http://jl.yuexingan06.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://av.9csxet.cn

PHP:  [$a, $b] = $pair;
来源：http://nd.bookmarksfly.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ml.huixiangedu.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wn.huixinmuqiang.cn

Java: // 无解构
来源：http://ai.hahajie.cn

Go:   // 无解构
来源：http://yl.yuntaijiaju.cn

Ruby: a, b = pair
来源：http://rv.szxytkj.cn

C#:   var (a, b) = pair;
来源：http://iz.huanxung.cn

[C16] 函数 / 方法重载
来源：http://lx.521024.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://pn.bookmarksfly.cn

PHP:  // 无重载
来源：http://aq.jianghongdianzi.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://hl.shxzskj.cn

TS:   // 用联合类型或重载签名声明
来源：http://sn.gzmigu.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://ys.hahajie.cn

Go:   // 无重载：用不同函数名
来源：http://yk.gzmigu.cn

Ruby: # 无重载：靠动态参数
来源：http://ne.jctech888.com.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ja.chemitech.net.cn

================================================================================
来源：http://bq.shxzukj.cn

D. 数组 / 列表 / 集合
来源：http://ic.9csxet.cn

================================================================================
来源：http://ks.lnxyls.cn

[D01] 创建数组 / 列表
来源：http://yq.wgjwhj.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ot.jctech888.com.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ly.nicolike.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://du.shtwfgs.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://cr.shxzskj.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://co.nszjky.cn


<!-- 参考信息 -->