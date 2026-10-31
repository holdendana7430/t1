代发 wailian999

[A26] 类型转换总览
来源：http://xk.colortex.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://vh.lnxyls.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://vf.nicolike.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://lc.jctech888.com.cn

TS:   Number() String() Boolean() x as number
来源：http://yj.szxytkj.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://uw.bookmarksfly.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ui.muxihuayi.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://ni.yuntaijiaju.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://cm.wgjwhj.cn

================================================================================
来源：http://nn.haigaiapp.cn

B. 流程控制
来源：http://on.huanxung.cn

================================================================================
来源：http://ja.lnxyls.cn

[B01] 条件判断 if / else
来源：http://jv.huanxung.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://ji.shtwfgs.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ld.nicolike.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://er.jianghongdianzi.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://xa.lnxyls.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://dz.colortex.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hl.yuexingan06.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://mt.jianghongdianzi.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://so.colortex.cn

[B02] 多分支 else if / elif
来源：http://yg.bookmarksfly.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hx.yuexingan06.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://bj.panjiajie.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zg.newstarts.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sf.muxihuayi.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gp.shxzskj.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://jx.hahajie.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://sj.muxihuayi.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xx.yuexingan06.cn

[B03] switch / match / case
来源：http://oh.hnjuh.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://qm.colortex.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://uv.nszjky.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://dj.nszjky.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hk.bookmarksfly.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://jl.szxytkj.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://zx.gzmigu.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ux.huanxung.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://fr.yuexingan06.cn

[B04] for 计数循环
来源：http://cq.wgjwhj.cn

Py:   for i in range(10): print(i)
来源：http://ul.yuntaijiaju.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://en.shxzukj.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://io.huixiangedu.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://cq.szsharing.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://xf.bookmarksfly.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://oa.lnxyls.cn

Ruby: 10.times { |i| puts i }
来源：http://mb.colortex.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://pj.huanxung.cn

[B05] 遍历数组 / 列表
来源：http://uf.huixinmuqiang.cn

Py:   for item in arr: print(item)
来源：http://xe.hnjuh.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ug.nicolike.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ak.asd995.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://kn.asd995.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://ki.haigaiapp.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ny.haigaiapp.cn

Ruby: arr.each { |item| puts item }
来源：http://mi.gzmigu.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://pk.yuntaijiaju.cn

[B06] 遍历字典 / 对象
来源：http://ae.muxihuayi.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://yc.jianghongdianzi.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://bm.chemitech.net.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://kz.colortex.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://zo.colortex.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://im.huixiangedu.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://xf.haigaiapp.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://tt.szxytkj.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://qw.gzmigu.cn

[B07] while 循环
来源：http://ks.hahajie.cn

Py:   while i < 10: i += 1
来源：http://ss.hnjuh.cn

PHP:  while ($i < 10) { $i++; }
来源：http://yn.panjiajie.cn

JS:   while (i < 10) { i++; }
来源：http://ps.huixinmuqiang.cn

TS:   while (i < 10) { i++; }
来源：http://mk.gzmigu.cn

Java: while (i < 10) { i++; }
来源：http://qp.shxzskj.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://fk.newstarts.cn

Ruby: while i < 10; i += 1; end
来源：http://gg.muxihuayi.cn

C#:   while (i < 10) { i++; }
来源：http://le.nszjky.cn

[B08] do-while（至少执行一次）
来源：http://rj.wgjwhj.cn

Py:   # 无 do-while：用 while True + break
来源：http://hy.shtwfgs.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://te.shtwfgs.cn

JS:   do { i++; } while (i < 10);
来源：http://fv.shxzskj.cn

TS:   do { i++; } while (i < 10);
来源：http://le.lnxyls.cn

Java: do { i++; } while (i < 10);
来源：http://ra.shxzskj.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://xz.szxytkj.cn

Ruby: begin; i += 1; end while i < 10
来源：http://jo.colortex.cn

C#:   do { i++; } while (i < 10);
来源：http://qh.asd995.cn

[B09] break 与 continue
来源：http://my.gzmigu.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://zn.wgjwhj.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://zw.521024.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bh.yuexingan06.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gb.asd995.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yo.521024.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://jm.hnjuh.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hs.panjiajie.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wh.yuntaijiaju.cn

[B10] 遍历同时拿索引
来源：http://fl.521024.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://fo.yuntaijiaju.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://iz.yuntaijiaju.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://uq.yuntaijiaju.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ms.gzmigu.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ys.lnxyls.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://tp.shxzskj.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://pt.9csxet.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://yn.shtwfgs.cn

[B11] 生成数字序列 / 区间
来源：http://vk.shxzukj.cn

Py:   list(range(0, 10, 2))
来源：http://xp.9csxet.cn

PHP:  range(0, 10, 2);
来源：http://co.shxzukj.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://tb.nicolike.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://cy.yuexingan06.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ob.shxzskj.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://sc.szxytkj.cn

Ruby: (0...10).step(2).to_a
来源：http://yh.huixiangedu.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://pp.szsharing.cn

[B12] 跳出多层循环
来源：http://xa.szxytkj.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://df.wgjwhj.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://lp.shxzskj.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://dr.shxzukj.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ma.shtwfgs.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://cw.asd995.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://di.hahajie.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://js.colortex.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://iw.9csxet.cn

[B13] 判断是否为数字
来源：http://dr.hnjuh.cn

Py:   isinstance(x, (int, float))
来源：http://ux.wgjwhj.cn

PHP:  is_numeric($x)
来源：http://hq.yuexingan06.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://te.huixiangedu.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://iv.asd995.cn

Java: x instanceof Number
来源：http://pc.bookmarksfly.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ew.shtwfgs.cn

Ruby: x.is_a?(Numeric)
来源：http://to.jctech888.com.cn

C#:   x is int or double or decimal
来源：http://un.newstarts.cn

[B14] 判断值是否在集合内
来源：http://fv.9csxet.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://vy.szxytkj.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://sa.huanxung.cn

JS:   [1, 2, 3].includes(x)
来源：http://ed.jctech888.com.cn

TS:   [1, 2, 3].includes(x)
来源：http://pi.hahajie.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://jc.shxzskj.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://pd.nicolike.cn

Ruby: [1, 2, 3].include?(x)
来源：http://aa.nicolike.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://cl.hahajie.cn

[B15] 布尔运算与取反
来源：http://bd.jctech888.com.cn

Py:   a and b or not c
来源：http://sa.wgjwhj.cn

PHP:  $a && $b || !$c
来源：http://yi.9csxet.cn

JS:   a && b || !c
来源：http://xw.chemitech.net.cn

TS:   a && b || !c
来源：http://co.huanxung.cn

Java: a && b || !c
来源：http://oj.yuntaijiaju.cn

Go:   a && b || !c
来源：http://er.huanxung.cn

Ruby: a && b || !c
来源：http://mt.gzmigu.cn

C#:   a && b || !c
来源：http://qx.wgjwhj.cn

[B16] 卫语句：不满足条件提前返回
来源：http://so.bjjhwx.cn

Py:   if not data: return
来源：http://wu.nszjky.cn

PHP:  if (!$data) { return; }
来源：http://kn.jctech888.com.cn

JS:   if (!data) return;
来源：http://yp.lnxyls.cn

TS:   if (!data) return;
来源：http://ec.shxzskj.cn

Java: if (data == null) return;
来源：http://bf.huixinmuqiang.cn

Go:   if data == nil { return }
来源：http://tr.bjjhwx.cn

Ruby: return if data.nil?
来源：http://vs.jianghongdianzi.cn

C#:   if (data == null) return;
来源：http://kn.9csxet.cn

================================================================================
来源：http://ix.shtwfgs.cn

C. 函数与作用域
来源：http://xc.wgjwhj.cn

================================================================================
来源：http://rh.haigaiapp.cn

[C01] 定义函数
来源：http://oc.nicolike.cn

Py:   def add(a, b): return a + b
来源：http://qq.huixiangedu.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://yg.nszjky.cn

JS:   function add(a, b) { return a + b; }
来源：http://ua.shxzukj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://fb.huixinmuqiang.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://gy.bookmarksfly.cn

Go:   func add(a, b int) int { return a + b }
来源：http://zv.huixinmuqiang.cn

Ruby: def add(a, b); a + b; end
来源：http://wv.huixiangedu.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://zl.haigaiapp.cn

[C02] 默认参数
来源：http://mh.muxihuayi.cn

Py:   def greet(name="World"): return name
来源：http://lg.huixiangedu.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://py.colortex.cn

JS:   function greet(name = "World") { return name; }
来源：http://nm.colortex.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://vm.521024.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://xk.panjiajie.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://op.gzmigu.cn

Ruby: def greet(name = "World") = name
来源：http://iu.bjjhwx.cn

C#:   string Greet(string name = "World") => name;
来源：http://em.hahajie.cn

[C03] 可变参数
来源：http://nq.gzmigu.cn

Py:   def total(*args): return sum(args)
来源：http://ce.gzmigu.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://sl.wgjwhj.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://dz.nszjky.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://yj.shxzskj.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://og.9csxet.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://bt.bookmarksfly.cn

Ruby: def total(*nums); nums.sum; end
来源：http://iu.nicolike.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://uq.shtwfgs.cn

[C04] 命名参数 / 关键字参数
来源：http://ji.muxihuayi.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://he.haigaiapp.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://yc.huixiangedu.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wb.shxzskj.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://kn.nszjky.cn

Java: // 无：用 Builder 模式或 record
来源：http://lj.wgjwhj.cn

Go:   // 无：用配置结构体参数
来源：http://he.huanxung.cn

Ruby: f(a: 1, b: 2)
来源：http://td.9csxet.cn

C#:   f(a: 1, b: 2)
来源：http://po.shtwfgs.cn

[C05] 返回多个值
来源：http://hv.bookmarksfly.cn

Py:   return a, b
来源：http://mu.szxytkj.cn

PHP:  return [$a, $b];
来源：http://tx.lnxyls.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://zj.wgjwhj.cn

TS:   return { a, b };
来源：http://dh.bookmarksfly.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://bn.asd995.cn

Go:   return a, b
来源：http://im.haigaiapp.cn

Ruby: return a, b
来源：http://vz.huanxung.cn

C#:   return (a, b);              // ValueTuple
来源：http://fu.szxytkj.cn

[C06] 匿名函数 / lambda
来源：http://pi.nszjky.cn

Py:   square = lambda x: x * x
来源：http://tf.muxihuayi.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://gr.bjjhwx.cn

JS:   const square = x => x * x;
来源：http://ge.szsharing.cn

TS:   const square = (x: number): number => x * x;
来源：http://um.newstarts.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ul.wgjwhj.cn

Go:   sq := func(x int) int { return x * x }
来源：http://le.shtwfgs.cn

Ruby: square = ->(x) { x * x }
来源：http://ip.hnjuh.cn

C#:   Func<int, int> square = x => x * x;
来源：http://dh.jianghongdianzi.cn

[C07] 把函数作为参数传入
来源：http://pp.nicolike.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://tn.yuntaijiaju.cn

PHP:  array_map("strtoupper", $arr);
来源：http://xl.newstarts.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://dc.521024.cn

TS:   arr.map(String)
来源：http://wc.huixinmuqiang.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://rr.panjiajie.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://vm.shxzukj.cn

Ruby: arr.map(&:upcase)
来源：http://uz.szsharing.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://mm.newstarts.cn

[C08] 闭包
来源：http://jn.panjiajie.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ax.shxzskj.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://dm.hnjuh.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://st.jianghongdianzi.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://sw.muxihuayi.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://vc.jctech888.com.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ps.huixinmuqiang.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://xl.nicolike.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://oi.shtwfgs.cn

[C09] 递归
来源：http://zm.jianghongdianzi.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://sv.521024.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hq.shxzskj.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://zv.bjjhwx.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ah.nicolike.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://aq.hnjuh.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://xq.hnjuh.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://vf.nicolike.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://sh.szsharing.cn

[C10] 变量作用域
来源：http://tp.colortex.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://xk.bookmarksfly.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://bl.huanxung.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://vm.hahajie.cn

TS:   同 JS
来源：http://zy.bookmarksfly.cn

Java: 方法内为块级作用域
来源：http://mg.jianghongdianzi.cn

Go:   花括号块级作用域
来源：http://fs.chemitech.net.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ke.bjjhwx.cn

C#:   块级作用域
来源：http://kc.521024.cn

[C11] 模块导入与导出
来源：http://rs.9csxet.cn

Py:   from module import func
来源：http://ky.haigaiapp.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://uy.newstarts.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://do.szxytkj.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://da.bookmarksfly.cn

Java: import java.util.List;
来源：http://dv.jianghongdianzi.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://qm.jctech888.com.cn

Ruby: require "json"; require_relative "./util"
来源：http://yh.asd995.cn

C#:   using System.Text;
来源：http://ib.wgjwhj.cn

[C12] 立即执行函数 IIFE
来源：http://wd.lnxyls.cn

Py:   (lambda: print("run"))()
来源：http://uf.shtwfgs.cn

PHP:  (function () { echo "run"; })();
来源：http://wl.shxzukj.cn

JS:   (() => { console.log("run"); })();
来源：http://db.shtwfgs.cn

TS:   (() => { console.log("run"); })();
来源：http://qo.521024.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://aw.szsharing.cn

Go:   func() { fmt.Println("run") }()
来源：http://vs.jianghongdianzi.cn

Ruby: -> { puts "run" }.call
来源：http://jb.hahajie.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://lv.nicolike.cn

[C13] 类型声明 / 类型注解
来源：http://sf.chemitech.net.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://dh.newstarts.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://zn.jctech888.com.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://qi.colortex.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://kw.muxihuayi.cn

Java: int add(int a, int b) { return a + b; }
来源：http://ec.szsharing.cn

Go:   func add(a, b int) int
来源：http://ca.lnxyls.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ym.yuexingan06.cn

C#:   int Add(int a, int b) => a + b;
来源：http://xo.szxytkj.cn

[C14] 泛型函数
来源：http://dm.newstarts.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ad.shtwfgs.cn

PHP:  // 无泛型
来源：http://wz.colortex.cn

JS:   // 无泛型
来源：http://wk.szsharing.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hn.jianghongdianzi.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://uj.lnxyls.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://lp.huixinmuqiang.cn

Ruby: # 无泛型
来源：http://cb.bjjhwx.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://tv.nicolike.cn

[C15] 解构 / 展开参数
来源：http://dq.szsharing.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ll.lnxyls.cn

PHP:  [$a, $b] = $pair;
来源：http://jy.hahajie.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://oa.huixiangedu.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://vd.szxytkj.cn

Java: // 无解构
来源：http://ep.panjiajie.cn

Go:   // 无解构
来源：http://wb.lnxyls.cn

Ruby: a, b = pair
来源：http://np.jianghongdianzi.cn

C#:   var (a, b) = pair;
来源：http://ne.haigaiapp.cn

[C16] 函数 / 方法重载
来源：http://hd.wgjwhj.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://fi.hnjuh.cn

PHP:  // 无重载
来源：http://qv.lnxyls.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://sr.panjiajie.cn

TS:   // 用联合类型或重载签名声明
来源：http://ou.wgjwhj.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://zm.asd995.cn


<!-- 参考信息 -->