代发 wailian999

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://av.wgjwhj.cn

================================================================================
来源：http://mg.huanxung.cn

B. 流程控制
来源：http://gd.asd995.cn

================================================================================
来源：http://vd.shxzukj.cn

[B01] 条件判断 if / else
来源：http://ub.panjiajie.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://ww.asd995.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://xf.newstarts.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://iq.hnjuh.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://br.hnjuh.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://yc.muxihuayi.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://nr.hahajie.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ik.nicolike.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://fs.lnxyls.cn

[B02] 多分支 else if / elif
来源：http://ik.huixiangedu.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ep.asd995.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://rd.chemitech.net.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tc.szxytkj.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dg.szxytkj.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xc.colortex.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://lb.muxihuayi.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://cr.chemitech.net.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ru.shxzskj.cn

[B03] switch / match / case
来源：http://by.szxytkj.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://bp.jctech888.com.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://jb.huixiangedu.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ak.jctech888.com.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ku.newstarts.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://or.shxzukj.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://vy.bookmarksfly.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://qf.colortex.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://lq.shtwfgs.cn

[B04] for 计数循环
来源：http://xb.colortex.cn

Py:   for i in range(10): print(i)
来源：http://uw.bjjhwx.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://zv.yuntaijiaju.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ip.muxihuayi.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ga.jianghongdianzi.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://et.haigaiapp.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://qh.shxzukj.cn

Ruby: 10.times { |i| puts i }
来源：http://qu.nicolike.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://tv.huixinmuqiang.cn

[B05] 遍历数组 / 列表
来源：http://mi.lnxyls.cn

Py:   for item in arr: print(item)
来源：http://cq.shtwfgs.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://fn.jctech888.com.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://oj.jianghongdianzi.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://hi.shtwfgs.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://tp.shtwfgs.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://qj.shxzskj.cn

Ruby: arr.each { |item| puts item }
来源：http://dd.521024.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://aq.chemitech.net.cn

[B06] 遍历字典 / 对象
来源：http://my.jianghongdianzi.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ss.newstarts.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://fk.yuexingan06.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wm.9csxet.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ux.wgjwhj.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://lg.bookmarksfly.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://fs.muxihuayi.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://kk.nszjky.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://es.asd995.cn

[B07] while 循环
来源：http://sm.shxzskj.cn

Py:   while i < 10: i += 1
来源：http://qf.lnxyls.cn

PHP:  while ($i < 10) { $i++; }
来源：http://jc.jctech888.com.cn

JS:   while (i < 10) { i++; }
来源：http://fu.hnjuh.cn

TS:   while (i < 10) { i++; }
来源：http://zk.gzmigu.cn

Java: while (i < 10) { i++; }
来源：http://wa.hnjuh.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ri.nicolike.cn

Ruby: while i < 10; i += 1; end
来源：http://ja.jctech888.com.cn

C#:   while (i < 10) { i++; }
来源：http://tc.haigaiapp.cn

[B08] do-while（至少执行一次）
来源：http://im.bookmarksfly.cn

Py:   # 无 do-while：用 while True + break
来源：http://sa.huixinmuqiang.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://cn.wgjwhj.cn

JS:   do { i++; } while (i < 10);
来源：http://gv.nicolike.cn

TS:   do { i++; } while (i < 10);
来源：http://jx.bjjhwx.cn

Java: do { i++; } while (i < 10);
来源：http://jl.nicolike.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://hj.huixinmuqiang.cn

Ruby: begin; i += 1; end while i < 10
来源：http://zw.nszjky.cn

C#:   do { i++; } while (i < 10);
来源：http://qp.panjiajie.cn

[B09] break 与 continue
来源：http://vk.nicolike.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://nl.szsharing.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://na.nicolike.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tp.huixiangedu.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lo.shxzskj.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.lnxyls.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://cw.9csxet.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://bl.nicolike.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qj.shxzskj.cn

[B10] 遍历同时拿索引
来源：http://ro.panjiajie.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://xm.jianghongdianzi.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://md.huanxung.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://tp.jianghongdianzi.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://sp.shxzukj.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://xc.shtwfgs.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ff.haigaiapp.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ob.panjiajie.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wo.bookmarksfly.cn

[B11] 生成数字序列 / 区间
来源：http://lq.9csxet.cn

Py:   list(range(0, 10, 2))
来源：http://zp.yuntaijiaju.cn

PHP:  range(0, 10, 2);
来源：http://km.shtwfgs.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hd.asd995.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ba.muxihuayi.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://dc.nicolike.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hn.9csxet.cn

Ruby: (0...10).step(2).to_a
来源：http://az.huanxung.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://nc.9csxet.cn

[B12] 跳出多层循环
来源：http://nh.hnjuh.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://un.panjiajie.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://sj.newstarts.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://gg.jianghongdianzi.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ae.shxzukj.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://pe.shtwfgs.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://bo.asd995.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ig.shxzskj.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wl.lnxyls.cn

[B13] 判断是否为数字
来源：http://uv.huanxung.cn

Py:   isinstance(x, (int, float))
来源：http://rz.shxzukj.cn

PHP:  is_numeric($x)
来源：http://vn.shxzukj.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mz.shxzskj.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://gg.colortex.cn

Java: x instanceof Number
来源：http://hu.panjiajie.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mr.bookmarksfly.cn

Ruby: x.is_a?(Numeric)
来源：http://ci.shtwfgs.cn

C#:   x is int or double or decimal
来源：http://wn.wgjwhj.cn

[B14] 判断值是否在集合内
来源：http://at.521024.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://bc.hahajie.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://uz.lnxyls.cn

JS:   [1, 2, 3].includes(x)
来源：http://oo.panjiajie.cn

TS:   [1, 2, 3].includes(x)
来源：http://ks.jianghongdianzi.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ny.asd995.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mg.jctech888.com.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ds.bjjhwx.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://jf.nicolike.cn

[B15] 布尔运算与取反
来源：http://gc.newstarts.cn

Py:   a and b or not c
来源：http://wb.wgjwhj.cn

PHP:  $a && $b || !$c
来源：http://nn.hahajie.cn

JS:   a && b || !c
来源：http://cl.panjiajie.cn

TS:   a && b || !c
来源：http://au.asd995.cn

Java: a && b || !c
来源：http://ey.wgjwhj.cn

Go:   a && b || !c
来源：http://lv.bookmarksfly.cn

Ruby: a && b || !c
来源：http://ds.huixinmuqiang.cn

C#:   a && b || !c
来源：http://xc.gzmigu.cn

[B16] 卫语句：不满足条件提前返回
来源：http://hu.szsharing.cn

Py:   if not data: return
来源：http://pi.panjiajie.cn

PHP:  if (!$data) { return; }
来源：http://vv.huixiangedu.cn

JS:   if (!data) return;
来源：http://ei.huixinmuqiang.cn

TS:   if (!data) return;
来源：http://wz.521024.cn

Java: if (data == null) return;
来源：http://mg.nicolike.cn

Go:   if data == nil { return }
来源：http://ku.nszjky.cn

Ruby: return if data.nil?
来源：http://ev.colortex.cn

C#:   if (data == null) return;
来源：http://ub.hahajie.cn

================================================================================
来源：http://ua.jianghongdianzi.cn

C. 函数与作用域
来源：http://ru.shxzukj.cn

================================================================================
来源：http://au.bookmarksfly.cn

[C01] 定义函数
来源：http://wy.lnxyls.cn

Py:   def add(a, b): return a + b
来源：http://ny.szsharing.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xw.asd995.cn

JS:   function add(a, b) { return a + b; }
来源：http://ui.521024.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://lm.asd995.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ya.huixinmuqiang.cn

Go:   func add(a, b int) int { return a + b }
来源：http://dd.nszjky.cn

Ruby: def add(a, b); a + b; end
来源：http://qz.newstarts.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://bb.yuexingan06.cn

[C02] 默认参数
来源：http://kx.yuntaijiaju.cn

Py:   def greet(name="World"): return name
来源：http://ux.yuexingan06.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://wh.521024.cn

JS:   function greet(name = "World") { return name; }
来源：http://zk.shxzukj.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ce.shxzukj.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://rr.hahajie.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ev.bjjhwx.cn

Ruby: def greet(name = "World") = name
来源：http://yv.asd995.cn

C#:   string Greet(string name = "World") => name;
来源：http://cd.hahajie.cn

[C03] 可变参数
来源：http://cg.bjjhwx.cn

Py:   def total(*args): return sum(args)
来源：http://fc.shtwfgs.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://sw.9csxet.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://cu.bjjhwx.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ln.panjiajie.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://rn.hahajie.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://vn.muxihuayi.cn

Ruby: def total(*nums); nums.sum; end
来源：http://tv.lnxyls.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://at.hahajie.cn

[C04] 命名参数 / 关键字参数
来源：http://zv.huanxung.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ij.muxihuayi.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://rm.jctech888.com.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://xl.wgjwhj.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://xc.shtwfgs.cn

Java: // 无：用 Builder 模式或 record
来源：http://em.muxihuayi.cn

Go:   // 无：用配置结构体参数
来源：http://uo.chemitech.net.cn

Ruby: f(a: 1, b: 2)
来源：http://xg.hahajie.cn

C#:   f(a: 1, b: 2)
来源：http://hq.nicolike.cn

[C05] 返回多个值
来源：http://xb.jianghongdianzi.cn

Py:   return a, b
来源：http://hp.huixinmuqiang.cn

PHP:  return [$a, $b];
来源：http://rm.bookmarksfly.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://pb.jctech888.com.cn

TS:   return { a, b };
来源：http://iv.shtwfgs.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://dn.nszjky.cn

Go:   return a, b
来源：http://so.chemitech.net.cn

Ruby: return a, b
来源：http://br.yuexingan06.cn

C#:   return (a, b);              // ValueTuple
来源：http://lx.hahajie.cn

[C06] 匿名函数 / lambda
来源：http://ar.huanxung.cn

Py:   square = lambda x: x * x
来源：http://bk.shxzukj.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ij.nszjky.cn

JS:   const square = x => x * x;
来源：http://uc.haigaiapp.cn

TS:   const square = (x: number): number => x * x;
来源：http://lh.haigaiapp.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ps.nicolike.cn

Go:   sq := func(x int) int { return x * x }
来源：http://fe.panjiajie.cn

Ruby: square = ->(x) { x * x }
来源：http://cm.huixinmuqiang.cn

C#:   Func<int, int> square = x => x * x;
来源：http://mh.9csxet.cn

[C07] 把函数作为参数传入
来源：http://yv.asd995.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ll.muxihuayi.cn

PHP:  array_map("strtoupper", $arr);
来源：http://jr.szxytkj.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mg.hnjuh.cn

TS:   arr.map(String)
来源：http://cu.hnjuh.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://bs.yuntaijiaju.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wa.hnjuh.cn

Ruby: arr.map(&:upcase)
来源：http://gj.wgjwhj.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://nc.shxzskj.cn

[C08] 闭包
来源：http://ka.gzmigu.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ie.hnjuh.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ms.shtwfgs.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://xp.colortex.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://uk.szsharing.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://em.wgjwhj.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://bb.jctech888.com.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://pu.jctech888.com.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://zx.huanxung.cn

[C09] 递归
来源：http://ht.lnxyls.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ce.colortex.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://el.gzmigu.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://rf.shxzukj.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://oh.muxihuayi.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://xy.shtwfgs.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://bb.hnjuh.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://qr.wgjwhj.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://jp.panjiajie.cn

[C10] 变量作用域
来源：http://ih.nszjky.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://lq.shtwfgs.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://uh.shxzukj.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://tg.huanxung.cn

TS:   同 JS
来源：http://bw.shxzukj.cn

Java: 方法内为块级作用域
来源：http://ct.shtwfgs.cn

Go:   花括号块级作用域
来源：http://ep.huanxung.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://sh.hnjuh.cn

C#:   块级作用域
来源：http://ww.shxzskj.cn

[C11] 模块导入与导出
来源：http://jn.szsharing.cn

Py:   from module import func
来源：http://ve.bjjhwx.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://as.jctech888.com.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://xo.hnjuh.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://jx.wgjwhj.cn

Java: import java.util.List;
来源：http://pn.nicolike.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://qk.wgjwhj.cn

Ruby: require "json"; require_relative "./util"
来源：http://cz.9csxet.cn

C#:   using System.Text;
来源：http://zm.lnxyls.cn

[C12] 立即执行函数 IIFE
来源：http://kg.colortex.cn

Py:   (lambda: print("run"))()
来源：http://tl.chemitech.net.cn

PHP:  (function () { echo "run"; })();
来源：http://hd.jctech888.com.cn

JS:   (() => { console.log("run"); })();
来源：http://wz.bjjhwx.cn

TS:   (() => { console.log("run"); })();
来源：http://gs.muxihuayi.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://kr.gzmigu.cn

Go:   func() { fmt.Println("run") }()
来源：http://gn.panjiajie.cn

Ruby: -> { puts "run" }.call
来源：http://sz.hnjuh.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://dp.nicolike.cn

[C13] 类型声明 / 类型注解
来源：http://zy.bookmarksfly.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ga.yuexingan06.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://me.bjjhwx.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://re.9csxet.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wn.9csxet.cn

Java: int add(int a, int b) { return a + b; }
来源：http://rp.lnxyls.cn

Go:   func add(a, b int) int
来源：http://pq.shxzukj.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://nh.gzmigu.cn

C#:   int Add(int a, int b) => a + b;
来源：http://yx.hnjuh.cn

[C14] 泛型函数
来源：http://on.wgjwhj.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://nw.521024.cn

PHP:  // 无泛型
来源：http://ib.huixinmuqiang.cn

JS:   // 无泛型
来源：http://pk.jctech888.com.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://fp.hnjuh.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://gq.nszjky.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://us.panjiajie.cn

Ruby: # 无泛型
来源：http://gh.shxzukj.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://dq.yuexingan06.cn

[C15] 解构 / 展开参数
来源：http://jq.nicolike.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wn.hahajie.cn

PHP:  [$a, $b] = $pair;
来源：http://rk.gzmigu.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://yi.shxzskj.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://uu.huixinmuqiang.cn

Java: // 无解构
来源：http://yp.jctech888.com.cn

Go:   // 无解构
来源：http://bj.shxzukj.cn

Ruby: a, b = pair
来源：http://ji.hahajie.cn

C#:   var (a, b) = pair;
来源：http://lm.huanxung.cn

[C16] 函数 / 方法重载
来源：http://na.huixiangedu.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://lx.bookmarksfly.cn

PHP:  // 无重载
来源：http://qq.nicolike.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://nn.chemitech.net.cn

TS:   // 用联合类型或重载签名声明
来源：http://jz.wgjwhj.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://pq.jctech888.com.cn

Go:   // 无重载：用不同函数名
来源：http://un.yuexingan06.cn

Ruby: # 无重载：靠动态参数
来源：http://hf.9csxet.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://cv.shxzskj.cn

================================================================================
来源：http://vy.hahajie.cn

D. 数组 / 列表 / 集合
来源：http://gq.521024.cn

================================================================================
来源：http://zz.hahajie.cn

[D01] 创建数组 / 列表
来源：http://vg.chemitech.net.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://kp.panjiajie.cn


<!-- 参考信息 -->