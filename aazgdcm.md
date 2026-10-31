代发 wailian999

[B01] 条件判断 if / else
来源：http://cp.nicolike.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://go.asd995.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://qs.bjjhwx.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://pe.lnxyls.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://xf.yuexingan06.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://xz.newstarts.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://fh.jctech888.com.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://px.gzmigu.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://sy.colortex.cn

[B02] 多分支 else if / elif
来源：http://gt.wgjwhj.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://fn.hnjuh.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://tg.nicolike.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gi.jctech888.com.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ft.521024.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qa.chemitech.net.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://fv.colortex.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://rj.chemitech.net.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yv.nicolike.cn

[B03] switch / match / case
来源：http://ov.chemitech.net.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://pb.colortex.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://wo.panjiajie.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ab.yuexingan06.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://se.yuntaijiaju.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://iy.nicolike.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://er.newstarts.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://sx.shxzskj.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://qj.hnjuh.cn

[B04] for 计数循环
来源：http://bm.panjiajie.cn

Py:   for i in range(10): print(i)
来源：http://gb.shxzskj.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://bq.szxytkj.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ha.521024.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://fc.colortex.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ps.yuntaijiaju.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://kv.chemitech.net.cn

Ruby: 10.times { |i| puts i }
来源：http://wk.gzmigu.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://nd.chemitech.net.cn

[B05] 遍历数组 / 列表
来源：http://lu.jctech888.com.cn

Py:   for item in arr: print(item)
来源：http://wn.nszjky.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ug.hnjuh.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://sp.huanxung.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ig.huixinmuqiang.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://ra.panjiajie.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://fy.muxihuayi.cn

Ruby: arr.each { |item| puts item }
来源：http://fa.bookmarksfly.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ka.bjjhwx.cn

[B06] 遍历字典 / 对象
来源：http://kj.521024.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://en.asd995.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://kd.wgjwhj.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ot.newstarts.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://eq.colortex.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://mu.hahajie.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://qx.bookmarksfly.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://yi.panjiajie.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://fa.shtwfgs.cn

[B07] while 循环
来源：http://vo.panjiajie.cn

Py:   while i < 10: i += 1
来源：http://nd.jctech888.com.cn

PHP:  while ($i < 10) { $i++; }
来源：http://cj.yuntaijiaju.cn

JS:   while (i < 10) { i++; }
来源：http://jp.9csxet.cn

TS:   while (i < 10) { i++; }
来源：http://dy.hnjuh.cn

Java: while (i < 10) { i++; }
来源：http://sd.szxytkj.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://sg.nicolike.cn

Ruby: while i < 10; i += 1; end
来源：http://ff.jctech888.com.cn

C#:   while (i < 10) { i++; }
来源：http://aa.bookmarksfly.cn

[B08] do-while（至少执行一次）
来源：http://sb.asd995.cn

Py:   # 无 do-while：用 while True + break
来源：http://lz.hahajie.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://vh.lnxyls.cn

JS:   do { i++; } while (i < 10);
来源：http://iu.huixinmuqiang.cn

TS:   do { i++; } while (i < 10);
来源：http://dq.shxzskj.cn

Java: do { i++; } while (i < 10);
来源：http://rh.jianghongdianzi.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://rt.haigaiapp.cn

Ruby: begin; i += 1; end while i < 10
来源：http://tj.chemitech.net.cn

C#:   do { i++; } while (i < 10);
来源：http://jq.9csxet.cn

[B09] break 与 continue
来源：http://dp.huanxung.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://nh.hnjuh.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://lw.bjjhwx.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pv.shxzukj.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wf.asd995.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vu.yuntaijiaju.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://nl.shtwfgs.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://on.jctech888.com.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uk.bookmarksfly.cn

[B10] 遍历同时拿索引
来源：http://hi.szxytkj.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://gu.bookmarksfly.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://vl.yuntaijiaju.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://jy.jctech888.com.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://dx.nszjky.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://gr.colortex.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://kx.bookmarksfly.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ft.muxihuayi.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://it.jianghongdianzi.cn

[B11] 生成数字序列 / 区间
来源：http://xm.szsharing.cn

Py:   list(range(0, 10, 2))
来源：http://pb.panjiajie.cn

PHP:  range(0, 10, 2);
来源：http://tq.muxihuayi.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://nm.nicolike.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://fo.hahajie.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ab.jianghongdianzi.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hv.huixinmuqiang.cn

Ruby: (0...10).step(2).to_a
来源：http://oo.wgjwhj.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ar.shxzskj.cn

[B12] 跳出多层循环
来源：http://vv.shtwfgs.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ge.9csxet.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://yq.lnxyls.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://qh.panjiajie.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ba.hnjuh.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ax.wgjwhj.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://zh.nicolike.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ef.9csxet.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://es.wgjwhj.cn

[B13] 判断是否为数字
来源：http://kt.521024.cn

Py:   isinstance(x, (int, float))
来源：http://bg.chemitech.net.cn

PHP:  is_numeric($x)
来源：http://ix.lnxyls.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://kt.jianghongdianzi.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://me.wgjwhj.cn

Java: x instanceof Number
来源：http://ej.yuntaijiaju.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mj.huixiangedu.cn

Ruby: x.is_a?(Numeric)
来源：http://ls.nszjky.cn

C#:   x is int or double or decimal
来源：http://xi.9csxet.cn

[B14] 判断值是否在集合内
来源：http://jm.gzmigu.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://yr.chemitech.net.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://aw.hnjuh.cn

JS:   [1, 2, 3].includes(x)
来源：http://vk.szsharing.cn

TS:   [1, 2, 3].includes(x)
来源：http://ha.hnjuh.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://gv.yuntaijiaju.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://jw.9csxet.cn

Ruby: [1, 2, 3].include?(x)
来源：http://io.chemitech.net.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://yn.muxihuayi.cn

[B15] 布尔运算与取反
来源：http://ks.colortex.cn

Py:   a and b or not c
来源：http://kg.nszjky.cn

PHP:  $a && $b || !$c
来源：http://fu.huanxung.cn

JS:   a && b || !c
来源：http://co.wgjwhj.cn

TS:   a && b || !c
来源：http://tm.jianghongdianzi.cn

Java: a && b || !c
来源：http://ph.shxzukj.cn

Go:   a && b || !c
来源：http://qe.newstarts.cn

Ruby: a && b || !c
来源：http://py.shtwfgs.cn

C#:   a && b || !c
来源：http://ie.hnjuh.cn

[B16] 卫语句：不满足条件提前返回
来源：http://as.szxytkj.cn

Py:   if not data: return
来源：http://ll.shxzskj.cn

PHP:  if (!$data) { return; }
来源：http://hq.lnxyls.cn

JS:   if (!data) return;
来源：http://te.huanxung.cn

TS:   if (!data) return;
来源：http://vu.asd995.cn

Java: if (data == null) return;
来源：http://bl.shxzukj.cn

Go:   if data == nil { return }
来源：http://dh.shxzskj.cn

Ruby: return if data.nil?
来源：http://dj.yuexingan06.cn

C#:   if (data == null) return;
来源：http://so.521024.cn

================================================================================
来源：http://yi.bookmarksfly.cn

C. 函数与作用域
来源：http://wr.shxzukj.cn

================================================================================
来源：http://rq.bookmarksfly.cn

[C01] 定义函数
来源：http://mf.jctech888.com.cn

Py:   def add(a, b): return a + b
来源：http://tc.521024.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://io.lnxyls.cn

JS:   function add(a, b) { return a + b; }
来源：http://tj.hnjuh.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://sl.huanxung.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://tj.panjiajie.cn

Go:   func add(a, b int) int { return a + b }
来源：http://wd.huixiangedu.cn

Ruby: def add(a, b); a + b; end
来源：http://qy.chemitech.net.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://et.9csxet.cn

[C02] 默认参数
来源：http://ty.muxihuayi.cn

Py:   def greet(name="World"): return name
来源：http://ux.shtwfgs.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://tv.huixinmuqiang.cn

JS:   function greet(name = "World") { return name; }
来源：http://uf.huixiangedu.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ft.shtwfgs.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://of.jctech888.com.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://cm.nicolike.cn

Ruby: def greet(name = "World") = name
来源：http://cs.yuntaijiaju.cn

C#:   string Greet(string name = "World") => name;
来源：http://km.nicolike.cn

[C03] 可变参数
来源：http://wu.colortex.cn

Py:   def total(*args): return sum(args)
来源：http://jc.panjiajie.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://um.shtwfgs.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hk.jianghongdianzi.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ja.wgjwhj.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://qn.szxytkj.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ak.jianghongdianzi.cn

Ruby: def total(*nums); nums.sum; end
来源：http://qm.bjjhwx.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://cq.nicolike.cn

[C04] 命名参数 / 关键字参数
来源：http://pe.asd995.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://cq.nszjky.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://th.jctech888.com.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://lo.nicolike.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ub.yuexingan06.cn

Java: // 无：用 Builder 模式或 record
来源：http://ek.szxytkj.cn

Go:   // 无：用配置结构体参数
来源：http://op.wgjwhj.cn

Ruby: f(a: 1, b: 2)
来源：http://ma.shxzskj.cn

C#:   f(a: 1, b: 2)
来源：http://bf.hahajie.cn

[C05] 返回多个值
来源：http://fg.wgjwhj.cn

Py:   return a, b
来源：http://no.hnjuh.cn

PHP:  return [$a, $b];
来源：http://du.yuexingan06.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://rg.haigaiapp.cn

TS:   return { a, b };
来源：http://cr.newstarts.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://dr.shxzskj.cn

Go:   return a, b
来源：http://wj.nicolike.cn

Ruby: return a, b
来源：http://ms.muxihuayi.cn

C#:   return (a, b);              // ValueTuple
来源：http://yo.chemitech.net.cn

[C06] 匿名函数 / lambda
来源：http://cd.hnjuh.cn

Py:   square = lambda x: x * x
来源：http://os.haigaiapp.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://uo.shxzskj.cn

JS:   const square = x => x * x;
来源：http://jy.yuexingan06.cn

TS:   const square = (x: number): number => x * x;
来源：http://cl.panjiajie.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://fq.lnxyls.cn

Go:   sq := func(x int) int { return x * x }
来源：http://qd.newstarts.cn

Ruby: square = ->(x) { x * x }
来源：http://aa.shxzskj.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ut.nszjky.cn

[C07] 把函数作为参数传入
来源：http://yf.gzmigu.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://tn.hnjuh.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ix.jianghongdianzi.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://up.521024.cn

TS:   arr.map(String)
来源：http://hz.yuexingan06.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://dm.yuexingan06.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ns.9csxet.cn

Ruby: arr.map(&:upcase)
来源：http://ye.panjiajie.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://fe.huixinmuqiang.cn

[C08] 闭包
来源：http://mq.lnxyls.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://uq.colortex.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://jp.yuexingan06.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://kf.yuntaijiaju.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://in.yuexingan06.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://yb.huixinmuqiang.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://tk.asd995.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ao.colortex.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://jc.chemitech.net.cn

[C09] 递归
来源：http://aj.bookmarksfly.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://du.nicolike.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://qn.colortex.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ih.huanxung.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://jv.bjjhwx.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://fv.huixiangedu.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://pa.shxzskj.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://eb.huanxung.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://he.muxihuayi.cn

[C10] 变量作用域
来源：http://ro.jctech888.com.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://sc.shxzskj.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ho.yuexingan06.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://bl.shxzskj.cn

TS:   同 JS
来源：http://yt.521024.cn

Java: 方法内为块级作用域
来源：http://wg.hahajie.cn

Go:   花括号块级作用域
来源：http://gi.haigaiapp.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hj.panjiajie.cn

C#:   块级作用域
来源：http://zq.wgjwhj.cn

[C11] 模块导入与导出
来源：http://ro.nszjky.cn

Py:   from module import func
来源：http://at.bjjhwx.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://ao.jianghongdianzi.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://bo.lnxyls.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://zz.hnjuh.cn

Java: import java.util.List;
来源：http://wn.szsharing.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://tk.muxihuayi.cn

Ruby: require "json"; require_relative "./util"
来源：http://va.hahajie.cn

C#:   using System.Text;
来源：http://nx.panjiajie.cn

[C12] 立即执行函数 IIFE
来源：http://pg.bookmarksfly.cn

Py:   (lambda: print("run"))()
来源：http://oo.9csxet.cn

PHP:  (function () { echo "run"; })();
来源：http://pk.hahajie.cn

JS:   (() => { console.log("run"); })();
来源：http://qv.jctech888.com.cn

TS:   (() => { console.log("run"); })();
来源：http://yu.hahajie.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://sc.huixinmuqiang.cn

Go:   func() { fmt.Println("run") }()
来源：http://hp.shxzskj.cn

Ruby: -> { puts "run" }.call
来源：http://ez.gzmigu.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://zr.wgjwhj.cn

[C13] 类型声明 / 类型注解
来源：http://nq.521024.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wy.nicolike.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://db.newstarts.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://dk.shtwfgs.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://sv.yuntaijiaju.cn

Java: int add(int a, int b) { return a + b; }
来源：http://ig.huanxung.cn

Go:   func add(a, b int) int
来源：http://hd.gzmigu.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://tv.chemitech.net.cn

C#:   int Add(int a, int b) => a + b;
来源：http://hm.huixinmuqiang.cn

[C14] 泛型函数
来源：http://lg.haigaiapp.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wu.huixinmuqiang.cn

PHP:  // 无泛型
来源：http://xa.szsharing.cn

JS:   // 无泛型
来源：http://gt.colortex.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://zn.huixinmuqiang.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://qf.newstarts.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://vo.muxihuayi.cn

Ruby: # 无泛型
来源：http://du.hnjuh.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://lk.colortex.cn

[C15] 解构 / 展开参数
来源：http://up.521024.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://dx.hnjuh.cn

PHP:  [$a, $b] = $pair;
来源：http://rz.panjiajie.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://yk.colortex.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ym.colortex.cn

Java: // 无解构
来源：http://db.wgjwhj.cn

Go:   // 无解构
来源：http://kb.nszjky.cn

Ruby: a, b = pair
来源：http://hp.9csxet.cn

C#:   var (a, b) = pair;
来源：http://vq.lnxyls.cn

[C16] 函数 / 方法重载
来源：http://qe.521024.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://rn.hnjuh.cn

PHP:  // 无重载
来源：http://ui.huixinmuqiang.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://fs.huixiangedu.cn

TS:   // 用联合类型或重载签名声明
来源：http://ft.yuexingan06.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://pe.haigaiapp.cn

Go:   // 无重载：用不同函数名
来源：http://vy.gzmigu.cn

Ruby: # 无重载：靠动态参数
来源：http://kt.shxzskj.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://pl.panjiajie.cn

================================================================================
来源：http://tw.gzmigu.cn

D. 数组 / 列表 / 集合
来源：http://lv.colortex.cn

================================================================================
来源：http://dx.yuexingan06.cn

[D01] 创建数组 / 列表
来源：http://jf.gzmigu.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://pn.gzmigu.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://vs.gzmigu.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://pm.colortex.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://lo.szsharing.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ih.muxihuayi.cn


<!-- 参考信息 -->