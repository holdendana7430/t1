代发 wailian999

[B01] 条件判断 if / else
来源：http://cb.jctech888.com.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://ba.asd995.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://cr.muxihuayi.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://iw.muxihuayi.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hf.muxihuayi.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://sc.wgjwhj.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://za.521024.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://fj.colortex.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://id.jianghongdianzi.cn

[B02] 多分支 else if / elif
来源：http://df.newstarts.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ys.521024.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://bw.wgjwhj.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lb.chemitech.net.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wi.jctech888.com.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hq.jianghongdianzi.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://oy.chemitech.net.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://eg.jctech888.com.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qf.colortex.cn

[B03] switch / match / case
来源：http://br.szxytkj.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://nc.huixinmuqiang.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://js.yuntaijiaju.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://pc.521024.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://qu.bookmarksfly.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://lx.newstarts.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://lb.jianghongdianzi.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://jo.asd995.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://qy.lnxyls.cn

[B04] for 计数循环
来源：http://xr.nszjky.cn

Py:   for i in range(10): print(i)
来源：http://ed.bookmarksfly.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://zm.huanxung.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wb.szsharing.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://vs.colortex.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://cc.lnxyls.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://jv.haigaiapp.cn

Ruby: 10.times { |i| puts i }
来源：http://bj.wgjwhj.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://lw.huixinmuqiang.cn

[B05] 遍历数组 / 列表
来源：http://jv.szxytkj.cn

Py:   for item in arr: print(item)
来源：http://kq.yuexingan06.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ce.bjjhwx.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://rw.bjjhwx.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://xa.521024.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://tg.shxzskj.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ff.nszjky.cn

Ruby: arr.each { |item| puts item }
来源：http://sn.huanxung.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://rk.bjjhwx.cn

[B06] 遍历字典 / 对象
来源：http://jt.jctech888.com.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://rd.yuntaijiaju.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://sx.shxzukj.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://yb.newstarts.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://js.bjjhwx.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://yk.colortex.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://xf.shxzukj.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://bb.hahajie.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://cy.bjjhwx.cn

[B07] while 循环
来源：http://kt.wgjwhj.cn

Py:   while i < 10: i += 1
来源：http://jj.9csxet.cn

PHP:  while ($i < 10) { $i++; }
来源：http://tx.newstarts.cn

JS:   while (i < 10) { i++; }
来源：http://rk.gzmigu.cn

TS:   while (i < 10) { i++; }
来源：http://uk.chemitech.net.cn

Java: while (i < 10) { i++; }
来源：http://mx.jctech888.com.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://zn.nszjky.cn

Ruby: while i < 10; i += 1; end
来源：http://hk.shxzskj.cn

C#:   while (i < 10) { i++; }
来源：http://fq.gzmigu.cn

[B08] do-while（至少执行一次）
来源：http://yc.haigaiapp.cn

Py:   # 无 do-while：用 while True + break
来源：http://wu.hahajie.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://xg.yuexingan06.cn

JS:   do { i++; } while (i < 10);
来源：http://cq.nicolike.cn

TS:   do { i++; } while (i < 10);
来源：http://tw.huanxung.cn

Java: do { i++; } while (i < 10);
来源：http://xs.hnjuh.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://cp.muxihuayi.cn

Ruby: begin; i += 1; end while i < 10
来源：http://hr.szxytkj.cn

C#:   do { i++; } while (i < 10);
来源：http://md.9csxet.cn

[B09] break 与 continue
来源：http://pr.yuntaijiaju.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://qe.shxzukj.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://dc.hahajie.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ck.shtwfgs.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bf.yuntaijiaju.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nt.chemitech.net.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://fn.wgjwhj.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://zi.yuntaijiaju.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ok.bjjhwx.cn

[B10] 遍历同时拿索引
来源：http://iz.gzmigu.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://bt.shtwfgs.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://rm.gzmigu.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://sf.lnxyls.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://rr.szsharing.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://fn.hahajie.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ms.shxzukj.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://cj.bjjhwx.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://zb.huanxung.cn

[B11] 生成数字序列 / 区间
来源：http://by.huanxung.cn

Py:   list(range(0, 10, 2))
来源：http://xd.muxihuayi.cn

PHP:  range(0, 10, 2);
来源：http://kw.asd995.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://rf.szxytkj.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://vx.lnxyls.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://aj.lnxyls.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://gx.9csxet.cn

Ruby: (0...10).step(2).to_a
来源：http://qn.panjiajie.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://dt.muxihuayi.cn

[B12] 跳出多层循环
来源：http://wk.szsharing.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ik.newstarts.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://gn.wgjwhj.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ed.haigaiapp.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://yr.jctech888.com.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://pr.jctech888.com.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ad.colortex.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wt.muxihuayi.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://gn.yuexingan06.cn

[B13] 判断是否为数字
来源：http://qr.bjjhwx.cn

Py:   isinstance(x, (int, float))
来源：http://cs.521024.cn

PHP:  is_numeric($x)
来源：http://yd.asd995.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hu.huixiangedu.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://gf.huanxung.cn

Java: x instanceof Number
来源：http://bv.szxytkj.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://yt.yuexingan06.cn

Ruby: x.is_a?(Numeric)
来源：http://xn.panjiajie.cn

C#:   x is int or double or decimal
来源：http://ap.muxihuayi.cn

[B14] 判断值是否在集合内
来源：http://ee.nicolike.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ns.wgjwhj.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://dc.hahajie.cn

JS:   [1, 2, 3].includes(x)
来源：http://qt.lnxyls.cn

TS:   [1, 2, 3].includes(x)
来源：http://mn.gzmigu.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://oh.yuntaijiaju.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://iy.bookmarksfly.cn

Ruby: [1, 2, 3].include?(x)
来源：http://af.bjjhwx.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://fk.huixiangedu.cn

[B15] 布尔运算与取反
来源：http://na.hahajie.cn

Py:   a and b or not c
来源：http://kb.yuntaijiaju.cn

PHP:  $a && $b || !$c
来源：http://kc.muxihuayi.cn

JS:   a && b || !c
来源：http://fu.shxzskj.cn

TS:   a && b || !c
来源：http://uf.shxzskj.cn

Java: a && b || !c
来源：http://tx.gzmigu.cn

Go:   a && b || !c
来源：http://ys.huanxung.cn

Ruby: a && b || !c
来源：http://hs.asd995.cn

C#:   a && b || !c
来源：http://qe.haigaiapp.cn

[B16] 卫语句：不满足条件提前返回
来源：http://wz.newstarts.cn

Py:   if not data: return
来源：http://dt.panjiajie.cn

PHP:  if (!$data) { return; }
来源：http://op.nicolike.cn

JS:   if (!data) return;
来源：http://fg.521024.cn

TS:   if (!data) return;
来源：http://ba.bookmarksfly.cn

Java: if (data == null) return;
来源：http://dv.hahajie.cn

Go:   if data == nil { return }
来源：http://bj.jctech888.com.cn

Ruby: return if data.nil?
来源：http://zb.muxihuayi.cn

C#:   if (data == null) return;
来源：http://mh.szsharing.cn

================================================================================
来源：http://fx.jctech888.com.cn

C. 函数与作用域
来源：http://ar.muxihuayi.cn

================================================================================
来源：http://hm.panjiajie.cn

[C01] 定义函数
来源：http://bz.hahajie.cn

Py:   def add(a, b): return a + b
来源：http://xf.jctech888.com.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ih.haigaiapp.cn

JS:   function add(a, b) { return a + b; }
来源：http://ty.hnjuh.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mh.newstarts.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://gc.huixinmuqiang.cn

Go:   func add(a, b int) int { return a + b }
来源：http://pv.shxzukj.cn

Ruby: def add(a, b); a + b; end
来源：http://km.bookmarksfly.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mb.yuntaijiaju.cn

[C02] 默认参数
来源：http://pk.haigaiapp.cn

Py:   def greet(name="World"): return name
来源：http://fa.asd995.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://bp.hahajie.cn

JS:   function greet(name = "World") { return name; }
来源：http://fh.colortex.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://hu.newstarts.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://jf.szsharing.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ga.colortex.cn

Ruby: def greet(name = "World") = name
来源：http://kq.panjiajie.cn

C#:   string Greet(string name = "World") => name;
来源：http://di.szxytkj.cn

[C03] 可变参数
来源：http://hl.colortex.cn

Py:   def total(*args): return sum(args)
来源：http://sf.shxzukj.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://td.521024.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://pj.panjiajie.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://vl.lnxyls.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://uj.szsharing.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://uc.gzmigu.cn

Ruby: def total(*nums); nums.sum; end
来源：http://es.nicolike.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://cu.jctech888.com.cn

[C04] 命名参数 / 关键字参数
来源：http://yv.asd995.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://fw.hnjuh.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://su.newstarts.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://aa.bookmarksfly.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://lj.lnxyls.cn

Java: // 无：用 Builder 模式或 record
来源：http://fv.bjjhwx.cn

Go:   // 无：用配置结构体参数
来源：http://uu.9csxet.cn

Ruby: f(a: 1, b: 2)
来源：http://rh.jctech888.com.cn

C#:   f(a: 1, b: 2)
来源：http://yu.nszjky.cn

[C05] 返回多个值
来源：http://ml.colortex.cn

Py:   return a, b
来源：http://zr.yuntaijiaju.cn

PHP:  return [$a, $b];
来源：http://ww.nszjky.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ep.huanxung.cn

TS:   return { a, b };
来源：http://mh.muxihuayi.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://pv.jianghongdianzi.cn

Go:   return a, b
来源：http://es.9csxet.cn

Ruby: return a, b
来源：http://ci.hahajie.cn

C#:   return (a, b);              // ValueTuple
来源：http://ec.shxzskj.cn

[C06] 匿名函数 / lambda
来源：http://uv.nicolike.cn

Py:   square = lambda x: x * x
来源：http://ii.jctech888.com.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ce.bjjhwx.cn

JS:   const square = x => x * x;
来源：http://bc.521024.cn

TS:   const square = (x: number): number => x * x;
来源：http://hg.gzmigu.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ut.jianghongdianzi.cn

Go:   sq := func(x int) int { return x * x }
来源：http://tn.shtwfgs.cn

Ruby: square = ->(x) { x * x }
来源：http://fj.gzmigu.cn

C#:   Func<int, int> square = x => x * x;
来源：http://me.chemitech.net.cn

[C07] 把函数作为参数传入
来源：http://gk.muxihuayi.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hv.bjjhwx.cn

PHP:  array_map("strtoupper", $arr);
来源：http://th.muxihuayi.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mu.nicolike.cn

TS:   arr.map(String)
来源：http://fi.shxzukj.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hh.lnxyls.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ag.huixiangedu.cn

Ruby: arr.map(&:upcase)
来源：http://hd.nicolike.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://of.bookmarksfly.cn

[C08] 闭包
来源：http://gy.jianghongdianzi.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://bv.yuexingan06.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://jz.jctech888.com.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://pa.bjjhwx.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://og.9csxet.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://jz.chemitech.net.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ji.shtwfgs.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://lb.hahajie.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ja.shtwfgs.cn

[C09] 递归
来源：http://yt.muxihuayi.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://og.jianghongdianzi.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://rj.szxytkj.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wh.nszjky.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ae.shtwfgs.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://iq.colortex.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://dj.yuexingan06.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://st.bookmarksfly.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ns.shxzskj.cn

[C10] 变量作用域
来源：http://my.hnjuh.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ik.huanxung.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://kq.chemitech.net.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ba.shtwfgs.cn

TS:   同 JS
来源：http://lj.bookmarksfly.cn

Java: 方法内为块级作用域
来源：http://fq.huixinmuqiang.cn

Go:   花括号块级作用域
来源：http://xq.9csxet.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://vg.521024.cn

C#:   块级作用域
来源：http://pf.yuntaijiaju.cn

[C11] 模块导入与导出
来源：http://kr.521024.cn

Py:   from module import func
来源：http://pi.muxihuayi.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://gb.szxytkj.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://pu.yuntaijiaju.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://zz.shtwfgs.cn

Java: import java.util.List;
来源：http://pl.nicolike.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ik.bjjhwx.cn

Ruby: require "json"; require_relative "./util"
来源：http://ot.huixinmuqiang.cn

C#:   using System.Text;
来源：http://ez.muxihuayi.cn

[C12] 立即执行函数 IIFE
来源：http://vo.9csxet.cn

Py:   (lambda: print("run"))()
来源：http://sc.haigaiapp.cn

PHP:  (function () { echo "run"; })();
来源：http://fp.yuexingan06.cn

JS:   (() => { console.log("run"); })();
来源：http://qt.huixinmuqiang.cn

TS:   (() => { console.log("run"); })();
来源：http://jg.wgjwhj.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://gb.huanxung.cn

Go:   func() { fmt.Println("run") }()
来源：http://gl.colortex.cn

Ruby: -> { puts "run" }.call
来源：http://dq.jianghongdianzi.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://iz.szxytkj.cn

[C13] 类型声明 / 类型注解
来源：http://pg.9csxet.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://zf.gzmigu.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://yr.hnjuh.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://sk.panjiajie.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://sy.gzmigu.cn

Java: int add(int a, int b) { return a + b; }
来源：http://be.jianghongdianzi.cn

Go:   func add(a, b int) int
来源：http://bn.gzmigu.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ld.hnjuh.cn

C#:   int Add(int a, int b) => a + b;
来源：http://gf.9csxet.cn

[C14] 泛型函数
来源：http://xf.muxihuayi.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://vi.huixiangedu.cn

PHP:  // 无泛型
来源：http://uj.huixinmuqiang.cn

JS:   // 无泛型
来源：http://eg.haigaiapp.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://gr.chemitech.net.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://vw.hahajie.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mq.muxihuayi.cn

Ruby: # 无泛型
来源：http://nz.yuexingan06.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://gn.wgjwhj.cn

[C15] 解构 / 展开参数
来源：http://sl.szsharing.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ul.szsharing.cn

PHP:  [$a, $b] = $pair;
来源：http://jt.szxytkj.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://sv.lnxyls.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ok.huixiangedu.cn

Java: // 无解构
来源：http://bz.nicolike.cn

Go:   // 无解构
来源：http://yg.lnxyls.cn

Ruby: a, b = pair
来源：http://mn.shxzskj.cn

C#:   var (a, b) = pair;
来源：http://jd.nszjky.cn

[C16] 函数 / 方法重载
来源：http://cz.lnxyls.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hy.bookmarksfly.cn

PHP:  // 无重载
来源：http://nw.szsharing.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://at.chemitech.net.cn

TS:   // 用联合类型或重载签名声明
来源：http://kz.hnjuh.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://mk.szsharing.cn

Go:   // 无重载：用不同函数名
来源：http://nl.haigaiapp.cn

Ruby: # 无重载：靠动态参数
来源：http://tk.shxzskj.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://bs.yuntaijiaju.cn

================================================================================
来源：http://dg.yuntaijiaju.cn

D. 数组 / 列表 / 集合
来源：http://yu.lnxyls.cn

================================================================================
来源：http://il.bjjhwx.cn

[D01] 创建数组 / 列表
来源：http://mo.shtwfgs.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://tb.521024.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://oy.yuntaijiaju.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://er.shtwfgs.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://dp.shxzskj.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://gz.muxihuayi.cn


<!-- 参考信息 -->