代发 wailian999

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://wz.jctech888.com.cn

================================================================================
来源：http://ux.huanxung.cn

B. 流程控制
来源：http://ml.521024.cn

================================================================================
来源：http://mm.haigaiapp.cn

[B01] 条件判断 if / else
来源：http://au.lnxyls.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://dg.asd995.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://qt.shxzukj.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://lb.panjiajie.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://dx.yuntaijiaju.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://xe.szxytkj.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://yy.newstarts.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ey.bookmarksfly.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ve.newstarts.cn

[B02] 多分支 else if / elif
来源：http://bi.colortex.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://pe.yuntaijiaju.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://jo.huixinmuqiang.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sb.yuexingan06.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lz.nicolike.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://am.muxihuayi.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://sv.9csxet.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://lr.bookmarksfly.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qh.bjjhwx.cn

[B03] switch / match / case
来源：http://cw.muxihuayi.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ys.huixiangedu.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://vp.newstarts.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://gi.nicolike.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://gm.521024.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://rb.muxihuayi.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://at.9csxet.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ua.huixiangedu.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://xs.muxihuayi.cn

[B04] for 计数循环
来源：http://sg.hahajie.cn

Py:   for i in range(10): print(i)
来源：http://zw.lnxyls.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://zy.newstarts.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://bm.szsharing.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ag.521024.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://od.jctech888.com.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://jl.huixinmuqiang.cn

Ruby: 10.times { |i| puts i }
来源：http://ir.szxytkj.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://he.9csxet.cn

[B05] 遍历数组 / 列表
来源：http://kt.haigaiapp.cn

Py:   for item in arr: print(item)
来源：http://cp.huixiangedu.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ze.gzmigu.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://hf.jctech888.com.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://tj.bookmarksfly.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://gn.shxzukj.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://th.asd995.cn

Ruby: arr.each { |item| puts item }
来源：http://zc.huixinmuqiang.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://dx.colortex.cn

[B06] 遍历字典 / 对象
来源：http://hv.chemitech.net.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://jq.nicolike.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wh.huixiangedu.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://xn.colortex.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wc.huixiangedu.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://bg.asd995.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://sv.yuntaijiaju.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://vr.shxzukj.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ao.9csxet.cn

[B07] while 循环
来源：http://wk.asd995.cn

Py:   while i < 10: i += 1
来源：http://jh.wgjwhj.cn

PHP:  while ($i < 10) { $i++; }
来源：http://kp.lnxyls.cn

JS:   while (i < 10) { i++; }
来源：http://er.nszjky.cn

TS:   while (i < 10) { i++; }
来源：http://dx.shxzukj.cn

Java: while (i < 10) { i++; }
来源：http://xy.jctech888.com.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://bq.shxzskj.cn

Ruby: while i < 10; i += 1; end
来源：http://ad.szxytkj.cn

C#:   while (i < 10) { i++; }
来源：http://yr.colortex.cn

[B08] do-while（至少执行一次）
来源：http://se.muxihuayi.cn

Py:   # 无 do-while：用 while True + break
来源：http://az.shxzskj.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://xj.jianghongdianzi.cn

JS:   do { i++; } while (i < 10);
来源：http://hm.lnxyls.cn

TS:   do { i++; } while (i < 10);
来源：http://on.asd995.cn

Java: do { i++; } while (i < 10);
来源：http://ul.chemitech.net.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://zh.521024.cn

Ruby: begin; i += 1; end while i < 10
来源：http://cs.szsharing.cn

C#:   do { i++; } while (i < 10);
来源：http://pn.lnxyls.cn

[B09] break 与 continue
来源：http://mp.haigaiapp.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://nu.bookmarksfly.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://xm.shtwfgs.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qk.521024.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jn.hahajie.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ss.huanxung.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://gl.haigaiapp.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://fp.yuexingan06.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kj.asd995.cn

[B10] 遍历同时拿索引
来源：http://af.shtwfgs.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://rj.hnjuh.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://qp.huixinmuqiang.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hs.colortex.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hw.yuexingan06.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://en.nszjky.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://nw.chemitech.net.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://rr.huixiangedu.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ve.huanxung.cn

[B11] 生成数字序列 / 区间
来源：http://ur.szxytkj.cn

Py:   list(range(0, 10, 2))
来源：http://fm.shtwfgs.cn

PHP:  range(0, 10, 2);
来源：http://wx.szxytkj.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://pw.bookmarksfly.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://kw.nicolike.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://fd.nicolike.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://nj.hnjuh.cn

Ruby: (0...10).step(2).to_a
来源：http://jd.szsharing.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://lh.asd995.cn

[B12] 跳出多层循环
来源：http://qx.jctech888.com.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://nt.jianghongdianzi.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://cu.huixiangedu.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://aq.lnxyls.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ye.chemitech.net.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://qp.yuntaijiaju.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://kg.nszjky.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ri.lnxyls.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://rn.hahajie.cn

[B13] 判断是否为数字
来源：http://gb.bookmarksfly.cn

Py:   isinstance(x, (int, float))
来源：http://iz.hnjuh.cn

PHP:  is_numeric($x)
来源：http://hd.shtwfgs.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://yx.asd995.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://tq.asd995.cn

Java: x instanceof Number
来源：http://vf.szxytkj.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hv.bjjhwx.cn

Ruby: x.is_a?(Numeric)
来源：http://yp.jctech888.com.cn

C#:   x is int or double or decimal
来源：http://sw.szsharing.cn

[B14] 判断值是否在集合内
来源：http://dj.huanxung.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hb.shtwfgs.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://qu.muxihuayi.cn

JS:   [1, 2, 3].includes(x)
来源：http://ah.jctech888.com.cn

TS:   [1, 2, 3].includes(x)
来源：http://ca.shtwfgs.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://rj.lnxyls.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://kr.gzmigu.cn

Ruby: [1, 2, 3].include?(x)
来源：http://tc.muxihuayi.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://yc.muxihuayi.cn

[B15] 布尔运算与取反
来源：http://ih.yuntaijiaju.cn

Py:   a and b or not c
来源：http://zm.yuntaijiaju.cn

PHP:  $a && $b || !$c
来源：http://vw.shtwfgs.cn

JS:   a && b || !c
来源：http://aa.hahajie.cn

TS:   a && b || !c
来源：http://lb.wgjwhj.cn

Java: a && b || !c
来源：http://hw.shxzskj.cn

Go:   a && b || !c
来源：http://fx.bjjhwx.cn

Ruby: a && b || !c
来源：http://jy.szxytkj.cn

C#:   a && b || !c
来源：http://in.huixiangedu.cn

[B16] 卫语句：不满足条件提前返回
来源：http://xu.wgjwhj.cn

Py:   if not data: return
来源：http://wc.jctech888.com.cn

PHP:  if (!$data) { return; }
来源：http://if.panjiajie.cn

JS:   if (!data) return;
来源：http://qx.huixinmuqiang.cn

TS:   if (!data) return;
来源：http://ma.hnjuh.cn

Java: if (data == null) return;
来源：http://wt.huanxung.cn

Go:   if data == nil { return }
来源：http://nv.szsharing.cn

Ruby: return if data.nil?
来源：http://ji.huanxung.cn

C#:   if (data == null) return;
来源：http://rm.bjjhwx.cn

================================================================================
来源：http://dp.gzmigu.cn

C. 函数与作用域
来源：http://zq.yuntaijiaju.cn

================================================================================
来源：http://oq.jctech888.com.cn

[C01] 定义函数
来源：http://hp.colortex.cn

Py:   def add(a, b): return a + b
来源：http://bu.jctech888.com.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://kg.bookmarksfly.cn

JS:   function add(a, b) { return a + b; }
来源：http://su.wgjwhj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ba.hnjuh.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://vg.bjjhwx.cn

Go:   func add(a, b int) int { return a + b }
来源：http://yg.lnxyls.cn

Ruby: def add(a, b); a + b; end
来源：http://ap.huixiangedu.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://at.muxihuayi.cn

[C02] 默认参数
来源：http://bq.jianghongdianzi.cn

Py:   def greet(name="World"): return name
来源：http://hx.shxzukj.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://oy.yuexingan06.cn

JS:   function greet(name = "World") { return name; }
来源：http://rm.hnjuh.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://eg.shxzukj.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://jq.huixinmuqiang.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://io.nicolike.cn

Ruby: def greet(name = "World") = name
来源：http://ej.yuntaijiaju.cn

C#:   string Greet(string name = "World") => name;
来源：http://vv.shxzukj.cn

[C03] 可变参数
来源：http://vb.jctech888.com.cn

Py:   def total(*args): return sum(args)
来源：http://cz.colortex.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://jx.huanxung.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wt.muxihuayi.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://kp.nicolike.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://jp.shxzukj.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://kt.yuntaijiaju.cn

Ruby: def total(*nums); nums.sum; end
来源：http://ov.jctech888.com.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://qr.gzmigu.cn

[C04] 命名参数 / 关键字参数
来源：http://nz.jctech888.com.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ui.colortex.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://in.colortex.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ki.nicolike.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://qt.shxzskj.cn

Java: // 无：用 Builder 模式或 record
来源：http://im.yuexingan06.cn

Go:   // 无：用配置结构体参数
来源：http://ff.newstarts.cn

Ruby: f(a: 1, b: 2)
来源：http://dz.jianghongdianzi.cn

C#:   f(a: 1, b: 2)
来源：http://jo.colortex.cn

[C05] 返回多个值
来源：http://vg.huanxung.cn

Py:   return a, b
来源：http://bm.shxzukj.cn

PHP:  return [$a, $b];
来源：http://vs.shxzukj.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://pv.shtwfgs.cn

TS:   return { a, b };
来源：http://hw.lnxyls.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://yt.shtwfgs.cn

Go:   return a, b
来源：http://uw.shtwfgs.cn

Ruby: return a, b
来源：http://hy.haigaiapp.cn

C#:   return (a, b);              // ValueTuple
来源：http://xx.yuntaijiaju.cn

[C06] 匿名函数 / lambda
来源：http://zh.shtwfgs.cn

Py:   square = lambda x: x * x
来源：http://ho.9csxet.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://iy.newstarts.cn

JS:   const square = x => x * x;
来源：http://wy.9csxet.cn

TS:   const square = (x: number): number => x * x;
来源：http://pf.colortex.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://lk.haigaiapp.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ky.lnxyls.cn

Ruby: square = ->(x) { x * x }
来源：http://fs.yuntaijiaju.cn

C#:   Func<int, int> square = x => x * x;
来源：http://br.521024.cn

[C07] 把函数作为参数传入
来源：http://rx.wgjwhj.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://xo.chemitech.net.cn

PHP:  array_map("strtoupper", $arr);
来源：http://li.hnjuh.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://fr.newstarts.cn

TS:   arr.map(String)
来源：http://lo.chemitech.net.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://el.chemitech.net.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://of.szxytkj.cn

Ruby: arr.map(&:upcase)
来源：http://ht.asd995.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://hc.wgjwhj.cn

[C08] 闭包
来源：http://bs.nicolike.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ce.huanxung.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://xv.muxihuayi.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://aa.asd995.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://vh.yuexingan06.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://du.huixiangedu.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ea.asd995.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ew.szxytkj.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://vn.haigaiapp.cn

[C09] 递归
来源：http://eq.bjjhwx.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://px.muxihuayi.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ra.szsharing.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://rz.asd995.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://om.haigaiapp.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wk.huanxung.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://xx.9csxet.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://os.szsharing.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://og.asd995.cn

[C10] 变量作用域
来源：http://qq.gzmigu.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://pd.newstarts.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wz.shxzukj.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://fy.haigaiapp.cn

TS:   同 JS
来源：http://cm.huixinmuqiang.cn

Java: 方法内为块级作用域
来源：http://uv.huixiangedu.cn

Go:   花括号块级作用域
来源：http://es.hnjuh.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://nx.bookmarksfly.cn

C#:   块级作用域
来源：http://jl.nszjky.cn

[C11] 模块导入与导出
来源：http://ad.yuntaijiaju.cn

Py:   from module import func
来源：http://cy.huixiangedu.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://cq.shxzskj.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://bn.jctech888.com.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://pd.521024.cn

Java: import java.util.List;
来源：http://gx.shxzskj.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://sn.shxzskj.cn

Ruby: require "json"; require_relative "./util"
来源：http://aa.muxihuayi.cn

C#:   using System.Text;
来源：http://mk.yuntaijiaju.cn

[C12] 立即执行函数 IIFE
来源：http://ew.shxzskj.cn

Py:   (lambda: print("run"))()
来源：http://en.hahajie.cn

PHP:  (function () { echo "run"; })();
来源：http://ra.huanxung.cn

JS:   (() => { console.log("run"); })();
来源：http://tn.szsharing.cn

TS:   (() => { console.log("run"); })();
来源：http://jq.521024.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://gq.huixiangedu.cn

Go:   func() { fmt.Println("run") }()
来源：http://wu.colortex.cn

Ruby: -> { puts "run" }.call
来源：http://ai.jctech888.com.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ml.panjiajie.cn

[C13] 类型声明 / 类型注解
来源：http://hn.jctech888.com.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ko.jianghongdianzi.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://tk.nicolike.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ol.gzmigu.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ba.chemitech.net.cn

Java: int add(int a, int b) { return a + b; }
来源：http://cz.lnxyls.cn

Go:   func add(a, b int) int
来源：http://rk.shxzskj.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://av.huixinmuqiang.cn

C#:   int Add(int a, int b) => a + b;
来源：http://og.jianghongdianzi.cn

[C14] 泛型函数
来源：http://yo.yuexingan06.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://iv.bjjhwx.cn

PHP:  // 无泛型
来源：http://bi.huixiangedu.cn

JS:   // 无泛型
来源：http://uj.bjjhwx.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://rl.shxzukj.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hk.lnxyls.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://qu.haigaiapp.cn

Ruby: # 无泛型
来源：http://fa.huixiangedu.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://jd.jianghongdianzi.cn

[C15] 解构 / 展开参数
来源：http://oi.bookmarksfly.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://je.shxzukj.cn

PHP:  [$a, $b] = $pair;
来源：http://gw.chemitech.net.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://bw.haigaiapp.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ii.huanxung.cn

Java: // 无解构
来源：http://ej.wgjwhj.cn

Go:   // 无解构
来源：http://ak.9csxet.cn

Ruby: a, b = pair
来源：http://xy.huanxung.cn

C#:   var (a, b) = pair;
来源：http://iz.lnxyls.cn

[C16] 函数 / 方法重载
来源：http://qu.521024.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://vn.huixiangedu.cn

PHP:  // 无重载
来源：http://ma.hahajie.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://lb.haigaiapp.cn

TS:   // 用联合类型或重载签名声明
来源：http://pm.colortex.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://wh.asd995.cn

Go:   // 无重载：用不同函数名
来源：http://tj.huanxung.cn

Ruby: # 无重载：靠动态参数
来源：http://jq.bookmarksfly.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://yk.huixinmuqiang.cn

================================================================================
来源：http://hy.lnxyls.cn

D. 数组 / 列表 / 集合
来源：http://to.521024.cn

================================================================================
来源：http://zo.szsharing.cn

[D01] 创建数组 / 列表
来源：http://vp.huanxung.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://cb.jctech888.com.cn


<!-- 参考信息 -->