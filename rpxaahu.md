代发 wailian999

[A26] 类型转换总览
来源：http://sd.newstarts.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ez.nszjky.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://lk.nszjky.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://vq.bjjhwx.cn

TS:   Number() String() Boolean() x as number
来源：http://db.asd995.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://zj.yuntaijiaju.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://zt.shxzskj.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://gm.wgjwhj.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://xz.wgjwhj.cn

================================================================================
来源：http://pc.wgjwhj.cn

B. 流程控制
来源：http://tm.panjiajie.cn

================================================================================
来源：http://vx.huanxung.cn

[B01] 条件判断 if / else
来源：http://zo.9csxet.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://aw.huanxung.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ay.nszjky.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ra.shxzskj.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://gq.haigaiapp.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://qt.colortex.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://eh.hahajie.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://xq.jctech888.com.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://fc.wgjwhj.cn

[B02] 多分支 else if / elif
来源：http://wd.newstarts.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://pf.shtwfgs.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://we.jctech888.com.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yq.hnjuh.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ze.newstarts.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rw.bjjhwx.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://nz.nszjky.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://vu.9csxet.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dp.9csxet.cn

[B03] switch / match / case
来源：http://nw.shtwfgs.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://sr.bookmarksfly.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://iv.nicolike.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://kl.bookmarksfly.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://yj.huixinmuqiang.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://sy.colortex.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hu.bjjhwx.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ot.wgjwhj.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ps.colortex.cn

[B04] for 计数循环
来源：http://ci.muxihuayi.cn

Py:   for i in range(10): print(i)
来源：http://ym.hnjuh.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://go.yuntaijiaju.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://na.yuexingan06.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://kz.szxytkj.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://pl.panjiajie.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://jd.panjiajie.cn

Ruby: 10.times { |i| puts i }
来源：http://oy.9csxet.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://yj.nszjky.cn

[B05] 遍历数组 / 列表
来源：http://ev.panjiajie.cn

Py:   for item in arr: print(item)
来源：http://ob.gzmigu.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://xl.shxzskj.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://kh.newstarts.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://or.haigaiapp.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://sa.szxytkj.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wi.haigaiapp.cn

Ruby: arr.each { |item| puts item }
来源：http://sr.bookmarksfly.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://vg.panjiajie.cn

[B06] 遍历字典 / 对象
来源：http://fa.huixiangedu.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://lm.shtwfgs.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://xf.yuntaijiaju.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://zs.bjjhwx.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ce.muxihuayi.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://di.szxytkj.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://nz.shtwfgs.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ul.nicolike.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://my.521024.cn

[B07] while 循环
来源：http://iv.9csxet.cn

Py:   while i < 10: i += 1
来源：http://gd.wgjwhj.cn

PHP:  while ($i < 10) { $i++; }
来源：http://nt.huixiangedu.cn

JS:   while (i < 10) { i++; }
来源：http://xk.haigaiapp.cn

TS:   while (i < 10) { i++; }
来源：http://em.shxzukj.cn

Java: while (i < 10) { i++; }
来源：http://hb.nszjky.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ep.bjjhwx.cn

Ruby: while i < 10; i += 1; end
来源：http://gd.nszjky.cn

C#:   while (i < 10) { i++; }
来源：http://ww.nszjky.cn

[B08] do-while（至少执行一次）
来源：http://qa.hnjuh.cn

Py:   # 无 do-while：用 while True + break
来源：http://mi.asd995.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://dp.hnjuh.cn

JS:   do { i++; } while (i < 10);
来源：http://ii.521024.cn

TS:   do { i++; } while (i < 10);
来源：http://un.yuntaijiaju.cn

Java: do { i++; } while (i < 10);
来源：http://ln.huanxung.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://jd.jianghongdianzi.cn

Ruby: begin; i += 1; end while i < 10
来源：http://zt.bookmarksfly.cn

C#:   do { i++; } while (i < 10);
来源：http://ce.521024.cn

[B09] break 与 continue
来源：http://ds.newstarts.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://jm.huixinmuqiang.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://nm.shtwfgs.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://iu.asd995.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ms.newstarts.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://et.bookmarksfly.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://sn.hahajie.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mp.lnxyls.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vw.521024.cn

[B10] 遍历同时拿索引
来源：http://cc.yuntaijiaju.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://kj.shxzskj.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ti.yuntaijiaju.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ip.szsharing.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://vt.nicolike.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://sz.shxzskj.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://up.asd995.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hb.szsharing.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mw.szsharing.cn

[B11] 生成数字序列 / 区间
来源：http://cg.shxzukj.cn

Py:   list(range(0, 10, 2))
来源：http://xj.huanxung.cn

PHP:  range(0, 10, 2);
来源：http://mj.yuntaijiaju.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wl.nszjky.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://lp.nszjky.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://rw.huixinmuqiang.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://vo.shxzukj.cn

Ruby: (0...10).step(2).to_a
来源：http://sk.shxzukj.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mk.jianghongdianzi.cn

[B12] 跳出多层循环
来源：http://jl.yuntaijiaju.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://rz.yuexingan06.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://jb.shxzukj.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://cu.lnxyls.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://qs.nszjky.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://gk.wgjwhj.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://uw.huanxung.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://sp.wgjwhj.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://fx.jianghongdianzi.cn

[B13] 判断是否为数字
来源：http://uz.chemitech.net.cn

Py:   isinstance(x, (int, float))
来源：http://ah.panjiajie.cn

PHP:  is_numeric($x)
来源：http://fy.hahajie.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://dp.gzmigu.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ko.yuexingan06.cn

Java: x instanceof Number
来源：http://pc.yuntaijiaju.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://lq.huixinmuqiang.cn

Ruby: x.is_a?(Numeric)
来源：http://ko.521024.cn

C#:   x is int or double or decimal
来源：http://bv.jctech888.com.cn

[B14] 判断值是否在集合内
来源：http://kh.yuntaijiaju.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://zv.bjjhwx.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://sn.hnjuh.cn

JS:   [1, 2, 3].includes(x)
来源：http://rg.szxytkj.cn

TS:   [1, 2, 3].includes(x)
来源：http://zb.bookmarksfly.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://md.muxihuayi.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://du.jianghongdianzi.cn

Ruby: [1, 2, 3].include?(x)
来源：http://cl.muxihuayi.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://cm.shtwfgs.cn

[B15] 布尔运算与取反
来源：http://zj.bjjhwx.cn

Py:   a and b or not c
来源：http://ft.colortex.cn

PHP:  $a && $b || !$c
来源：http://tc.bjjhwx.cn

JS:   a && b || !c
来源：http://aq.huixiangedu.cn

TS:   a && b || !c
来源：http://pn.szxytkj.cn

Java: a && b || !c
来源：http://dd.shxzukj.cn

Go:   a && b || !c
来源：http://dd.521024.cn

Ruby: a && b || !c
来源：http://gl.bookmarksfly.cn

C#:   a && b || !c
来源：http://dc.bjjhwx.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ui.colortex.cn

Py:   if not data: return
来源：http://ka.hahajie.cn

PHP:  if (!$data) { return; }
来源：http://wt.wgjwhj.cn

JS:   if (!data) return;
来源：http://pk.panjiajie.cn

TS:   if (!data) return;
来源：http://po.shtwfgs.cn

Java: if (data == null) return;
来源：http://ul.huixinmuqiang.cn

Go:   if data == nil { return }
来源：http://ob.9csxet.cn

Ruby: return if data.nil?
来源：http://it.szxytkj.cn

C#:   if (data == null) return;
来源：http://nw.nszjky.cn

================================================================================
来源：http://ki.shxzskj.cn

C. 函数与作用域
来源：http://ni.shxzukj.cn

================================================================================
来源：http://ii.newstarts.cn

[C01] 定义函数
来源：http://kl.lnxyls.cn

Py:   def add(a, b): return a + b
来源：http://pr.yuntaijiaju.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://rs.lnxyls.cn

JS:   function add(a, b) { return a + b; }
来源：http://sg.jctech888.com.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://kn.haigaiapp.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://px.lnxyls.cn

Go:   func add(a, b int) int { return a + b }
来源：http://fy.haigaiapp.cn

Ruby: def add(a, b); a + b; end
来源：http://xq.panjiajie.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mp.huixinmuqiang.cn

[C02] 默认参数
来源：http://vu.nicolike.cn

Py:   def greet(name="World"): return name
来源：http://kq.chemitech.net.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://bz.szsharing.cn

JS:   function greet(name = "World") { return name; }
来源：http://zc.bookmarksfly.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ll.hnjuh.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://iy.panjiajie.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://nn.yuexingan06.cn

Ruby: def greet(name = "World") = name
来源：http://rm.shxzskj.cn

C#:   string Greet(string name = "World") => name;
来源：http://ma.muxihuayi.cn

[C03] 可变参数
来源：http://vj.nicolike.cn

Py:   def total(*args): return sum(args)
来源：http://cd.muxihuayi.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://kh.lnxyls.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://pq.bjjhwx.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://sg.panjiajie.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://id.jctech888.com.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://pr.bjjhwx.cn

Ruby: def total(*nums); nums.sum; end
来源：http://er.wgjwhj.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://fj.lnxyls.cn

[C04] 命名参数 / 关键字参数
来源：http://vq.wgjwhj.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://cy.jctech888.com.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ub.shxzukj.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://kl.gzmigu.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://tc.bookmarksfly.cn

Java: // 无：用 Builder 模式或 record
来源：http://de.jianghongdianzi.cn

Go:   // 无：用配置结构体参数
来源：http://vo.wgjwhj.cn

Ruby: f(a: 1, b: 2)
来源：http://qa.shxzukj.cn

C#:   f(a: 1, b: 2)
来源：http://ls.lnxyls.cn

[C05] 返回多个值
来源：http://nz.shxzukj.cn

Py:   return a, b
来源：http://wq.hahajie.cn

PHP:  return [$a, $b];
来源：http://la.jctech888.com.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ns.muxihuayi.cn

TS:   return { a, b };
来源：http://lm.hahajie.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://gl.szsharing.cn

Go:   return a, b
来源：http://xm.521024.cn

Ruby: return a, b
来源：http://op.nszjky.cn

C#:   return (a, b);              // ValueTuple
来源：http://eb.jianghongdianzi.cn

[C06] 匿名函数 / lambda
来源：http://te.yuntaijiaju.cn

Py:   square = lambda x: x * x
来源：http://dl.jctech888.com.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://tb.chemitech.net.cn

JS:   const square = x => x * x;
来源：http://bl.gzmigu.cn

TS:   const square = (x: number): number => x * x;
来源：http://re.chemitech.net.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://em.asd995.cn

Go:   sq := func(x int) int { return x * x }
来源：http://op.shtwfgs.cn

Ruby: square = ->(x) { x * x }
来源：http://jz.bookmarksfly.cn

C#:   Func<int, int> square = x => x * x;
来源：http://sf.jianghongdianzi.cn

[C07] 把函数作为参数传入
来源：http://hc.lnxyls.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://vo.nicolike.cn

PHP:  array_map("strtoupper", $arr);
来源：http://oh.shtwfgs.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://nd.chemitech.net.cn

TS:   arr.map(String)
来源：http://dm.521024.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://nm.muxihuayi.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ly.huanxung.cn

Ruby: arr.map(&:upcase)
来源：http://am.bookmarksfly.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://av.jianghongdianzi.cn

[C08] 闭包
来源：http://bd.huanxung.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ny.yuntaijiaju.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hy.shtwfgs.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wj.jianghongdianzi.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hn.yuntaijiaju.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ug.jianghongdianzi.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://up.nicolike.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ls.newstarts.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://jc.shxzukj.cn

[C09] 递归
来源：http://vd.colortex.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://vi.muxihuayi.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://gm.colortex.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://xl.jctech888.com.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://kp.shxzskj.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://bl.haigaiapp.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://pn.asd995.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://nl.colortex.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://qy.shtwfgs.cn

[C10] 变量作用域
来源：http://ux.lnxyls.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://qs.hahajie.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://pk.nszjky.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mc.jctech888.com.cn

TS:   同 JS
来源：http://tu.9csxet.cn

Java: 方法内为块级作用域
来源：http://ub.szsharing.cn

Go:   花括号块级作用域
来源：http://xy.haigaiapp.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ao.asd995.cn

C#:   块级作用域
来源：http://rm.shtwfgs.cn

[C11] 模块导入与导出
来源：http://ri.nicolike.cn

Py:   from module import func
来源：http://wo.szsharing.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://az.lnxyls.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://ee.jianghongdianzi.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ds.asd995.cn

Java: import java.util.List;
来源：http://bb.newstarts.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://fp.asd995.cn

Ruby: require "json"; require_relative "./util"
来源：http://uk.521024.cn

C#:   using System.Text;
来源：http://vl.haigaiapp.cn

[C12] 立即执行函数 IIFE
来源：http://gk.colortex.cn

Py:   (lambda: print("run"))()
来源：http://ts.panjiajie.cn

PHP:  (function () { echo "run"; })();
来源：http://fc.gzmigu.cn

JS:   (() => { console.log("run"); })();
来源：http://to.521024.cn

TS:   (() => { console.log("run"); })();
来源：http://kb.nicolike.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ly.nszjky.cn

Go:   func() { fmt.Println("run") }()
来源：http://pl.9csxet.cn

Ruby: -> { puts "run" }.call
来源：http://rp.bookmarksfly.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://kv.hahajie.cn

[C13] 类型声明 / 类型注解
来源：http://xt.bjjhwx.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://zh.newstarts.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://op.asd995.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://qw.szsharing.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ry.lnxyls.cn

Java: int add(int a, int b) { return a + b; }
来源：http://qi.muxihuayi.cn

Go:   func add(a, b int) int
来源：http://si.huanxung.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://cc.9csxet.cn

C#:   int Add(int a, int b) => a + b;
来源：http://jx.huanxung.cn

[C14] 泛型函数
来源：http://dn.lnxyls.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://sy.huixinmuqiang.cn

PHP:  // 无泛型
来源：http://hx.panjiajie.cn

JS:   // 无泛型
来源：http://rs.hnjuh.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wl.huanxung.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://vr.jianghongdianzi.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://eb.szxytkj.cn

Ruby: # 无泛型
来源：http://yk.lnxyls.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://jv.lnxyls.cn

[C15] 解构 / 展开参数
来源：http://us.jctech888.com.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://yo.szxytkj.cn

PHP:  [$a, $b] = $pair;
来源：http://xr.newstarts.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://di.chemitech.net.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://aa.panjiajie.cn

Java: // 无解构
来源：http://ae.jctech888.com.cn

Go:   // 无解构
来源：http://ca.huanxung.cn

Ruby: a, b = pair
来源：http://ls.nicolike.cn

C#:   var (a, b) = pair;
来源：http://tt.yuexingan06.cn

[C16] 函数 / 方法重载
来源：http://at.9csxet.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wi.nicolike.cn

PHP:  // 无重载
来源：http://qb.shxzukj.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://wv.gzmigu.cn

TS:   // 用联合类型或重载签名声明
来源：http://fj.bjjhwx.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://vj.nszjky.cn


<!-- 参考信息 -->