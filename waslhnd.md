代发 wailian999

TS:   Number() String() Boolean() x as number
来源：http://nd.szxytkj.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://tv.chemitech.net.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ly.panjiajie.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://sx.haigaiapp.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://vk.huanxung.cn

================================================================================
来源：http://by.lnxyls.cn

B. 流程控制
来源：http://qn.szsharing.cn

================================================================================
来源：http://yh.huixiangedu.cn

[B01] 条件判断 if / else
来源：http://zo.colortex.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://ur.jianghongdianzi.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ez.shtwfgs.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ms.hahajie.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://fg.nszjky.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://hh.shxzukj.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://iq.shxzskj.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://so.bjjhwx.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://aj.yuexingan06.cn

[B02] 多分支 else if / elif
来源：http://yn.bjjhwx.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://nl.lnxyls.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://fg.panjiajie.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nk.521024.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lt.yuntaijiaju.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yf.huanxung.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://pc.newstarts.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://mc.shtwfgs.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jn.newstarts.cn

[B03] switch / match / case
来源：http://cu.hnjuh.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://qj.shxzskj.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://je.huixinmuqiang.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://pm.hnjuh.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://pk.colortex.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hh.szxytkj.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://cf.521024.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://cq.nicolike.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ax.shxzukj.cn

[B04] for 计数循环
来源：http://wa.colortex.cn

Py:   for i in range(10): print(i)
来源：http://sk.asd995.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://mn.colortex.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ff.newstarts.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://se.newstarts.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://mc.shxzukj.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://bm.panjiajie.cn

Ruby: 10.times { |i| puts i }
来源：http://qo.colortex.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://dg.szsharing.cn

[B05] 遍历数组 / 列表
来源：http://hm.shxzukj.cn

Py:   for item in arr: print(item)
来源：http://hw.colortex.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://jv.521024.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://hj.chemitech.net.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://bk.hnjuh.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://th.newstarts.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://jl.newstarts.cn

Ruby: arr.each { |item| puts item }
来源：http://dl.colortex.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ar.haigaiapp.cn

[B06] 遍历字典 / 对象
来源：http://xk.hnjuh.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://gj.521024.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ju.jianghongdianzi.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://dq.nszjky.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://vt.bookmarksfly.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://bn.521024.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://xj.panjiajie.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://lo.9csxet.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://mp.haigaiapp.cn

[B07] while 循环
来源：http://xn.hnjuh.cn

Py:   while i < 10: i += 1
来源：http://vw.bookmarksfly.cn

PHP:  while ($i < 10) { $i++; }
来源：http://sr.haigaiapp.cn

JS:   while (i < 10) { i++; }
来源：http://om.shxzskj.cn

TS:   while (i < 10) { i++; }
来源：http://es.nszjky.cn

Java: while (i < 10) { i++; }
来源：http://wc.hnjuh.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://av.shtwfgs.cn

Ruby: while i < 10; i += 1; end
来源：http://we.shxzukj.cn

C#:   while (i < 10) { i++; }
来源：http://eu.gzmigu.cn

[B08] do-while（至少执行一次）
来源：http://zd.szxytkj.cn

Py:   # 无 do-while：用 while True + break
来源：http://vq.colortex.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ha.yuntaijiaju.cn

JS:   do { i++; } while (i < 10);
来源：http://cl.haigaiapp.cn

TS:   do { i++; } while (i < 10);
来源：http://os.shxzskj.cn

Java: do { i++; } while (i < 10);
来源：http://jd.hnjuh.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://cy.gzmigu.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ww.hahajie.cn

C#:   do { i++; } while (i < 10);
来源：http://xa.wgjwhj.cn

[B09] break 与 continue
来源：http://jm.9csxet.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://kb.521024.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ih.gzmigu.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ra.jianghongdianzi.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pv.shtwfgs.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lf.jianghongdianzi.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ok.shxzskj.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://lx.jianghongdianzi.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ng.szsharing.cn

[B10] 遍历同时拿索引
来源：http://jv.haigaiapp.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wt.bookmarksfly.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://lx.jctech888.com.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://tr.jianghongdianzi.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://tx.9csxet.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ax.521024.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://xi.lnxyls.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://va.panjiajie.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ol.521024.cn

[B11] 生成数字序列 / 区间
来源：http://je.muxihuayi.cn

Py:   list(range(0, 10, 2))
来源：http://bj.panjiajie.cn

PHP:  range(0, 10, 2);
来源：http://zp.9csxet.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://jx.szxytkj.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ip.9csxet.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://pm.yuntaijiaju.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://sk.yuexingan06.cn

Ruby: (0...10).step(2).to_a
来源：http://xs.huixinmuqiang.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hw.nicolike.cn

[B12] 跳出多层循环
来源：http://ju.szsharing.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ku.yuntaijiaju.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://rz.bjjhwx.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://fr.colortex.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://sh.hahajie.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://qc.yuntaijiaju.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://gd.yuntaijiaju.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ci.huixinmuqiang.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mx.9csxet.cn

[B13] 判断是否为数字
来源：http://vg.huanxung.cn

Py:   isinstance(x, (int, float))
来源：http://io.9csxet.cn

PHP:  is_numeric($x)
来源：http://xi.newstarts.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://jp.jctech888.com.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wd.yuexingan06.cn

Java: x instanceof Number
来源：http://kz.huanxung.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://le.jianghongdianzi.cn

Ruby: x.is_a?(Numeric)
来源：http://iw.nszjky.cn

C#:   x is int or double or decimal
来源：http://xu.shxzskj.cn

[B14] 判断值是否在集合内
来源：http://sj.9csxet.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ll.jianghongdianzi.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://qj.chemitech.net.cn

JS:   [1, 2, 3].includes(x)
来源：http://hc.shtwfgs.cn

TS:   [1, 2, 3].includes(x)
来源：http://nr.huixiangedu.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://jn.colortex.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://qv.521024.cn

Ruby: [1, 2, 3].include?(x)
来源：http://zd.wgjwhj.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://lt.colortex.cn

[B15] 布尔运算与取反
来源：http://fw.yuntaijiaju.cn

Py:   a and b or not c
来源：http://gt.shxzukj.cn

PHP:  $a && $b || !$c
来源：http://zw.521024.cn

JS:   a && b || !c
来源：http://vc.chemitech.net.cn

TS:   a && b || !c
来源：http://sz.521024.cn

Java: a && b || !c
来源：http://cp.muxihuayi.cn

Go:   a && b || !c
来源：http://nf.newstarts.cn

Ruby: a && b || !c
来源：http://hs.szsharing.cn

C#:   a && b || !c
来源：http://co.bjjhwx.cn

[B16] 卫语句：不满足条件提前返回
来源：http://xc.lnxyls.cn

Py:   if not data: return
来源：http://ok.wgjwhj.cn

PHP:  if (!$data) { return; }
来源：http://jz.shxzukj.cn

JS:   if (!data) return;
来源：http://oe.szxytkj.cn

TS:   if (!data) return;
来源：http://ml.muxihuayi.cn

Java: if (data == null) return;
来源：http://yg.colortex.cn

Go:   if data == nil { return }
来源：http://it.hnjuh.cn

Ruby: return if data.nil?
来源：http://oh.chemitech.net.cn

C#:   if (data == null) return;
来源：http://ef.nszjky.cn

================================================================================
来源：http://xe.jianghongdianzi.cn

C. 函数与作用域
来源：http://lr.newstarts.cn

================================================================================
来源：http://fn.shxzskj.cn

[C01] 定义函数
来源：http://pa.yuexingan06.cn

Py:   def add(a, b): return a + b
来源：http://uh.nszjky.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ui.lnxyls.cn

JS:   function add(a, b) { return a + b; }
来源：http://ig.nszjky.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://yx.nszjky.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ix.521024.cn

Go:   func add(a, b int) int { return a + b }
来源：http://si.wgjwhj.cn

Ruby: def add(a, b); a + b; end
来源：http://lf.huixinmuqiang.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://dm.nicolike.cn

[C02] 默认参数
来源：http://tp.asd995.cn

Py:   def greet(name="World"): return name
来源：http://vl.shtwfgs.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://iw.bookmarksfly.cn

JS:   function greet(name = "World") { return name; }
来源：http://ne.haigaiapp.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://zo.nicolike.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://hi.jctech888.com.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://lq.yuntaijiaju.cn

Ruby: def greet(name = "World") = name
来源：http://hr.521024.cn

C#:   string Greet(string name = "World") => name;
来源：http://ko.huixiangedu.cn

[C03] 可变参数
来源：http://gj.huixinmuqiang.cn

Py:   def total(*args): return sum(args)
来源：http://az.bookmarksfly.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://dj.hnjuh.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ry.szsharing.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://qx.szsharing.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://oo.shtwfgs.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://qc.haigaiapp.cn

Ruby: def total(*nums); nums.sum; end
来源：http://yc.hahajie.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://qs.colortex.cn

[C04] 命名参数 / 关键字参数
来源：http://dg.521024.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ga.muxihuayi.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ke.jianghongdianzi.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wu.shxzskj.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://su.9csxet.cn

Java: // 无：用 Builder 模式或 record
来源：http://zw.haigaiapp.cn

Go:   // 无：用配置结构体参数
来源：http://mw.9csxet.cn

Ruby: f(a: 1, b: 2)
来源：http://qt.chemitech.net.cn

C#:   f(a: 1, b: 2)
来源：http://ly.huixinmuqiang.cn

[C05] 返回多个值
来源：http://il.chemitech.net.cn

Py:   return a, b
来源：http://cx.wgjwhj.cn

PHP:  return [$a, $b];
来源：http://ud.haigaiapp.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://jk.haigaiapp.cn

TS:   return { a, b };
来源：http://ep.hnjuh.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wy.chemitech.net.cn

Go:   return a, b
来源：http://fc.lnxyls.cn

Ruby: return a, b
来源：http://ui.nicolike.cn

C#:   return (a, b);              // ValueTuple
来源：http://ja.521024.cn

[C06] 匿名函数 / lambda
来源：http://ej.huixinmuqiang.cn

Py:   square = lambda x: x * x
来源：http://kv.jctech888.com.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://bw.hahajie.cn

JS:   const square = x => x * x;
来源：http://ya.nszjky.cn

TS:   const square = (x: number): number => x * x;
来源：http://gp.bookmarksfly.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://lt.huixiangedu.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ux.wgjwhj.cn

Ruby: square = ->(x) { x * x }
来源：http://ud.haigaiapp.cn

C#:   Func<int, int> square = x => x * x;
来源：http://cs.hnjuh.cn

[C07] 把函数作为参数传入
来源：http://ca.wgjwhj.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://xy.panjiajie.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ez.huanxung.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://xh.panjiajie.cn

TS:   arr.map(String)
来源：http://fo.521024.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://xf.shtwfgs.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ur.jianghongdianzi.cn

Ruby: arr.map(&:upcase)
来源：http://bd.wgjwhj.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://mw.nicolike.cn

[C08] 闭包
来源：http://lp.bjjhwx.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://js.yuntaijiaju.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://gu.521024.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://fw.newstarts.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://sj.shxzukj.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://da.shxzukj.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ja.shtwfgs.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://pb.gzmigu.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://xg.huixiangedu.cn

[C09] 递归
来源：http://vo.haigaiapp.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://qn.huixinmuqiang.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://lu.yuntaijiaju.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://cq.szxytkj.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://xj.haigaiapp.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://bm.shxzskj.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://lx.huixinmuqiang.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wd.yuexingan06.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://yi.colortex.cn

[C10] 变量作用域
来源：http://se.9csxet.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://io.haigaiapp.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://vg.nszjky.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://az.colortex.cn

TS:   同 JS
来源：http://lh.gzmigu.cn

Java: 方法内为块级作用域
来源：http://pv.521024.cn

Go:   花括号块级作用域
来源：http://wj.lnxyls.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://fg.muxihuayi.cn

C#:   块级作用域
来源：http://lr.shxzukj.cn

[C11] 模块导入与导出
来源：http://oh.jianghongdianzi.cn

Py:   from module import func
来源：http://dx.chemitech.net.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://bi.yuexingan06.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://rm.jianghongdianzi.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://av.yuexingan06.cn

Java: import java.util.List;
来源：http://qa.nszjky.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://um.huixinmuqiang.cn

Ruby: require "json"; require_relative "./util"
来源：http://rr.szxytkj.cn

C#:   using System.Text;
来源：http://jh.panjiajie.cn

[C12] 立即执行函数 IIFE
来源：http://qx.wgjwhj.cn

Py:   (lambda: print("run"))()
来源：http://lh.jianghongdianzi.cn

PHP:  (function () { echo "run"; })();
来源：http://ei.shxzskj.cn

JS:   (() => { console.log("run"); })();
来源：http://au.chemitech.net.cn

TS:   (() => { console.log("run"); })();
来源：http://mv.bjjhwx.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ak.yuexingan06.cn

Go:   func() { fmt.Println("run") }()
来源：http://ax.newstarts.cn

Ruby: -> { puts "run" }.call
来源：http://yd.lnxyls.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://px.bookmarksfly.cn

[C13] 类型声明 / 类型注解
来源：http://sd.yuntaijiaju.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://jl.newstarts.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://lr.jianghongdianzi.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://py.yuntaijiaju.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://oo.nszjky.cn

Java: int add(int a, int b) { return a + b; }
来源：http://sc.szxytkj.cn

Go:   func add(a, b int) int
来源：http://jv.shtwfgs.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ys.haigaiapp.cn

C#:   int Add(int a, int b) => a + b;
来源：http://bx.szsharing.cn

[C14] 泛型函数
来源：http://yd.nicolike.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://dd.521024.cn

PHP:  // 无泛型
来源：http://wq.panjiajie.cn

JS:   // 无泛型
来源：http://ds.521024.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://qx.bookmarksfly.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://aw.shxzukj.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://in.wgjwhj.cn

Ruby: # 无泛型
来源：http://vl.haigaiapp.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://gp.huanxung.cn

[C15] 解构 / 展开参数
来源：http://gv.jianghongdianzi.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://xq.shxzukj.cn

PHP:  [$a, $b] = $pair;
来源：http://gd.hnjuh.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://lr.szsharing.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://zh.gzmigu.cn

Java: // 无解构
来源：http://my.hahajie.cn

Go:   // 无解构
来源：http://if.huanxung.cn

Ruby: a, b = pair
来源：http://ne.shxzskj.cn

C#:   var (a, b) = pair;
来源：http://xs.hnjuh.cn

[C16] 函数 / 方法重载
来源：http://ru.shxzskj.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://az.szxytkj.cn

PHP:  // 无重载
来源：http://ac.haigaiapp.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://zq.colortex.cn

TS:   // 用联合类型或重载签名声明
来源：http://sp.gzmigu.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://ph.newstarts.cn

Go:   // 无重载：用不同函数名
来源：http://pe.wgjwhj.cn

Ruby: # 无重载：靠动态参数
来源：http://se.hnjuh.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://sa.newstarts.cn

================================================================================
来源：http://rf.bookmarksfly.cn


<!-- 参考信息 -->