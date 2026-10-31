代发 wailian999

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ey.yuexingan06.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://zt.wgjwhj.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://hq.szsharing.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://gb.hahajie.cn

[A26] 类型转换总览
来源：http://fx.szsharing.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ox.huixinmuqiang.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://um.szxytkj.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://nw.asd995.cn

TS:   Number() String() Boolean() x as number
来源：http://bl.szsharing.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://eb.huixiangedu.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://iz.hnjuh.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://uf.asd995.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://cl.wgjwhj.cn

================================================================================
来源：http://op.nicolike.cn

B. 流程控制
来源：http://ca.szxytkj.cn

================================================================================
来源：http://jp.shxzukj.cn

[B01] 条件判断 if / else
来源：http://ut.colortex.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://dg.hnjuh.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://yb.shtwfgs.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://gx.muxihuayi.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ai.panjiajie.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ma.yuntaijiaju.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ui.yuexingan06.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://mn.chemitech.net.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://sh.haigaiapp.cn

[B02] 多分支 else if / elif
来源：http://sy.bjjhwx.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://lq.gzmigu.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://wu.yuntaijiaju.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zg.shxzskj.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://iy.nicolike.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xg.nicolike.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://td.bjjhwx.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ur.muxihuayi.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.asd995.cn

[B03] switch / match / case
来源：http://fg.colortex.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://un.jctech888.com.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://sa.hnjuh.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://nn.hahajie.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://sh.colortex.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://sf.521024.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://po.bookmarksfly.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://wk.haigaiapp.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://qw.szsharing.cn

[B04] for 计数循环
来源：http://nd.jctech888.com.cn

Py:   for i in range(10): print(i)
来源：http://pp.szxytkj.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://bz.wgjwhj.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ap.hahajie.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qb.yuntaijiaju.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://jg.chemitech.net.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://gt.hnjuh.cn

Ruby: 10.times { |i| puts i }
来源：http://hw.huixinmuqiang.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://je.wgjwhj.cn

[B05] 遍历数组 / 列表
来源：http://sy.panjiajie.cn

Py:   for item in arr: print(item)
来源：http://mr.szxytkj.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://sq.lnxyls.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ly.muxihuayi.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://xh.bookmarksfly.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://tj.szsharing.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://mq.haigaiapp.cn

Ruby: arr.each { |item| puts item }
来源：http://fs.9csxet.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ds.shtwfgs.cn

[B06] 遍历字典 / 对象
来源：http://if.shxzukj.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://bl.haigaiapp.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://yy.521024.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://yx.bjjhwx.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://rf.panjiajie.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://zl.colortex.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://zm.huixiangedu.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://uv.jctech888.com.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://pk.yuexingan06.cn

[B07] while 循环
来源：http://om.yuexingan06.cn

Py:   while i < 10: i += 1
来源：http://lp.szxytkj.cn

PHP:  while ($i < 10) { $i++; }
来源：http://dj.huixinmuqiang.cn

JS:   while (i < 10) { i++; }
来源：http://eb.haigaiapp.cn

TS:   while (i < 10) { i++; }
来源：http://zb.jianghongdianzi.cn

Java: while (i < 10) { i++; }
来源：http://xz.szxytkj.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ns.newstarts.cn

Ruby: while i < 10; i += 1; end
来源：http://ue.yuexingan06.cn

C#:   while (i < 10) { i++; }
来源：http://eo.lnxyls.cn

[B08] do-while（至少执行一次）
来源：http://mn.yuexingan06.cn

Py:   # 无 do-while：用 while True + break
来源：http://nt.muxihuayi.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://eo.szxytkj.cn

JS:   do { i++; } while (i < 10);
来源：http://md.haigaiapp.cn

TS:   do { i++; } while (i < 10);
来源：http://mz.chemitech.net.cn

Java: do { i++; } while (i < 10);
来源：http://mk.huanxung.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://hk.chemitech.net.cn

Ruby: begin; i += 1; end while i < 10
来源：http://nu.colortex.cn

C#:   do { i++; } while (i < 10);
来源：http://dc.yuexingan06.cn

[B09] break 与 continue
来源：http://ma.yuntaijiaju.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://rz.lnxyls.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://vg.haigaiapp.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qu.nicolike.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ne.jctech888.com.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vz.bookmarksfly.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://mp.huanxung.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ad.szsharing.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lm.huanxung.cn

[B10] 遍历同时拿索引
来源：http://xi.521024.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ah.panjiajie.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://fy.nicolike.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://oe.hahajie.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://dg.lnxyls.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ih.szxytkj.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://va.hnjuh.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://lp.haigaiapp.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://sy.9csxet.cn

[B11] 生成数字序列 / 区间
来源：http://bz.panjiajie.cn

Py:   list(range(0, 10, 2))
来源：http://mk.chemitech.net.cn

PHP:  range(0, 10, 2);
来源：http://gx.huixinmuqiang.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ec.jctech888.com.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mw.nszjky.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://pn.szxytkj.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://dh.wgjwhj.cn

Ruby: (0...10).step(2).to_a
来源：http://gs.yuexingan06.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://sh.szxytkj.cn

[B12] 跳出多层循环
来源：http://qz.chemitech.net.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://tp.shxzskj.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://sf.bookmarksfly.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ph.muxihuayi.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hx.szsharing.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://sv.muxihuayi.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ii.jctech888.com.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ns.shtwfgs.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://zn.huixiangedu.cn

[B13] 判断是否为数字
来源：http://si.jctech888.com.cn

Py:   isinstance(x, (int, float))
来源：http://ag.shxzukj.cn

PHP:  is_numeric($x)
来源：http://qr.hahajie.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://zn.colortex.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://oz.asd995.cn

Java: x instanceof Number
来源：http://ei.shxzskj.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://fu.szxytkj.cn

Ruby: x.is_a?(Numeric)
来源：http://kw.yuexingan06.cn

C#:   x is int or double or decimal
来源：http://xh.yuntaijiaju.cn

[B14] 判断值是否在集合内
来源：http://vi.chemitech.net.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://vj.hahajie.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ao.chemitech.net.cn

JS:   [1, 2, 3].includes(x)
来源：http://wa.wgjwhj.cn

TS:   [1, 2, 3].includes(x)
来源：http://mg.colortex.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://hg.szxytkj.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://sm.hahajie.cn

Ruby: [1, 2, 3].include?(x)
来源：http://nc.colortex.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://il.szsharing.cn

[B15] 布尔运算与取反
来源：http://ux.szsharing.cn

Py:   a and b or not c
来源：http://lz.panjiajie.cn

PHP:  $a && $b || !$c
来源：http://kl.shxzukj.cn

JS:   a && b || !c
来源：http://yy.wgjwhj.cn

TS:   a && b || !c
来源：http://fg.9csxet.cn

Java: a && b || !c
来源：http://gk.huanxung.cn

Go:   a && b || !c
来源：http://xi.hahajie.cn

Ruby: a && b || !c
来源：http://ad.shxzukj.cn

C#:   a && b || !c
来源：http://kx.huixinmuqiang.cn

[B16] 卫语句：不满足条件提前返回
来源：http://vm.chemitech.net.cn

Py:   if not data: return
来源：http://ta.521024.cn

PHP:  if (!$data) { return; }
来源：http://yv.nicolike.cn

JS:   if (!data) return;
来源：http://cj.panjiajie.cn

TS:   if (!data) return;
来源：http://ei.gzmigu.cn

Java: if (data == null) return;
来源：http://mh.shtwfgs.cn

Go:   if data == nil { return }
来源：http://mr.huixinmuqiang.cn

Ruby: return if data.nil?
来源：http://po.shtwfgs.cn

C#:   if (data == null) return;
来源：http://ly.chemitech.net.cn

================================================================================
来源：http://dw.yuntaijiaju.cn

C. 函数与作用域
来源：http://bs.huanxung.cn

================================================================================
来源：http://ja.bookmarksfly.cn

[C01] 定义函数
来源：http://xn.hahajie.cn

Py:   def add(a, b): return a + b
来源：http://zc.wgjwhj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xv.chemitech.net.cn

JS:   function add(a, b) { return a + b; }
来源：http://bn.jianghongdianzi.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://lo.huanxung.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://bh.yuexingan06.cn

Go:   func add(a, b int) int { return a + b }
来源：http://xp.muxihuayi.cn

Ruby: def add(a, b); a + b; end
来源：http://rw.jctech888.com.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://qy.asd995.cn

[C02] 默认参数
来源：http://lc.hnjuh.cn

Py:   def greet(name="World"): return name
来源：http://zi.521024.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://ed.shxzskj.cn

JS:   function greet(name = "World") { return name; }
来源：http://mu.9csxet.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://wv.colortex.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://lh.shtwfgs.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://sh.asd995.cn

Ruby: def greet(name = "World") = name
来源：http://vh.colortex.cn

C#:   string Greet(string name = "World") => name;
来源：http://rq.nicolike.cn

[C03] 可变参数
来源：http://xr.chemitech.net.cn

Py:   def total(*args): return sum(args)
来源：http://ya.9csxet.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://pt.hahajie.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://vw.521024.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wl.huanxung.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://nu.panjiajie.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mc.hnjuh.cn

Ruby: def total(*nums); nums.sum; end
来源：http://xn.huixinmuqiang.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://gw.nszjky.cn

[C04] 命名参数 / 关键字参数
来源：http://wb.nszjky.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://kl.huixinmuqiang.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ww.shxzskj.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ao.shtwfgs.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://zu.521024.cn

Java: // 无：用 Builder 模式或 record
来源：http://sn.muxihuayi.cn

Go:   // 无：用配置结构体参数
来源：http://nd.nicolike.cn

Ruby: f(a: 1, b: 2)
来源：http://up.huanxung.cn

C#:   f(a: 1, b: 2)
来源：http://hz.newstarts.cn

[C05] 返回多个值
来源：http://gn.colortex.cn

Py:   return a, b
来源：http://yl.huixinmuqiang.cn

PHP:  return [$a, $b];
来源：http://nk.shtwfgs.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://sz.wgjwhj.cn

TS:   return { a, b };
来源：http://nh.yuexingan06.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://go.jctech888.com.cn

Go:   return a, b
来源：http://kd.huixinmuqiang.cn

Ruby: return a, b
来源：http://aa.hahajie.cn

C#:   return (a, b);              // ValueTuple
来源：http://av.shxzskj.cn

[C06] 匿名函数 / lambda
来源：http://dw.muxihuayi.cn

Py:   square = lambda x: x * x
来源：http://iq.9csxet.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://kd.asd995.cn

JS:   const square = x => x * x;
来源：http://dl.newstarts.cn

TS:   const square = (x: number): number => x * x;
来源：http://ua.shxzskj.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://bm.huixinmuqiang.cn

Go:   sq := func(x int) int { return x * x }
来源：http://aj.nszjky.cn

Ruby: square = ->(x) { x * x }
来源：http://qw.muxihuayi.cn

C#:   Func<int, int> square = x => x * x;
来源：http://fm.szsharing.cn

[C07] 把函数作为参数传入
来源：http://ta.shxzskj.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ry.panjiajie.cn

PHP:  array_map("strtoupper", $arr);
来源：http://yc.huixiangedu.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://de.nszjky.cn

TS:   arr.map(String)
来源：http://be.chemitech.net.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://qu.lnxyls.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://em.huixinmuqiang.cn

Ruby: arr.map(&:upcase)
来源：http://vn.jctech888.com.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://bc.huixinmuqiang.cn

[C08] 闭包
来源：http://cy.muxihuayi.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://uh.gzmigu.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://fy.9csxet.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://qp.bjjhwx.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://nc.jianghongdianzi.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://qs.muxihuayi.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://kw.nszjky.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://te.yuntaijiaju.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://zy.nicolike.cn

[C09] 递归
来源：http://fo.9csxet.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://cv.shxzskj.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://es.yuexingan06.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://jo.haigaiapp.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://zt.chemitech.net.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://nq.muxihuayi.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://tc.colortex.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://xn.szxytkj.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://sd.bookmarksfly.cn

[C10] 变量作用域
来源：http://sv.jctech888.com.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wv.bjjhwx.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hu.yuntaijiaju.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://of.hahajie.cn

TS:   同 JS
来源：http://px.huixinmuqiang.cn

Java: 方法内为块级作用域
来源：http://hw.yuexingan06.cn

Go:   花括号块级作用域
来源：http://vk.muxihuayi.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ev.wgjwhj.cn

C#:   块级作用域
来源：http://yq.huixinmuqiang.cn

[C11] 模块导入与导出
来源：http://cy.chemitech.net.cn

Py:   from module import func
来源：http://dw.chemitech.net.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://ol.newstarts.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://oq.jianghongdianzi.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://rs.nszjky.cn

Java: import java.util.List;
来源：http://zc.nicolike.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://oz.bjjhwx.cn

Ruby: require "json"; require_relative "./util"
来源：http://ov.shxzskj.cn

C#:   using System.Text;
来源：http://cs.szsharing.cn

[C12] 立即执行函数 IIFE
来源：http://ko.jctech888.com.cn

Py:   (lambda: print("run"))()
来源：http://ak.colortex.cn

PHP:  (function () { echo "run"; })();
来源：http://jr.huixiangedu.cn

JS:   (() => { console.log("run"); })();
来源：http://ax.huixiangedu.cn

TS:   (() => { console.log("run"); })();
来源：http://eu.huanxung.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://sz.nszjky.cn

Go:   func() { fmt.Println("run") }()
来源：http://zr.hnjuh.cn

Ruby: -> { puts "run" }.call
来源：http://tz.huanxung.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://rt.gzmigu.cn

[C13] 类型声明 / 类型注解
来源：http://ue.huanxung.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://rq.yuntaijiaju.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ms.szsharing.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://kr.chemitech.net.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ci.jctech888.com.cn

Java: int add(int a, int b) { return a + b; }
来源：http://vl.bookmarksfly.cn

Go:   func add(a, b int) int
来源：http://dk.huixiangedu.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://km.bjjhwx.cn

C#:   int Add(int a, int b) => a + b;
来源：http://vs.9csxet.cn

[C14] 泛型函数
来源：http://ln.jctech888.com.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://gp.haigaiapp.cn

PHP:  // 无泛型
来源：http://go.huanxung.cn

JS:   // 无泛型
来源：http://dd.haigaiapp.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://vi.asd995.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mt.hnjuh.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://zm.huixinmuqiang.cn

Ruby: # 无泛型
来源：http://ha.jctech888.com.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://eq.bjjhwx.cn

[C15] 解构 / 展开参数
来源：http://ab.shtwfgs.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://rq.jianghongdianzi.cn

PHP:  [$a, $b] = $pair;
来源：http://ro.szxytkj.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://tt.haigaiapp.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://st.521024.cn

Java: // 无解构
来源：http://ku.panjiajie.cn

Go:   // 无解构
来源：http://il.yuntaijiaju.cn

Ruby: a, b = pair
来源：http://vj.jctech888.com.cn

C#:   var (a, b) = pair;
来源：http://st.muxihuayi.cn

[C16] 函数 / 方法重载
来源：http://tf.muxihuayi.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ff.lnxyls.cn


<!-- 参考信息 -->