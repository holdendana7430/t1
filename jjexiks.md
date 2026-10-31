代发 wailian999

TS:   const r = x > 0 ? "正" : "非正";
来源：http://vn.bookmarksfly.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://iq.hnjuh.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ml.bjjhwx.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://yd.muxihuayi.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://uf.jianghongdianzi.cn

[B02] 多分支 else if / elif
来源：http://bm.haigaiapp.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://md.hahajie.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://wn.wgjwhj.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jv.shtwfgs.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://em.jianghongdianzi.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bp.lnxyls.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ig.nicolike.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://jj.shxzskj.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qo.panjiajie.cn

[B03] switch / match / case
来源：http://jh.szsharing.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://jt.hnjuh.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://rt.yuntaijiaju.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://sx.huixinmuqiang.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://zv.nszjky.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://nf.jianghongdianzi.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hk.yuntaijiaju.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://lx.huanxung.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ri.muxihuayi.cn

[B04] for 计数循环
来源：http://pr.jianghongdianzi.cn

Py:   for i in range(10): print(i)
来源：http://gx.yuexingan06.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hc.shtwfgs.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://va.hnjuh.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ig.9csxet.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://bn.huixiangedu.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://fa.hnjuh.cn

Ruby: 10.times { |i| puts i }
来源：http://ks.haigaiapp.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://tq.colortex.cn

[B05] 遍历数组 / 列表
来源：http://cc.szxytkj.cn

Py:   for item in arr: print(item)
来源：http://bd.521024.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://br.nicolike.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://za.huixiangedu.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ea.panjiajie.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://nj.jianghongdianzi.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://dv.yuntaijiaju.cn

Ruby: arr.each { |item| puts item }
来源：http://oe.shtwfgs.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://cz.jianghongdianzi.cn

[B06] 遍历字典 / 对象
来源：http://my.9csxet.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ne.nszjky.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://nt.newstarts.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://zs.yuexingan06.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://yq.jctech888.com.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://xh.jctech888.com.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://lo.huanxung.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://eq.9csxet.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://xe.huixinmuqiang.cn

[B07] while 循环
来源：http://di.muxihuayi.cn

Py:   while i < 10: i += 1
来源：http://dj.521024.cn

PHP:  while ($i < 10) { $i++; }
来源：http://qu.jctech888.com.cn

JS:   while (i < 10) { i++; }
来源：http://gv.szsharing.cn

TS:   while (i < 10) { i++; }
来源：http://hl.huixiangedu.cn

Java: while (i < 10) { i++; }
来源：http://ht.wgjwhj.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://km.yuexingan06.cn

Ruby: while i < 10; i += 1; end
来源：http://it.jianghongdianzi.cn

C#:   while (i < 10) { i++; }
来源：http://vx.huixinmuqiang.cn

[B08] do-while（至少执行一次）
来源：http://ms.shtwfgs.cn

Py:   # 无 do-while：用 while True + break
来源：http://hu.bookmarksfly.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://uv.jianghongdianzi.cn

JS:   do { i++; } while (i < 10);
来源：http://dj.huixiangedu.cn

TS:   do { i++; } while (i < 10);
来源：http://ov.chemitech.net.cn

Java: do { i++; } while (i < 10);
来源：http://ya.yuexingan06.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://le.newstarts.cn

Ruby: begin; i += 1; end while i < 10
来源：http://cf.yuntaijiaju.cn

C#:   do { i++; } while (i < 10);
来源：http://qn.jianghongdianzi.cn

[B09] break 与 continue
来源：http://va.nicolike.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://vn.huixiangedu.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ch.lnxyls.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://do.lnxyls.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hn.jctech888.com.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bn.yuexingan06.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ps.chemitech.net.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://uz.newstarts.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ny.hnjuh.cn

[B10] 遍历同时拿索引
来源：http://bu.hnjuh.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://tu.hnjuh.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://qn.jianghongdianzi.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://qy.jianghongdianzi.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://al.haigaiapp.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ga.lnxyls.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://yo.521024.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://bw.shxzukj.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ic.szxytkj.cn

[B11] 生成数字序列 / 区间
来源：http://uj.panjiajie.cn

Py:   list(range(0, 10, 2))
来源：http://ev.muxihuayi.cn

PHP:  range(0, 10, 2);
来源：http://id.chemitech.net.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://pp.chemitech.net.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://az.9csxet.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://vo.jctech888.com.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://dw.muxihuayi.cn

Ruby: (0...10).step(2).to_a
来源：http://af.szsharing.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://zm.szxytkj.cn

[B12] 跳出多层循环
来源：http://ld.huixiangedu.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://vm.colortex.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://hd.jianghongdianzi.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://pb.nszjky.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://oy.yuntaijiaju.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://tk.shxzukj.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://co.9csxet.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://pl.jianghongdianzi.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://dg.nicolike.cn

[B13] 判断是否为数字
来源：http://yj.nicolike.cn

Py:   isinstance(x, (int, float))
来源：http://xl.9csxet.cn

PHP:  is_numeric($x)
来源：http://pr.521024.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ln.9csxet.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qn.bjjhwx.cn

Java: x instanceof Number
来源：http://lc.huixinmuqiang.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://xv.panjiajie.cn

Ruby: x.is_a?(Numeric)
来源：http://pr.521024.cn

C#:   x is int or double or decimal
来源：http://zk.muxihuayi.cn

[B14] 判断值是否在集合内
来源：http://mf.newstarts.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://cl.panjiajie.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://nr.shxzukj.cn

JS:   [1, 2, 3].includes(x)
来源：http://qt.huixiangedu.cn

TS:   [1, 2, 3].includes(x)
来源：http://sq.9csxet.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ut.chemitech.net.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://yb.szxytkj.cn

Ruby: [1, 2, 3].include?(x)
来源：http://uz.bjjhwx.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mp.bookmarksfly.cn

[B15] 布尔运算与取反
来源：http://ew.jianghongdianzi.cn

Py:   a and b or not c
来源：http://rg.nicolike.cn

PHP:  $a && $b || !$c
来源：http://yr.huixiangedu.cn

JS:   a && b || !c
来源：http://gd.wgjwhj.cn

TS:   a && b || !c
来源：http://jx.shxzskj.cn

Java: a && b || !c
来源：http://fb.szxytkj.cn

Go:   a && b || !c
来源：http://vk.huixiangedu.cn

Ruby: a && b || !c
来源：http://ok.colortex.cn

C#:   a && b || !c
来源：http://kk.bookmarksfly.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ol.hahajie.cn

Py:   if not data: return
来源：http://um.szsharing.cn

PHP:  if (!$data) { return; }
来源：http://em.9csxet.cn

JS:   if (!data) return;
来源：http://on.gzmigu.cn

TS:   if (!data) return;
来源：http://iv.colortex.cn

Java: if (data == null) return;
来源：http://te.lnxyls.cn

Go:   if data == nil { return }
来源：http://uc.yuexingan06.cn

Ruby: return if data.nil?
来源：http://fz.jianghongdianzi.cn

C#:   if (data == null) return;
来源：http://sb.lnxyls.cn

================================================================================
来源：http://fp.szsharing.cn

C. 函数与作用域
来源：http://tr.yuexingan06.cn

================================================================================
来源：http://vu.haigaiapp.cn

[C01] 定义函数
来源：http://xb.bjjhwx.cn

Py:   def add(a, b): return a + b
来源：http://te.jianghongdianzi.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mc.asd995.cn

JS:   function add(a, b) { return a + b; }
来源：http://gz.shxzskj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://vm.yuntaijiaju.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://xb.newstarts.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ur.bookmarksfly.cn

Ruby: def add(a, b); a + b; end
来源：http://hq.asd995.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mo.huixiangedu.cn

[C02] 默认参数
来源：http://xv.chemitech.net.cn

Py:   def greet(name="World"): return name
来源：http://lc.asd995.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://pi.jctech888.com.cn

JS:   function greet(name = "World") { return name; }
来源：http://uk.yuexingan06.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://xg.muxihuayi.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://jn.yuntaijiaju.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wb.bookmarksfly.cn

Ruby: def greet(name = "World") = name
来源：http://yw.nicolike.cn

C#:   string Greet(string name = "World") => name;
来源：http://ct.wgjwhj.cn

[C03] 可变参数
来源：http://lr.jctech888.com.cn

Py:   def total(*args): return sum(args)
来源：http://da.lnxyls.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://xg.shxzukj.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://nv.muxihuayi.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://fu.newstarts.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://fv.shxzukj.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ym.huixiangedu.cn

Ruby: def total(*nums); nums.sum; end
来源：http://sx.shxzukj.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://db.9csxet.cn

[C04] 命名参数 / 关键字参数
来源：http://qy.yuexingan06.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://lf.yuntaijiaju.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://oe.huixinmuqiang.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://gp.9csxet.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ib.huanxung.cn

Java: // 无：用 Builder 模式或 record
来源：http://du.hnjuh.cn

Go:   // 无：用配置结构体参数
来源：http://dy.521024.cn

Ruby: f(a: 1, b: 2)
来源：http://vt.yuntaijiaju.cn

C#:   f(a: 1, b: 2)
来源：http://fy.521024.cn

[C05] 返回多个值
来源：http://gu.jianghongdianzi.cn

Py:   return a, b
来源：http://pt.asd995.cn

PHP:  return [$a, $b];
来源：http://af.hnjuh.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://av.yuntaijiaju.cn

TS:   return { a, b };
来源：http://zj.bookmarksfly.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://vq.hnjuh.cn

Go:   return a, b
来源：http://qs.yuntaijiaju.cn

Ruby: return a, b
来源：http://zf.chemitech.net.cn

C#:   return (a, b);              // ValueTuple
来源：http://mo.shxzskj.cn

[C06] 匿名函数 / lambda
来源：http://vy.huixinmuqiang.cn

Py:   square = lambda x: x * x
来源：http://il.huixiangedu.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://iv.yuntaijiaju.cn

JS:   const square = x => x * x;
来源：http://tg.bookmarksfly.cn

TS:   const square = (x: number): number => x * x;
来源：http://hh.521024.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://nu.shtwfgs.cn

Go:   sq := func(x int) int { return x * x }
来源：http://wk.colortex.cn

Ruby: square = ->(x) { x * x }
来源：http://mr.panjiajie.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ed.szsharing.cn

[C07] 把函数作为参数传入
来源：http://nr.lnxyls.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://kw.muxihuayi.cn

PHP:  array_map("strtoupper", $arr);
来源：http://uv.shtwfgs.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mn.colortex.cn

TS:   arr.map(String)
来源：http://id.nszjky.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://am.haigaiapp.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://xg.jctech888.com.cn

Ruby: arr.map(&:upcase)
来源：http://yy.panjiajie.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://jm.shxzukj.cn

[C08] 闭包
来源：http://rt.jctech888.com.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://oh.colortex.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://lo.jianghongdianzi.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://gt.bjjhwx.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://he.bookmarksfly.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://pb.panjiajie.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://fq.colortex.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wv.shxzskj.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://df.szxytkj.cn

[C09] 递归
来源：http://ep.nszjky.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://oi.huixinmuqiang.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://eg.panjiajie.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://sn.muxihuayi.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://um.yuntaijiaju.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://oa.muxihuayi.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://gx.wgjwhj.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://cv.newstarts.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ej.nicolike.cn

[C10] 变量作用域
来源：http://tn.lnxyls.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ts.nicolike.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://lc.yuntaijiaju.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ar.newstarts.cn

TS:   同 JS
来源：http://ds.wgjwhj.cn

Java: 方法内为块级作用域
来源：http://bn.szxytkj.cn

Go:   花括号块级作用域
来源：http://hw.panjiajie.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://fr.hahajie.cn

C#:   块级作用域
来源：http://yh.lnxyls.cn

[C11] 模块导入与导出
来源：http://yi.huixinmuqiang.cn

Py:   from module import func
来源：http://db.panjiajie.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://rj.nicolike.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://ia.szsharing.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://in.lnxyls.cn

Java: import java.util.List;
来源：http://jo.newstarts.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://gp.bookmarksfly.cn

Ruby: require "json"; require_relative "./util"
来源：http://jt.huanxung.cn

C#:   using System.Text;
来源：http://gf.chemitech.net.cn

[C12] 立即执行函数 IIFE
来源：http://aq.muxihuayi.cn

Py:   (lambda: print("run"))()
来源：http://pd.haigaiapp.cn

PHP:  (function () { echo "run"; })();
来源：http://tj.yuntaijiaju.cn

JS:   (() => { console.log("run"); })();
来源：http://bv.asd995.cn

TS:   (() => { console.log("run"); })();
来源：http://lg.gzmigu.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://jz.newstarts.cn

Go:   func() { fmt.Println("run") }()
来源：http://lx.bjjhwx.cn

Ruby: -> { puts "run" }.call
来源：http://de.szxytkj.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://rt.wgjwhj.cn

[C13] 类型声明 / 类型注解
来源：http://ng.asd995.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://kc.hnjuh.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://lk.hahajie.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ve.huanxung.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://rm.huanxung.cn

Java: int add(int a, int b) { return a + b; }
来源：http://yt.shxzskj.cn

Go:   func add(a, b int) int
来源：http://yd.szsharing.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://xo.haigaiapp.cn

C#:   int Add(int a, int b) => a + b;
来源：http://zm.newstarts.cn

[C14] 泛型函数
来源：http://su.521024.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://is.panjiajie.cn

PHP:  // 无泛型
来源：http://rp.jctech888.com.cn

JS:   // 无泛型
来源：http://hg.lnxyls.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://bk.nszjky.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://fh.jianghongdianzi.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ej.huanxung.cn

Ruby: # 无泛型
来源：http://wl.chemitech.net.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://zt.shxzukj.cn

[C15] 解构 / 展开参数
来源：http://ab.wgjwhj.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://pg.huanxung.cn

PHP:  [$a, $b] = $pair;
来源：http://fs.szsharing.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://rn.muxihuayi.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://be.shxzskj.cn

Java: // 无解构
来源：http://oc.muxihuayi.cn

Go:   // 无解构
来源：http://uf.haigaiapp.cn

Ruby: a, b = pair
来源：http://xc.shxzskj.cn

C#:   var (a, b) = pair;
来源：http://mb.yuexingan06.cn

[C16] 函数 / 方法重载
来源：http://yc.hahajie.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ir.haigaiapp.cn

PHP:  // 无重载
来源：http://lr.haigaiapp.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://xj.szxytkj.cn

TS:   // 用联合类型或重载签名声明
来源：http://ti.hahajie.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://fa.lnxyls.cn

Go:   // 无重载：用不同函数名
来源：http://aj.nszjky.cn

Ruby: # 无重载：靠动态参数
来源：http://yw.jianghongdianzi.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://on.hahajie.cn

================================================================================
来源：http://um.huanxung.cn

D. 数组 / 列表 / 集合
来源：http://kc.panjiajie.cn

================================================================================
来源：http://rj.bookmarksfly.cn

[D01] 创建数组 / 列表
来源：http://zq.521024.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://xu.nicolike.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://cw.521024.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://pq.shxzukj.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://de.yuexingan06.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ei.asd995.cn

Go:   arr := []int{1, 2, 3}
来源：http://di.jctech888.com.cn

Ruby: arr = [1, 2, 3]
来源：http://qg.521024.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ac.szxytkj.cn

[D02] 追加元素到末尾
来源：http://gj.newstarts.cn


<!-- 参考信息 -->