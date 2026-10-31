代发 wailian999

[B01] 条件判断 if / else
来源：http://sq.newstarts.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://rr.huixiangedu.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ew.521024.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://gw.newstarts.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://fc.nszjky.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://it.bjjhwx.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://iy.panjiajie.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://rb.wgjwhj.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ul.szsharing.cn

[B02] 多分支 else if / elif
来源：http://fw.9csxet.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://gw.hahajie.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ap.nicolike.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://br.nicolike.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sl.jctech888.com.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://af.shxzukj.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://oh.9csxet.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://cl.wgjwhj.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fc.panjiajie.cn

[B03] switch / match / case
来源：http://gr.nicolike.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://uu.nicolike.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://fv.nicolike.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://aq.nszjky.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://kz.asd995.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://dk.haigaiapp.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://xp.lnxyls.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://mg.nszjky.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://of.huixiangedu.cn

[B04] for 计数循环
来源：http://ip.jianghongdianzi.cn

Py:   for i in range(10): print(i)
来源：http://fd.shxzukj.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://dx.hnjuh.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://he.colortex.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://gd.nicolike.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://pq.lnxyls.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://dx.jianghongdianzi.cn

Ruby: 10.times { |i| puts i }
来源：http://uo.newstarts.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://oz.szsharing.cn

[B05] 遍历数组 / 列表
来源：http://ab.bookmarksfly.cn

Py:   for item in arr: print(item)
来源：http://wx.panjiajie.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://bz.asd995.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://qg.hnjuh.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ll.bjjhwx.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://yv.bjjhwx.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://nz.hnjuh.cn

Ruby: arr.each { |item| puts item }
来源：http://sz.521024.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://qu.9csxet.cn

[B06] 遍历字典 / 对象
来源：http://pl.bjjhwx.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://jn.colortex.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wv.haigaiapp.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://lz.colortex.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://dh.shxzukj.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://fh.huixinmuqiang.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://tq.521024.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ih.shxzskj.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://gn.szsharing.cn

[B07] while 循环
来源：http://gt.shxzukj.cn

Py:   while i < 10: i += 1
来源：http://ag.shxzskj.cn

PHP:  while ($i < 10) { $i++; }
来源：http://eo.nszjky.cn

JS:   while (i < 10) { i++; }
来源：http://sn.yuexingan06.cn

TS:   while (i < 10) { i++; }
来源：http://iv.szxytkj.cn

Java: while (i < 10) { i++; }
来源：http://qv.lnxyls.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://pk.chemitech.net.cn

Ruby: while i < 10; i += 1; end
来源：http://yv.bjjhwx.cn

C#:   while (i < 10) { i++; }
来源：http://ga.hnjuh.cn

[B08] do-while（至少执行一次）
来源：http://ti.chemitech.net.cn

Py:   # 无 do-while：用 while True + break
来源：http://dv.shxzskj.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ql.szsharing.cn

JS:   do { i++; } while (i < 10);
来源：http://yd.bookmarksfly.cn

TS:   do { i++; } while (i < 10);
来源：http://pa.szxytkj.cn

Java: do { i++; } while (i < 10);
来源：http://fy.bookmarksfly.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://ac.huixiangedu.cn

Ruby: begin; i += 1; end while i < 10
来源：http://aj.nicolike.cn

C#:   do { i++; } while (i < 10);
来源：http://ni.jianghongdianzi.cn

[B09] break 与 continue
来源：http://sw.asd995.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://bx.yuntaijiaju.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://lx.bjjhwx.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bb.gzmigu.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pd.shxzskj.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kh.colortex.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://fm.colortex.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://or.jctech888.com.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mb.bjjhwx.cn

[B10] 遍历同时拿索引
来源：http://si.9csxet.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://rd.szsharing.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://rq.nicolike.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://yd.shxzskj.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://tr.jctech888.com.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://oh.9csxet.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wr.nszjky.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://jq.shxzskj.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://qz.shxzukj.cn

[B11] 生成数字序列 / 区间
来源：http://ep.yuntaijiaju.cn

Py:   list(range(0, 10, 2))
来源：http://ox.nicolike.cn

PHP:  range(0, 10, 2);
来源：http://qd.haigaiapp.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://jb.521024.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ep.yuntaijiaju.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://zp.bookmarksfly.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://lm.huixiangedu.cn

Ruby: (0...10).step(2).to_a
来源：http://jn.szsharing.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://vr.huixiangedu.cn

[B12] 跳出多层循环
来源：http://px.nszjky.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://xf.9csxet.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://bd.shxzukj.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://dm.newstarts.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://nv.lnxyls.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ar.nszjky.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://fr.wgjwhj.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mi.szxytkj.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://eh.szxytkj.cn

[B13] 判断是否为数字
来源：http://ki.huixiangedu.cn

Py:   isinstance(x, (int, float))
来源：http://kn.nszjky.cn

PHP:  is_numeric($x)
来源：http://gg.szsharing.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://gd.huixinmuqiang.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://iq.521024.cn

Java: x instanceof Number
来源：http://yr.huanxung.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://kz.shxzukj.cn

Ruby: x.is_a?(Numeric)
来源：http://jh.bjjhwx.cn

C#:   x is int or double or decimal
来源：http://lo.newstarts.cn

[B14] 判断值是否在集合内
来源：http://ow.huixiangedu.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://gz.huanxung.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://pk.hahajie.cn

JS:   [1, 2, 3].includes(x)
来源：http://ll.shxzukj.cn

TS:   [1, 2, 3].includes(x)
来源：http://bi.jianghongdianzi.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://hr.wgjwhj.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ls.shxzskj.cn

Ruby: [1, 2, 3].include?(x)
来源：http://nm.yuexingan06.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mg.bjjhwx.cn

[B15] 布尔运算与取反
来源：http://vu.haigaiapp.cn

Py:   a and b or not c
来源：http://ca.nszjky.cn

PHP:  $a && $b || !$c
来源：http://ns.yuntaijiaju.cn

JS:   a && b || !c
来源：http://kb.jctech888.com.cn

TS:   a && b || !c
来源：http://nv.szsharing.cn

Java: a && b || !c
来源：http://lm.bookmarksfly.cn

Go:   a && b || !c
来源：http://zv.panjiajie.cn

Ruby: a && b || !c
来源：http://mr.huixinmuqiang.cn

C#:   a && b || !c
来源：http://zh.hnjuh.cn

[B16] 卫语句：不满足条件提前返回
来源：http://nu.bjjhwx.cn

Py:   if not data: return
来源：http://iz.asd995.cn

PHP:  if (!$data) { return; }
来源：http://ee.9csxet.cn

JS:   if (!data) return;
来源：http://nz.lnxyls.cn

TS:   if (!data) return;
来源：http://ej.szsharing.cn

Java: if (data == null) return;
来源：http://pg.bookmarksfly.cn

Go:   if data == nil { return }
来源：http://de.jctech888.com.cn

Ruby: return if data.nil?
来源：http://xz.hahajie.cn

C#:   if (data == null) return;
来源：http://rt.shxzskj.cn

================================================================================
来源：http://qn.szsharing.cn

C. 函数与作用域
来源：http://ne.muxihuayi.cn

================================================================================
来源：http://fi.shxzskj.cn

[C01] 定义函数
来源：http://pf.jianghongdianzi.cn

Py:   def add(a, b): return a + b
来源：http://ek.yuntaijiaju.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://id.huixiangedu.cn

JS:   function add(a, b) { return a + b; }
来源：http://rc.bjjhwx.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jz.muxihuayi.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://hi.521024.cn

Go:   func add(a, b int) int { return a + b }
来源：http://td.nszjky.cn

Ruby: def add(a, b); a + b; end
来源：http://lk.gzmigu.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://al.bookmarksfly.cn

[C02] 默认参数
来源：http://pj.newstarts.cn

Py:   def greet(name="World"): return name
来源：http://kf.muxihuayi.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://fk.jianghongdianzi.cn

JS:   function greet(name = "World") { return name; }
来源：http://xq.panjiajie.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://mx.asd995.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://kw.hnjuh.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://om.gzmigu.cn

Ruby: def greet(name = "World") = name
来源：http://uf.jianghongdianzi.cn

C#:   string Greet(string name = "World") => name;
来源：http://qa.newstarts.cn

[C03] 可变参数
来源：http://og.nicolike.cn

Py:   def total(*args): return sum(args)
来源：http://qu.bookmarksfly.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://dz.szsharing.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://zb.yuntaijiaju.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://sg.lnxyls.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ng.yuexingan06.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://np.asd995.cn

Ruby: def total(*nums); nums.sum; end
来源：http://br.huixiangedu.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://bc.521024.cn

[C04] 命名参数 / 关键字参数
来源：http://bb.nszjky.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://qm.colortex.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://vc.521024.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://xo.9csxet.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://zy.muxihuayi.cn

Java: // 无：用 Builder 模式或 record
来源：http://uj.chemitech.net.cn

Go:   // 无：用配置结构体参数
来源：http://qm.9csxet.cn

Ruby: f(a: 1, b: 2)
来源：http://sx.yuexingan06.cn

C#:   f(a: 1, b: 2)
来源：http://ym.shxzskj.cn

[C05] 返回多个值
来源：http://qv.shxzukj.cn

Py:   return a, b
来源：http://ac.panjiajie.cn

PHP:  return [$a, $b];
来源：http://nw.yuexingan06.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://pc.szsharing.cn

TS:   return { a, b };
来源：http://gv.yuexingan06.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://yy.gzmigu.cn

Go:   return a, b
来源：http://cf.nicolike.cn

Ruby: return a, b
来源：http://uz.shtwfgs.cn

C#:   return (a, b);              // ValueTuple
来源：http://ms.nszjky.cn

[C06] 匿名函数 / lambda
来源：http://ml.szsharing.cn

Py:   square = lambda x: x * x
来源：http://kk.hahajie.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://za.shxzukj.cn

JS:   const square = x => x * x;
来源：http://bp.haigaiapp.cn

TS:   const square = (x: number): number => x * x;
来源：http://vf.chemitech.net.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://bk.muxihuayi.cn

Go:   sq := func(x int) int { return x * x }
来源：http://jh.shxzskj.cn

Ruby: square = ->(x) { x * x }
来源：http://aa.szsharing.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ux.asd995.cn

[C07] 把函数作为参数传入
来源：http://hf.shxzskj.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://he.shxzskj.cn

PHP:  array_map("strtoupper", $arr);
来源：http://zt.colortex.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://oe.hahajie.cn

TS:   arr.map(String)
来源：http://yk.panjiajie.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://pz.nicolike.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://pf.gzmigu.cn

Ruby: arr.map(&:upcase)
来源：http://vg.hahajie.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://na.9csxet.cn

[C08] 闭包
来源：http://qt.szxytkj.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ch.panjiajie.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://uo.bjjhwx.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://tq.hnjuh.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://zk.shxzukj.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://zo.shxzskj.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://oz.szsharing.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://zw.chemitech.net.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://xy.shxzskj.cn

[C09] 递归
来源：http://ak.huixinmuqiang.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://kq.huanxung.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ea.yuntaijiaju.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://rd.szsharing.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://db.521024.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://fb.huixiangedu.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://us.chemitech.net.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://he.wgjwhj.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://qr.muxihuayi.cn

[C10] 变量作用域
来源：http://tf.wgjwhj.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://jj.szsharing.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://fq.bookmarksfly.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://xr.bjjhwx.cn

TS:   同 JS
来源：http://uq.szxytkj.cn

Java: 方法内为块级作用域
来源：http://ux.lnxyls.cn

Go:   花括号块级作用域
来源：http://ot.szxytkj.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wi.bookmarksfly.cn

C#:   块级作用域
来源：http://gq.shxzskj.cn

[C11] 模块导入与导出
来源：http://fj.chemitech.net.cn

Py:   from module import func
来源：http://kf.lnxyls.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://ai.huixinmuqiang.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://hf.bjjhwx.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://nv.szxytkj.cn

Java: import java.util.List;
来源：http://lc.szxytkj.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://aj.chemitech.net.cn

Ruby: require "json"; require_relative "./util"
来源：http://en.lnxyls.cn

C#:   using System.Text;
来源：http://pl.chemitech.net.cn

[C12] 立即执行函数 IIFE
来源：http://bo.szsharing.cn

Py:   (lambda: print("run"))()
来源：http://ju.colortex.cn

PHP:  (function () { echo "run"; })();
来源：http://be.hnjuh.cn

JS:   (() => { console.log("run"); })();
来源：http://em.lnxyls.cn

TS:   (() => { console.log("run"); })();
来源：http://tu.asd995.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://sf.shxzskj.cn

Go:   func() { fmt.Println("run") }()
来源：http://pi.gzmigu.cn

Ruby: -> { puts "run" }.call
来源：http://to.wgjwhj.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://cj.jianghongdianzi.cn

[C13] 类型声明 / 类型注解
来源：http://qu.wgjwhj.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://kp.nicolike.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://lb.hnjuh.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://eo.lnxyls.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ja.asd995.cn

Java: int add(int a, int b) { return a + b; }
来源：http://ab.hnjuh.cn

Go:   func add(a, b int) int
来源：http://lv.haigaiapp.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ua.haigaiapp.cn

C#:   int Add(int a, int b) => a + b;
来源：http://ai.wgjwhj.cn

[C14] 泛型函数
来源：http://pz.shtwfgs.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://xf.panjiajie.cn

PHP:  // 无泛型
来源：http://hg.asd995.cn

JS:   // 无泛型
来源：http://nn.szsharing.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://yr.nszjky.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ny.jctech888.com.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://kw.huanxung.cn

Ruby: # 无泛型
来源：http://gh.shxzukj.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wu.hnjuh.cn

[C15] 解构 / 展开参数
来源：http://lx.panjiajie.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://vr.szsharing.cn

PHP:  [$a, $b] = $pair;
来源：http://me.hahajie.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wz.colortex.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ft.nszjky.cn

Java: // 无解构
来源：http://du.nicolike.cn

Go:   // 无解构
来源：http://kr.shxzukj.cn

Ruby: a, b = pair
来源：http://fq.gzmigu.cn

C#:   var (a, b) = pair;
来源：http://gw.colortex.cn

[C16] 函数 / 方法重载
来源：http://lj.gzmigu.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://kk.shxzskj.cn

PHP:  // 无重载
来源：http://iu.gzmigu.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://rm.chemitech.net.cn

TS:   // 用联合类型或重载签名声明
来源：http://ad.hnjuh.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://oz.bjjhwx.cn

Go:   // 无重载：用不同函数名
来源：http://rr.panjiajie.cn

Ruby: # 无重载：靠动态参数
来源：http://yp.jianghongdianzi.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ra.nszjky.cn

================================================================================
来源：http://mb.521024.cn

D. 数组 / 列表 / 集合
来源：http://yv.jctech888.com.cn

================================================================================
来源：http://yf.haigaiapp.cn

[D01] 创建数组 / 列表
来源：http://fb.huixinmuqiang.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://gb.521024.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://vu.haigaiapp.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://rk.haigaiapp.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://os.nicolike.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://kt.panjiajie.cn


<!-- 参考信息 -->